---
title: App Builder アプリケーションの作成
description: GenStudio for Performance Marketingを拡張するアプリまたはアドオンの作成を開始します。
feature: Extensibility
exl-id: 4e757dd4-a02d-472c-bc13-6f27dffa48f2
source-git-commit: 04a4f6432c5db87489e39f9396a7782c86441695
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# App Builder アプリの開発

GenStudio for Performance Marketingのネイティブ機能を拡張する開発者は、[Adobe App Builder](https://developer.adobe.com/app-builder/) を使用して、拡張可能なアプリやアドオンを作成、送信、デプロイします。

>[!BEGINSHADEBOX]

**前提条件**:

* Node.js （バージョン 20.x 以降）

* npm （Node.js とともにパッケージ化）

* Adobe Developer コマンドラインインターフェイス（CLI）。 npm と共にインストールするには、次のコマンドを実行します：`npm install -g @adobe/aio-cli`

>[!ENDSHADEBOX]

## アプリの構造

GenStudio for Performance Marketing アドオンはApp Builderのアプリであり、他のApp Builder アプリと同じ基本コンポーネントが含まれています。

### ビルドおよび設定ファイル

App Builder アプリケーションの主要なコンポーネントには、これらのビルドファイルおよび設定ファイルが含まれます。 このリストには、すべてのビルドファイルと設定ファイルが含まれるわけではありません。

* `README.md`: アプリに関する一般情報が含まれます。

* TS アプリケーション ファイル：

   * `package.json`
   * `package-lock.json`
   * `eslint`
   * `tsconfig`
   * `jest test up`

* App Builder設定ファイル：

   * `app.config.yaml`
   * `ext.config.yaml`：アドオンの設定ファイル
   * `app.config.yaml`：アドオンの設定ファイル（アプリをGenStudio for Performance Marketing アドオンとして定義することを含む）
   * `.aio`
   * `.env`: `.env` ファイルをソース管理にコミットしないでください。

### ソースコード

```
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

### Source コードコンポーネント

* `ExtensionRegistration.tsx`: ホストアプリ（GenStudio for Performance Marketing）がアドオンを読み込んで表示するために必要な API を定義します。

* `App.tsx`：他のコンポーネントへのルーティングを定義するメインアプリコンポーネント。

* `AdditionalContextDialog.tsx`：追加のコンテキストアドオンを表示するためのダイアログコンポーネント。

* `RightPanel.tsx`：検証アドオンのダイアログコンポーネント

* `Helper` コンポーネント：`ClaimsChecker` を含みます。

## 既存のアプリからのApp Builder アプリの作成

サンプルアプリを使用して、アドオンの作成をすぐに開始できます。

**既存のアプリからApp Builder アプリを作成するには**:

1. [GenStudio UIX Examples](https://github.com/adobe/genstudio-uix-examples) リポジトリからサンプルアプリをダウンロードします。

1. [Adobe Developer Console](https://developer.adobe.com/console/) のApp Builder プロジェクトワークスペースから、「[!UICONTROL &#x200B; すべてダウンロード &#x200B;]」を選択してプロジェクトの詳細をダウンロードします。

1. 好みの統合開発環境（IDE）で、サンプルアプリをローカルで開きます。

1. Adobe Developer コマンドラインインターフェイスによる認証：

   ```bash
   aio login
   ```

1. JSON ファイルをダウンロードし、アプリを作成します。

   ```bash
   aio app use '/path/to/your/downloaded/app-builder/project/details/config.json'
   ```

## アドオンにカスタムコードを追加

`AdditionalContextDialog.tsx` ファイルと `RightPanel.tsx` ファイルでアドオンコードを定義します。 これら 2 つのファイルは、ユーザーがアドオンにアクセスしたときのポップアップの外観と動作を定義します。

* `AdditionalContextDialog.tsx`: _コンテキストを追加_ アドオンを使用する予定がある場合は、このコンポーネントを定義します。 ユーザーは、_のプロンプトドロワーで_ アドオン [!DNL Create] をクリックすると、このコンポーネントを操作します。

* `RightPanel.tsx`：右側のパネル _アドオン_ エクスペリエンスの検証）を使用する予定がある場合は、このコンポーネントを定義します。 ユーザーは、エクスペリエンスドラフトの右側のパネルで検証アドオンをクリックすると、このコンポーネン [!DNL Create] を操作します。

## アプリ開発のベストプラクティス

開発環境を維持すると、アプリの開発およびデプロイメントエラーを回避できます。

* 古いバージョンのサンプルアプリを使用している場合は、依存関係を再インストールしてアップグレードします。

  ```bash
  rm -rf node_modules package-lock.json && npm i
  ```

* GenStudio UIX SDKをアップグレードします。 最新バージョンの [GenStudio UIX SDK](https://github.com/adobe/genstudio-uix-sdk) を使用していることを確認してください。 最新のGenStudioの変更内容の使用方法については [&#128279;](https://github.com/adobe/genstudio-uix-examples)SDK UIX のサンプルリポジトリを参照してください。

これで、[&#x200B; アプリをデプロイ &#x200B;](deploy-app.md) する準備が整いました
