---
title: Adobe GenStudio for Performance Marketing用Photoshop プラグイン
description: GenStudio for Performance MarketingのPhotoshop プラグインをインストール、設定、使用する方法について説明します。
feature: Generative AI
role: User
exl-id: e3f57acd-f2dd-4957-aa5e-c97595a29899
TQID: https://experienceleague.adobe.com/9p-ohsF1gIVKv3vwjnP9o675l3gJT3tVxx34PefFzCQ
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: e0aa398c-6185-4e77-8cf7-2561c578c181
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 816
ht-degree: 1%

---

# GenStudio for Performance Marketing用Photoshop プラグイン

GenStudio for Performance Marketing Photoshop プラグインは、オンブランドのコンテンツを生成できるパネルをAdobe Photoshopに追加します。

このページでは、プラグインのインストールおよび設定方法と使用方法について説明します。

このプラグインの機能は次のとおりです。

* Adobe IDでGenStudio for Performance Marketing インスタンスにログインします
* GenStudio for Performance Marketing コンテンツ生成フィールドをPhotoshop ドキュメントのテキストレイヤーにマッピングする
* コンテンツを生成するためのブランド、製品、ペルソナおよびテキストプロンプトの指定
* オプションで、画像を追加してテンプレート画像を置き換えます
* 生成されたオンブランドコンテンツのバリエーションのプレビュー
* 生成されたコンテンツを現在のドキュメント内のマップされたレイヤーに適用
* オンブランドのコンテンツ翻訳の作成
* 生成された [!DNL Experiences] をGenStudio for Performance Marketingに書き出す

