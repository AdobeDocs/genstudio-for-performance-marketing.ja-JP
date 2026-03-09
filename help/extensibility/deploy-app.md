---
title: App Builder アプリケーションのデプロイ
description: GenStudio for Performance Marketing用のApp Builder アプリまたはアドオンをデプロイします。
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
TQID: https://experienceleague.adobe.com/7Z4Fb-jPi4FHrTeOgHxxO4fl982sqri-7uEDoylFF-s
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: ad3738c7-91ac-48ed-a914-fd0b03f89396
  - id: bfaa655b-e017-428d-80d0-09de2183b296
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: da3860b0-d637-47df-bef0-273751180266
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 447
ht-degree: 0%

---

# アプリのデプロイ

アプリを実行すると、デプロイ前にアドオンの動作の予備スナップショットが提供されます。 これはデバッグに役立ちます。

## アプリの実行

`https://localhost:9080` でアプリを実行します。

```bash
aio app run
```

## アプリのデプロイ

1. デプロイメント ワークスペースに移動します。

   ```bash
   aio app use -w [deployment_workspace]
   ```

2. アプリをデプロイします。

   ```bash
   aio app deploy
   ```

## 再デプロイメントを強制

アプリを承認用に再送信しなくても、アプリのビルドとデプロイメントを強制的に行うことができます。

>[!NOTE]
>
>ビルドおよびデプロイメントを強制的に実行すると、既存のデプロイメントが上書きされます。**最初にテスト環境で** アプリのテストを十分に行います。

```bash
aio app build --force-build
```

```bash
aio app deploy --force-deploy
```

## ビルドとデプロイを同時に

```bash
aio app deploy --force-build --force-deploy
```

## 新しいアプリの検索

デプロイ後、GenStudio for Performance Marketingで新しいアプリを表示できます。

### URL で表示

`query` パラメーターをGenStudio for Performance Marketingの URL に追加して、新しいアプリを確認します。

```txt
https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create
```

### UI で表示

新しい拡張機能は、デプロイした拡張機能のタイプに応じて、UI の様々な場所に表示されます。 現在利用可能な拡張ポイントは次のとおりです。

* コンプライアンス拡張機能。次の機能が含まれます。
   * [*プロンプト拡張ポイント*](#find-prompt-extensions)：顧客は LLM 生成にコンテキストを追加できます。
   * [*検証拡張ポイント*](#find-validation-extensions)：顧客が LLM から生成されたコンテンツを検証できます。 検証は、多くの場合、迅速な延長と組み合わされて、延長された迅速なコンテンツが顧客の要件（例えば、医療用医薬品の請求や法務）に準拠していることを確認します
* [デジタルアセット管理（DAM）拡張機能](#find-dam-extensions)
* [テンプレート拡張機能](#find-template-extensions)
* [翻訳拡張機能](#find-translation-extensions)

### プロンプト拡張機能の検索

プロンプト拡張機能は、テンプレートの **パラメーターセクション** にある **アドオン** ドロップダウンで見つかります。

![&#x200B; プロンプト拡張機能 &#x200B;](./select-prompt-ext.png){width="600" zoomable="yes"}

アドオンダイアログが開き、LLM 生成用に追加する追加のコンテキストを選択できます。

![&#x200B; プロンプト拡張機能ドロップダウン &#x200B;](./select-prompt-dropdown.png){width="600" zoomable="yes"}

### 検証拡張機能の検索

検証拡張機能は、プロンプト生成後、結果と共に表示される右側のサイドナビで見つけることができます。

![&#x200B; 検証の拡張 &#x200B;](./validation-ext.png){width="600" zoomable="yes"}

選択した拡張機能を実行して、生成されたコンテンツを検証します。

![&#x200B; 有効な検証 &#x200B;](./validation-valid.png){width="600" zoomable="yes"}

### DAM 拡張機能の検索

デジタルアセット管理（DAM）拡張機能は、テンプレートの **パラメーターセクション** でコンテンツを選択すると見つかります。 **場所を選択** ドロップダウンの下部を参照して、アドオンを表示します。

![DAM 拡張機能 &#x200B;](./dam-ext.png){width="600" zoomable="yes"}

### テンプレート拡張機能の検索

テンプレートを選択すると、テンプレート拡張機能が「**外部テンプレートアプリ**」タブに表示されます。 このタブは、選択するテンプレートアプリがある場合にのみ表示されます。

![&#x200B; テンプレート拡張機能 &#x200B;](./template-ext.png){width="600" zoomable="yes"}


### 翻訳拡張機能の検索

GenStudioのデフォルトの翻訳を使用する代わりに、翻訳拡張ポイントを使用して、プロキシを介して独自の翻訳サービスを導入します。
これらの拡張機能には UI の場所がありません。

拡張機能が登録されている場合は、提供された翻訳サービスが使用されます。 それ以外の場合は、デフォルトのGenStudio翻訳サービスが使用されます。



アドオンに満足したら、`query` パラメーターを指定せずに配布する準備が整います。

これで、[&#x200B; アプリを配布 &#x200B;](distribute-app.md) できます。
