---
title: テンプレートのカスタマイズ
description: Adobe GenStudio for Performance Marketing用テンプレートをパーソナライズおよび最適化する方法について説明します。
level: Intermediate
feature: Templates, Content
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: ce08231cb723bec3d80a732837b72a435d3b552d
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 0%

---

# テンプレートのカスタマイズ

_Handlebars_ テンプレート言語を使用して、Adobe GenStudio for Performance Marketing用のHTMLテンプレートを調整します。 [!DNL Handlebars] の構文では、コンテンツのプレースホルダーとして中括弧を使用した通常のテキストを使用します。 テンプレートの準備方法については、_Handlebars 言語ガイド_ の [`What is [!DNL Handlebars]?`](https://handlebarsjs.com/guide/#what-is-handlebars) を参照してください。

次のいくつかの節では、コンテンツプレースホルダーを追加する方法、不要な要素をプレビューから非表示にする方法、静的コンテンツへのリンクを管理する方法について説明します。 テンプレートの準備が整ったら、[GenStudio for Performance Marketingにアップロード ](use-templates.md#upload-a-template)、カスタムテンプレートに基づいてパーソナライズされたメールの生成を開始できます。

## コンテンツプレースホルダー

GenStudio for Performance Marketingは、テンプレート内の特定の [ 要素 ](use-templates.md#template-elements) を認識しますが、それは認識されたフィールド名で識別した場合のみです。

テンプレートの head または body 内では、GenStudio for Performance Marketingに実際のコンテンツをテンプレートに入力させる必要がある場合、[!DNL Handlebars] 構文をコンテンツプレースホルダーとして使用できます。 GenStudio for Performance Marketingは、[ 認識された _field_ name](#recognized-field-names) に基づいてコンテンツプレースホルダーを認識および解釈します。

例えば、[!DNL Handlebars] の構文で `{{ headline }}` を使用して、メールのヘッドラインを配置する場所を示すことができます。

```handlebars
<div>{{headline}}</div>
```

### 認識されたフィールド名

次の表に、テンプレートへの母集団に対してGenStudio for Performance Marketingで認識されるフィールド名を示します。 GenStudio for Performance Marketingでコンテンツを生成する必要があるテンプレートに、[!DNL Handlebars] 構文を使用してこれらのフィールド名を追加します。

| フィールド | 役割 | チャネルテンプレート |
| -------------- | ---------------------- | ------------------------------ |
| `pre_header` | プリヘッダー | メール |
| `headline` | 見出し | メール <br> メタ広告 |
| `body` | 本文コピー | メール <br> メタ広告 |
| `cta` | コールトゥアクション | メール <br> メタ広告 |
| `on_image_text` | 画像テキスト上 | メタ広告 |
| `image` | 画像 | メール <br> メタ広告 |
| `brand_logo` | 選択したブランドのロゴ <br> 推奨使用については、[ ブランドロゴフィールド名 ](#brand-logo-field-name) を参照してください。 | メールメ <br> タ広告 |

GenStudio for Performance Marketingでは、特定のフィールドに次のテンプレートで自動的に入力されます。

- **メールテンプレート** で `subject` フィールドを識別する必要はありません
- **メタ広告テンプレート** では、「`headline`」、「`body`」、「`CTA`」フィールドを識別する必要はありません

<!--
- **Display Ads template** does not require you to idenitify the `CTA` field
-->

>[!WARNING]
>
>instagram広告の場合、生成されたヘッドラインは最終的なエクスペリエンスには表示されません。

テンプレートをGenStudio for Performance Marketingにアップロードできるフィールドは 20 個までです。 メールでは `subject` フィールドが自動的に生成されるので、1 つのフィールドとしてカウントされます。 つまり、メールテンプレートでは 19 個のフィールドを使用できます。

>[!TIP]
>
>GenStudio for Performance Marketingの [ テンプレートプレビュー ](#template-preview) を使用して、テンプレートを検証できます。

#### ブランドロゴフィールド名

現時点では、テンプレートのアップロードに使用するブランドロゴを選択することはできません。 次の例は、ブランドロゴを条件に応じてレンダリングする 2 つの方法を示しています。 各方法では、ソースを検証し、ブランドロゴが使用できない場合に備えてデフォルトまたは代替の画像を提供し、スタイルを適用します。

**例 1**：組み込みヘルパー条件 [!DNL Handlebars]HTML `img src` 属性に直接使用する

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**例 2**：組み込み条件ステートメント [!DNL Handlebars] 使用してHTMLをタグ `img` 囲む：

```handlebars
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

#### 手動フィールド名

その他のすべてのフィールド名は、手動で入力されたフィールドとして扱われます。

編集可能なセクションを作成するには、セクション名の周りに二重括弧を追加します。

```handlebars
{{customVariable}}
```

### セクションまたはグループ

_セクション_ このセクションのフィールドには高い一貫性が必要であることをGenStudio for Performance Marketingに伝えます。 この関係を確立すると、AI がセクションのクリエイティブ要素に一致するコンテンツを生成するのに役立ちます。

フィールド名に任意の接頭辞を使用して、フィールドがセクションまたはグループの一部であることを示します。 例えば、ハイライトされた領域に表示されるコンテンツにスポットライトを当てることができます。

- `pod1_headline`
- `pod1_body`

各セクションは、各フィールドタイプの 1 つのみを使用できます。 上記の例では、`pod1` セクションは 1 つの `pod1_headline` フィールドのみを使用できます。

テンプレートには、最大で次の 3 つのセクションを含めることができます。

- `headline`
- `body`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`

GenStudio for Performance Marketingは `pod1_headline` が `pod2_body` よりも `pod1_body` と密接に関係していることを理解しています。

## テンプレートのプレビュー

[ テンプレートをアップロード ](use-templates.md#upload-a-template) すると、GenStudio for Performance MarketingはHTMLファイルをスキャンして、認識されたフィールドを探します。 プレビューを使用して [ テンプレート要素 ](use-templates.md#template-elements) を確認し、それらが [ 認識されたフィールド名 ](#recognized-field-names) で正しく識別されたことを確認します。

メールテンプレートのプレビューの例：

![ プレビューフィールドが検出されました ](../../assets/template-detected-fields.png){width="650"}

### プレビューを制御

組み込みヘルパー（特定のアクションを実行する [!DNL Handlebars] テンプレート言語の特別な式）を使用して、特別なコンテンツの表示を制御できます。 例えば、プレビューリンクをクリーンに保ちながら、書き出されたテンプレート内のリンクにトラッキングパラメーターを追加する条件ステートメントを追加できます。

テンプレートのレンダリング時には `_genStudio.browser` の値が設定され、テンプレートの書き出し時には `genStudio.export` の値が設定されます。 条件付きラッパーを使用して、メールの上部に特定のコンテンツを含めることもできます。例えば、テンプレートを書き出しに使用する場合です。

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

もう 1 つの例として、GenStudio for Performance Marketingでテンプレートをプレビューする際に、トラッキングコードを使用しないようにすることがあります。 次の例では、プレビューリンクをクリーンな状態に保ちながら、書き出されたテンプレート内のリンクにトラッキングパラメーターを追加する方法を示します。

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## 静的コンテンツ

多くの場合、メールおよびメタテンプレートは、GenStudio for Performance Marketingの外部でホストされる画像や CSS ファイルにリンクされています。 GenStudio for Performance Marketingがこれらのテンプレートまたはそれらから派生したエクスペリエンスのサムネールを生成する際、正しいクロスオリジンリソース共有（CORS）ヘッダーがない場合、これらの外部リソースが無視される場合があります。

サムネール生成プロセスの実行中にこれらのリソースを使用できるようにするには、次の 2 つのオプションを検討します。

1. **CORS ヘッダーを使用**：ホストサーバーは、実稼動環境の値に設定された `Access-Control-Allow-Origin` ヘッダーで応答 `https://experience.adobe.com` 送信する必要があります。 これにより、GenStudio for Performance Marketingはリソースにアクセスして含めることができます。

1. **データ URL を使用**：データ URL を使用して、外部リソースをテンプレートに直接埋め込みます。 この方法では、CORS の制限をバイパスし、サムネールの生成中にリソースを利用できるようにします。

## テンプレートの例

+++例：1 つのセクションを持つメールテンプレート

次に、1 つのセクションを含むメールのHTMLテンプレートの基本的な例を示します。 ヘッドには、スタイル設定用のシンプルなインライン CSS が含まれています。 本文には、`pre-header`、`headline`、`image` [ プレースホルダー ](#content-placeholders) が含まれており、メール生成プロセス中にGenStudio for Performance Marketingでコンテンツを挿入するために使用されます。

```handlebars {line-numbers="true" highlight="13"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    </div>
</body>
</html>
```

+++

+++例：複数のセクションを持つメールテンプレート

以下は、上記の例と同じHTMLテンプレートですが、さらに 2 つのセクションがあります。 ヘッドには、グループのスタイル設定に使用するインライン CSS が含まれています。 本文では、プレフィックスを使用して、[ コンテンツプレースホルダー ](#content-placeholders) を含む 2 つのグループを使用します。

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
        .pod {
            background-color: #f8f8f8;
            margin: 10px;
            padding: 20px;
            border-radius: 5px;
        }
        .pod h2 {
            color: #333;
        }
        .pod p {
            color: #666;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    <!-- Pod1 -->
        <div class="pod">
            <h2>{{ pod1_header }}</h2>
            <p>{{ pod1_body }}</p>
        </div>
        <!-- End of Pod1 -->
    <!-- Pod2 -->
        <div class="pod">
            <h2>{{ pod2_header }}</h2>
            <p>{{ pod2_body }}</p>
        </div>
        <!-- End of Pod2 -->
    </div>
</body>
</html>
```

+++

+++例：メタ広告テンプレート

次に、メタ広告テンプレートの基本的な例を示します。 ヘッドには、スタイル設定用のインライン CSS が含まれています。 本文では、プレフィックスを使用して [ コンテンツプレースホルダー ](#content-placeholders) を使用します。

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adobe</title>
    <style>
        .ad-container {
            width: 300px;
            border: 1px solid #ddd;
            padding: 16px;
            font-family: Arial, sans-serif;
        }
        .ad-image {
            width: 100%;
            height: auto;
        }
        .ad-headline {
            font-size: 18px;
            font-weight: bold;
            margin: 12px 0;
        }
        .ad-body {
            font-size: 14px;
            margin: 12px 0;
        }
        .ad-cta {
            display: inline-block;
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            text-decoration: none;
            border-radius: 4px;
            text-align: center;
        }
    </style>
</head>
<body>
<div class="ad-container">
    <img src="{{ image }}" alt="Ad Image" class="ad-image">
    <div class="ad-headline">"{{ headline }}"</div>
    <div class="ad-body">"{{ body }}"</div>
    <a href="(https://example.com)" class="ad-cta">"{{ CTA }}"</a>
</div>
</body>
</html>
```

+++