>[!VIDEO](https://video.tv.adobe.com/v/3478808?learn=on)

## プラグインのインストール

次の手順に従ってプラグインをインストールします。

### 前提条件

* Creative Cloud デスクトップアプリケーション
* Photoshop、最小バージョン 25.6.0

### インストール手順

1. Adobe ExchangeのCreative Cloud Marketplace からプラグインをダウンロードして更新します。
1. Adobe Exchangeで **GenStudio Plugin for Photoshop** を検索します。
1. 画面の指示に従って、プラグインをインストールします。

### プラグインのアンインストール

1. Creative Cloud デスクトップアプリケーションを起動します。
1. 「**[!UICONTROL プラグイン]**」オプションをクリックします。
1. Creative Cloud GenStudio カードの省略記号 **[!UICONTROL （...）]** をクリックし、オプションを選択します。
1. 「**アンインストール**」を選択します。

## テンプレートの作成

コンテンツを生成するには、Photoshop ドキュメントからGenStudio for Performance Marketing テンプレートを作成する必要があります。

GenStudio対応テンプレートを作成するには：

1. Photoshopでドキュメントを開きます。
1. 生成されたコンテンツのテキストレイヤーを特定します。
1. 画層の名前をフィールド名表記形式 `{<name_of_generated_field>}` に変更します。 例：`{body}`、`{headline}`、`{cta}`。
1. すべてのレイヤーのレイヤー名を変更します [&#x200B; テンプレートタイプ用のチャネルに必要なフィールド &#x200B;](../../user-guide/templates/customize-template.md#recognized-field-names)。

| チャネル | 生成の必須フィールド | 生成用のオプション フィールド |
| --- | --- | --- |
| LinkedIn | `{on_image_text}`, `{image}` | `{headline}`, `{introductory_text}`, `{cta}`, `{website_url}` |
| Meta | `{on_image_text}`, `{image}` | `{body}`, `{headline}`, `{cta}`, `{website_url}`, `{display_link}` |
| ディスプレイ | `{body}`, `{image}` | `{headline}`, `{cta}`, `{website_url}` |

複数の画層で同じフィールド指定を共有できますが、各画層で指定できるフィールドは 1 つだけです。 例えば、ドキュメントに複数のアートボードがある場合：

* 各アートボードに `{headline}` レイヤーを指定できます。
* 1 つのアートボードに複数の `{headline}` レイヤーを指定できます。
* 1 つのレイヤーが `{headline}` と `{cta}` の両方のフィールド名を受け取るように指定することはできません。

### テンプレートサイズの要件

#### Meta テンプレート

Instagram および Facebook の投稿の場合：

* 幅：1080 px （固定）
* 高さ：1080 ピクセルまたは 1350 ピクセル

Instagram や Facebook のストーリーについて：

* 幅：1080 px （固定）
* 高さ：1920 ピクセル

プラグインは、テンプレートの高さに基づいて、生成されるエクスペリエンスのクロムを決定します。

#### 表示テンプレート

固定サイズの要件はありません。 表示テンプレートは、任意のサイズをサポートします。

#### LinkedIn テンプレート

* 幅：1200 px （固定）
* 高さ：1200 ピクセル、628 ピクセル、2292 ピクセル、1800 ピクセル、または 1500 ピクセル

これで、ドキュメントをプラグインで使用する準備が整いました。

## 新しいコンテンツを生成

1. Photoshopを開きます。
1. 作成したGenStudio対応テンプレートドキュメントを開くか（上記の手順を参照）、GenStudio for Performance Marketing スターターテンプレート `branding-template-acrobat-handlebars.psd` を使用します。
1. **[!UICONTROL プラグイン]**/**[!UICONTROL GenStudio]** でプラグインパネルを開きます。
1. 「**[!UICONTROL ログイン]**」ボタンをクリックします。 URL を開く権限を要求するメッセージが表示されたら、オプションで **選択内容を保存** のチェックボックスをオンにし、「**[!UICONTROL 許可]** をクリックします。
1. Web ブラウザーを使用して、GenStudio for Performance Marketingへのアクセス権を持つプロファイルでログインします。
1. 開いたテンプレートに適用されるチャネル（Meta、LinkedIn またはディスプレイ）を選択します。
   ![&#x200B; チャネル選択 &#x200B;](./ps-select-channel.png){width="300" zoomable="yes"}
1. コンテンツ生成の [!DNL Brand]、[!DNL Persona] および [!DNL Product] コンテキストを選択します。
   ![&#x200B; ブランド、ペルソナ、製品の選択 &#x200B;](./ps-select-box.png){width="300" zoomable="yes"}
1. 作成するバリエーションの数を選択します。
1. **[!UICONTROL コンテンツを選択]** の下にあるボタンを使用して、アセットから画像を参照して選択します。 最近追加された 40 個のアセットが最初に表示され、他のアセットを検索できます。 選択した画像は、テンプレートに合わせて自動的にサイズ変更されます。
1. **[!UICONTROL テキストプロンプト]** ボックスにコンテンツのテキストプロンプトを入力します。
1. 「**[!UICONTROL 生成]** ボタンをクリックします。 バリエーションは、プラグインパネルのカードに表示されます。

新しいドキュメントがPhotoshop Workspace に追加され、生成されたコンテンツがテンプレートフィールドに適用されます。 これらのドキュメントには、番号の付いたバリエーション接尾辞が付きます。

## コンテンツの翻訳

ユーザーは、コピーの生成後に、コンテンツをサポートされている言語に翻訳できます。

1. プラグインで広告コピーを生成したら、「**[!UICONTROL 翻訳]**」をクリックします。
1. 翻訳する 1 つ以上の言語を選択します。
1. 「**[!UICONTROL 翻訳]** ボタンをクリックします。

新しいドキュメントがPhotoshop Workspace に追加され、生成されたコンテンツがテンプレートフィールドに適用されます。 これらのドキュメントには、番号の付いたバリエーション接尾辞が付きます。

## GenStudioへのエクスペリエンスの書き出し

ユーザーは、コンテンツの生成または翻訳後に書き出しを選択できます。 書き出されたエクスペリエンスは、GenStudio for Performance Marketingの「コンテンツ」セクションに入力されます。

![&#x200B; 「コンテンツ」セクションに表示される、書き出されたアセット &#x200B;](./content-assets.png){width="90%"}

## トラブルシューティング

生成されたバリエーションでテキストや画像が置き換えられない場合は、次のベストプラクティスとヒントを考慮してください。

### マッピングされたフィールド

テキストまたは画像が置き換えられない場合、確認フィールドは、括弧 `()` ではなく、中括弧 `{}` で正しくマッピングされます。

### 使用可能なフォントの確認

生成時に置換を行うには、テキストフィールドのフォントがマシン上で使用可能である必要があります。 ファイルで使用されているすべてのフォントがお使いのマシンで使用できることを確認します（特に、ファイルが他のユーザーのマシンで作成された場合）。

### フィールドマッピングの例外

{{$include /help/_includes/field-mapping-exceptions.md}}
