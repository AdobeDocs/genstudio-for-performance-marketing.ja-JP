---
title: App Builder アプリのデプロイ
description: GenStudio for Performance Marketing用のApp Builder アプリまたはアドオンをデプロイします。
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
TQID: https://experienceleague.adobe.com/7Z4Fb-jPi4FHrTeOgHxxO4fl982sqri-7uEDoylFF-s
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: ad3738c7-91ac-48ed-a914-fd0b03f89396id: bfaa655b-e017-428d-80d0-09de2183b296id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: da3860b0-d637-47df-bef0-273751180266
source-git-commit: 3a50cdb378d024370808680ec9b606c789429dc2
workflow-type: tm+mt
source-wordcount: 501
ht-degree: 0%

---

# アプリをデプロイ

アプリを実行すると、展開前にアドオンの動作の予備スナップショットを入手できます。 これはデバッグに役立ちます。

## アプリの実行

`https://localhost:9080`でアプリを実行：

```bash
aio app run
```

## アプリのデプロイ

1. デプロイメントワークスペースに移動します。

   ```bash
   aio app use -w [deployment_workspace]
   ```

2. アプリをデプロイします。

   ```bash
   aio app deploy
   ```

## 強制的に再展開

アプリのビルドとデプロイメントを、承認のために再送信せずに強制的に行うことができます。

>[!NOTE]
>
>ビルドとデプロイメントを強制すると、既存のデプロイメントが上書きされます。 **テスト環境でアプリを徹底的にテストします**。

```bash
aio app build --force-build
```

```bash
aio app deploy --force-deploy
```

## ビルドとデプロイを同時に実行

```bash
aio app deploy --force-build --force-deploy
```

## 新しいアプリを探す

デプロイメント後、GenStudio for Performance Marketingで新しいアプリを表示できます。

### URLで表示

GenStudio for Performance Marketing URLに`query` パラメーターを追加して、新しいアプリを参照します。

```txt
https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create
```

### UIでの表示

新しい拡張機能は、デプロイした拡張機能のタイプに応じて、UIの様々な場所に表示されます。 現在使用可能な拡張ポイントは次のとおりです。

* 以下を含むコンプライアンス拡張機能：
   * [*プロンプト拡張ポイント*](#find-prompt-extensions)&#x200B;により、顧客はLLM生成に追加のコンテキストを追加でき、
   * [*検証の拡張ポイント*](#find-validation-extensions)。顧客は生成されたコンテンツをLLMから検証できます。 検証は、多くの場合、プロンプト拡張機能と組み合わせて使用され、拡張プロンプトで生成されたコンテンツが、お客様の要件（医療用医薬品の請求、法的など）に準拠していることを確認します
* [デジタルアセット管理（DAM）拡張機能](#find-dam-extensions)
* [テンプレート拡張機能](#find-template-extensions)
* [翻訳拡張機能](#find-translation-extensions)

### プロンプト拡張機能を探す

プロンプト拡張機能は、テンプレートの&#x200B;**パラメーターセクション**&#x200B;の&#x200B;**アドオン** ドロップダウンにあります。

![ プロンプト拡張機能](./select-prompt-ext.png){width="600" zoomable="yes"}

アドオンダイアログが開き、LLM生成用に追加する追加のコンテキストを選択できます。

![拡張機能のプロンプト ドロップダウン ](./select-prompt-dropdown.png){width="600" zoomable="yes"}

### 検証拡張機能を探す

検証の拡張機能は、プロンプトの生成後、結果とともに表示される右側のサイドナブに表示されます。

![拡張機能の検証](./validation-ext.png){width="600" zoomable="yes"}

選択した拡張機能を実行して、生成されたコンテンツを検証します。

![有効な検証](./validation-valid.png){width="600" zoomable="yes"}

エラーがある場合は、拡張機能を使用して、プログラムでエクスペリエンスのコピーを更新できます。 「**[!UICONTROL コピー]**」ボタンをクリックすると、候補テキストがクリップボードにコピーされます。 「**[!UICONTROL 適用]**」ボタンをクリックすると、生成されたエクスペリエンスの特定のテキストボックスにテキストが適用されます。

![ コピーと適用ボタンを表示する検証エラー](./validation-copy-apply.png){width="600" zoomable="yes"}

### DAM拡張機能を探す

デジタルアセット管理（DAM）拡張機能は、テンプレートの&#x200B;**パラメーターセクション**&#x200B;でコンテンツを選択する際に見つかります。 **場所を選択** ドロップダウンの下部にアドオンが表示されます。

![DAM拡張機能](./dam-ext.png){width="600" zoomable="yes"}

### テンプレート拡張機能を探す

テンプレートを選択すると、**外部テンプレートアプリ** タブにテンプレート拡張機能が表示されます。 このタブは、選択するテンプレートアプリがある場合にのみ表示されます。

![ テンプレート拡張機能](./template-ext.png){width="600" zoomable="yes"}


### 翻訳拡張機能を探す

翻訳拡張機能ポイントを使用すると、GenStudioのデフォルトの翻訳を使用する代わりに、プロキシを通じて独自の翻訳サービスを利用できます。
これらの拡張機能にはUIの場所がありません。

拡張機能が登録されている場合は、提供された翻訳サービスが使用されます。 それ以外の場合は、デフォルトのGenStudio翻訳サービスが使用されます。



アドオンに問題がなければ、`query` パラメーターを指定せずに配布しましょう。

これで、[ アプリを配布できます](distribute-app.md)。
