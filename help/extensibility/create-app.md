---
title: App Builder アプリの作成
description: GenStudio for Performance Marketingを拡張するアプリまたはアドオンの作成を開始します。
feature: Extensibility
exl-id: 4e757dd4-a02d-472c-bc13-6f27dffa48f2
TQID: https://experienceleague.adobe.com/-GBttZv63YVWezBz1o9yrxvd-Uu5mbP-Aqh7Tm-kco4
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: b6b93e3513804919d43a663bb899e67556a4cbcd
workflow-type: tm+mt
source-wordcount: 496
ht-degree: 1%

---

# App Builder アプリの開発

GenStudio for Performance Marketingのネイティブ機能を拡張する開発者は、[Adobe App Builder](https://developer.adobe.com/app-builder/)を使用して、拡張可能なアプリまたはアドオンを作成、送信、デプロイします。

>[!BEGINSHADEBOX]

**前提条件**:

* Node.js （バージョン 20.x以降）

* npm （Node.jsとパッケージ化）

* Adobe Developer コマンドラインインターフェイス（CLI）。 npmでインストールするには、次を実行します：`npm install -g @adobe/aio-cli`

>[!ENDSHADEBOX]

## アプリ構造

GenStudio for Performance Marketing アドオンはApp Builder アプリケーションであり、他のApp Builder アプリケーションと同じ基本コンポーネントを含んでいます。

### ビルドと設定ファイル

App Builder アプリケーションの主要なコンポーネントには、以下のビルドファイルと設定ファイルが含まれます。 このリストには、すべてのビルドファイルと設定ファイルが含まれていません。

* `README.md`: アプリに関する一般的な情報が含まれます。

* TS アプリファイル：

   * `package.json`
   * `package-lock.json`
   * `eslint`
   * `tsconfig`
   * `jest test up`

* App Builder設定ファイル：

   * `app.config.yaml`
   * `ext.config.yaml`: アドオンの設定ファイル。
   * `app.config.yaml`: アドオンの設定ファイル （アプリをGenStudio for Performance Marketing アドオンとして定義することを含む）。
   * `.aio`
   * `.env`: `.env` ファイルをソース管理にコミットしないでください。

### ソースコード

```txt
- src/
    - genstudiopem/
        - web-src/
            - src/
                - components/
                - utils/
                - Constants.ts
                - index.tsx
                - index.css
                - utils.ts
        - index.html
```

### Sourceのコードコンポーネント

* `ExtensionRegistration.tsx`: ホストアプリ （GenStudio for Performance Marketing）がアドオンを読み込んで表示するために必要なAPIを定義します。

* `App.tsx`：他のコンポーネントへのルーティングを定義するメイン アプリ コンポーネント。

* `AdditionalContextDialog.tsx`：追加のコンテキスト アドオンを表示するためのダイアログ コンポーネント。

* `RightPanel.tsx`：検証アドオンのダイアログコンポーネント。

* `Helper` コンポーネント：`ClaimsChecker`が含まれます。

## 既存のアプリからApp Builder アプリを作成する

サンプルアプリを使えば、アドオン作成をすぐに始められます。

**既存のアプリからApp Builder アプリを作成するには**:

1. [GenStudio UIX Examples](https://github.com/adobe/genstudio-uix-examples) リポジトリからサンプルアプリをダウンロードします。

1. [Adobe Developer Console](https://developer.adobe.com/console/)のApp Builder プロジェクト ワークスペースから、「[!UICONTROL すべてをダウンロード &#x200B;]」を選択して、プロジェクトの詳細をダウンロードします。

1. 使用する統合開発環境（IDE）でサンプルアプリをローカルに開きます。

1. Adobe Developer コマンドラインインターフェイスを使用して認証します。

   ```bash
   aio login
   ```

1. JSON ファイルをダウンロードし、アプリを作成します。

   ```bash
   aio app use '/path/to/your/downloaded/app-builder/project/details/config.json'
   ```

## アドオンにカスタムコードを追加しましょう

`AdditionalContextDialog.tsx`と`RightPanel.tsx` ファイルでアドオンコードを定義してください。 これら2つのファイルは、ユーザーがアドオンにアクセスした際のポップアップの外観と動作を定義します。

* `AdditionalContextDialog.tsx`: _Add Context_ アドオンを使用する場合は、このコンポーネントを定義します。 ユーザーは、[!DNL Create]のプロンプトドロワーで&#x200B;_アドオン_&#x200B;をクリックすると、このコンポーネントを操作できます。

* `RightPanel.tsx`: _右パネル_ アドオンを使用する場合は、このコンポーネントを定義します（エクスペリエンス検証）。 ユーザーは、[!DNL Create] エクスペリエンスドラフトの右側のパネルにある検証アドオンをクリックすると、このコンポーネントを操作できます。

## アプリ開発のベストプラクティス

開発環境を維持することで、アプリの開発とデプロイメントエラーを回避できます。

* 古いバージョンのサンプルアプリを使用している場合は、依存関係を再インストールしてアップグレードします。

  ```bash
  rm -rf node_modules package-lock.json && npm i
  ```

* GenStudio UIX SDKをアップグレードします。 最新バージョンの[GenStudio UIX SDK](https://github.com/adobe/genstudio-uix-sdk)を使用していることを確認してください。 最新のSDKの変更点の使用方法については、[GenStudio UIX サンプルリポジトリ &#x200B;](https://github.com/adobe/genstudio-uix-examples)を参照してください。

これで、[&#x200B; アプリをデプロイする準備が整いました](deploy-app.md)
