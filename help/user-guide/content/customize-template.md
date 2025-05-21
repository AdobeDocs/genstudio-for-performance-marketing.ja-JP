---
title: テンプレートのカスタマイズ
description: Adobe GenStudio for Performance Marketing生成 AI で認識されるコンテンツプレースホルダーを使用して、HTML テンプレートをカスタマイズする方法について説明します。
level: Intermediate
role: Developer
feature: Media Templates, Content Generation, Generative AI
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: f6c00f473d561cae123997ab3e310867fbdf60d1
workflow-type: tm+mt
source-wordcount: '1530'
ht-degree: 0%

---

# テンプレートのカスタマイズ

生成 AI がコンテンツの挿入に使用するコンテンツプレースホルダー（フィールド）を挿入することで、GenStudio for Performance Marketingで使用するテンプレートをカスタマイズできます。

以降の節では、_[!DNL Handlebars]_&#x200B;テンプレート言語を使用してHTML テンプレートをGenStudio for Performance Marketingに適応させる方法について説明します。 [!DNL Handlebars] の構文では、コンテンツのプレースホルダーとして中括弧を使用した通常のテキストを使用します。 テンプレートの準備方法については、_ Handlebars 言語ガイド _の [ 概要  [!DNL Handlebars]](https://handlebarsjs.com/guide/#what-is-handlebars) を参照してください。

テンプレートの準備が整ったら、[GenStudio for Performance Marketingにアップロード ](use-templates.md#upload-a-template)、カスタムテンプレートに基づいてパーソナライズされたメールの生成を開始できます。

>[!TIP]
>
>[ アクセシビリティガイドライン ](accessibility-for-templates.md) および [ ベストプラクティス ](/help/user-guide/content/best-practices-for-templates.md) に従って、より多くのオーディエンスにリーチし、最適なエクスペリエンスを提供できるようにします。

## コンテンツプレースホルダー

GenStudio for Performance Marketingはテンプレート内の特定の [ 要素 ](use-templates.md#template-elements) を認識しますが、それは [ 認識されたフィールド名 ](#recognized-field-names) で識別した場合に限られます。

HTML テンプレートの先頭または本文内では、[!DNL Handlebars] の構文を使用して、GenStudio for Performance Marketingに実際のコンテンツをテンプレートに入力させる必要があるコンテンツプレースホルダーを挿入できます。 GenStudio for Performance Marketingは、これらのプレースホルダーを [ 認識された _field_ name](#recognized-field-names) に基づいて認識および解釈します。 各フィールド名は、コンテンツの生成方法とテンプレートへの挿入方法を決定する特定のルールと動作に関連付けられています。

例えば、[!DNL Handlebars] 構文で `{{headline}}` を使用して、メールのヘッドラインを配置する場所を示すことができます。 GenStudioはこのフィールドを認識し、ガイドラインとプロンプトの条件に基づいて関連するヘッドラインを生成して、この場所にヘッドラインを挿入します。

```handlebars
<div>{{headline}}</div>
```

### 認識されたフィールド名

次の表に、テンプレートにプレースホルダーを追加するためにGenStudio for Performance Marketingで認識されるフィールド名を示します。 各フィールドは、特定のチャネルガイドライン、LLM の手順、役割ベースのルールに従います。 GenStudio for Performance Marketingで特定のタイプのコンテンツを生成する必要があるテンプレートに、[!DNL Handlebars] 構文を使用してこれらのフィールド名を追加します。

| フィールド | 役割 | チャネルテンプレート |
| ----------------------- | ------------------------- | ------------------------------------------------ |
| `{{pre_header}}` | プリヘッダー | メール |
| `{{headline}}` | 見出し | メール <br> メタ広告 <br> バナーとディスプレイ広告 <br>LinkedIn 広告 |
| `{{sub_headline}}` | サブ見出し | メールバナ <br> とディスプレイ広告 |
| `{{introductory_text}}` | 紹介テキスト | LinkedIn 広告 |
| `{{body}}` | 本文コピー | メール <br> メタ広告 <br> バナーとディスプレイ広告 |
| `{{cta}}` | Call to action<br>[ コールトゥアクション ](#calls-to-action) を参照 | メール <br> メタ広告 <br> バナーとディスプレイ広告 <br>LinkedIn 広告 |
| `{{image}}` | 画像 – [!DNL Content] から選択 | メール <br> メタ広告 <br> バナーとディスプレイ広告 <br>LinkedIn 広告 |
| `{{on_image_text}}` | 画像テキスト上 <br>[ 画像テキスト上 ](#on-image-text) を参照してください。 | メタ広告 <br>LinkedIn 広告 |
| `{{link}}` | 画像上のコールトゥアクション <br> 画像の [ リンク ](#link-on-image) を参照してください。 | メール |

<!-- | `{{brand_logo}}`        | Logo of selected brand<br>See [Brand logo field name](#brand-logo-field-name). | email<br>Meta ad <br>LinkedIn ad | -->

GenStudio for Performance Marketingでは、特定のフィールドが次のテンプレートで自動的に生成されます。

- **メールテンプレート** で `subject` フィールドを識別する必要はありません
- **メタ広告テンプレート** では、「`headline`」、「`body`」、「`CTA`」フィールドを識別する必要はありません
- **バナーとディスプレイ広告テンプレート** で、`CTA` フィールドを識別する必要はありません
- **LinkedIn 広告テンプレート** では、「`headline`」、「`introductory_text`」、「`CTA`」フィールドを識別する必要はありません

>[!WARNING]
>
>Instagram 広告の場合、生成されたヘッドラインは最終的なエクスペリエンスには表示されません。

テンプレートをGenStudio for Performance Marketingにアップロードできるフィールドは 20 個までです。 メールでは `subject` フィールドが自動的に生成されるので、1 つのフィールドとしてカウントされます。 つまり、メールテンプレートでは 19 個のフィールドを使用できます。

>[!TIP]
>
>GenStudio for Performance Marketingの [ テンプレートプレビュー ](#template-preview) を使用して、テンプレートを検証できます。

### コールトゥアクション

コールトゥアクション（CTA）には、フレーズとリンクが含まれます。 バリアントの生成プロセスで _[!UICONTROL 再フレーズ]_ および _[!UICONTROL リンクを追加]_ の機能が正しく機能するには、テンプレートにリンクとフレーズのプレースホルダーを含める必要があります。

次のガイダンスを使用して、CTAのプレースホルダーを設定します。

- CTAのフレーズ変更が可能で、リンクを編集できます

  ```html
  <a class="button" href="{{pod1_link}}" >{{cta}}</a>
  ```

- CTAのフレーズを変更できますが、実際のリンクはテンプレートで提供されるので、リンクは編集 **できません**

  ```html
  <a align="center" href="https://link">{{cta}}</a>
  ```

- CTA リンクは編集できますが、フレーズはテンプレートで提供されているので、再フレーズは使用 **できません**

  ```html
  <a class="button" href="{{pod1_link}}" >Register now</a>
  ```

GenStudio for Performance Marketingでは、様々なコールトゥアクションフレーズを提供することもできます。 [Call to actionの改訂 ](/help/user-guide/create/manage-variants.md#revise-call-to-action) を参照してください。

### 画像上のリンク

メールテンプレートをカスタマイズして、クリエイティブが画像にリンクを追加できるようにすることができます。 CTA リンクと同様に、次のガイダンスを使用して画像タグに `link` プレースホルダーを適用します。

```html
<a href="{{link}}"><img src="image-source.jpg" alt="{{imageDescription}}"></a>
```

この例では、次のようになります。

- `{{link}}` は、実際の URL のプレースホルダーです。
- `src="image-source.jpg"` は、実際の画像ソース URL に置き換える必要があります。
- `{{imageDescription}}` は、ユーザー定義のフィールド名で、画像の代替テキストのプレースホルダーを提供します。これは、アクセシビリティや SEO に役立ちます。

### 代替テキスト

ユーザー定義のフィールド名をプレースホルダーとして使用して、画像の代替テキスト（HTML `alt="text"` 属性）説明を生成します。 次の `{{imageDescription}}` プレースホルダーは、同じ `<img>` タグ内の `{{image}}` フィールドで使用され、画像とその説明の間の関係が保持されます。

```html
<img src="{{image}}" alt="{{imageDescription}}">
```

この例では、次のようになります。

- `{{image}}` は、画像のソース URL のプレースホルダーです。
- `{{imageDescription}}` は代替テキストのプレースホルダーで、アクセシビリティおよび SEO のために画像の説明が提供されます。

### 画像テキスト上

`{{on_image_text}}` プレースホルダーは、エクスペリエンスの画像に直接配置された、短い影響を受けるメッセージのテキストオーバーレイを指定するために使用されます。

```html
<div class="image-text">{{on_image_text}}</div>
```

<!-- this field does not work in Create canvas 2025/03

### Brand logo field name

At this time, you cannot select the brand logo for the template upload. The following examples demonstrate two methods that conditionally render the brand logo. Each method verifies the source, provides a default or alternative image in case the brand logo is not available, and applies a style:

**Example 1**: Using [!DNL Handlebars] Built-in Helpers condition directly in the HTML `img src` attribute:

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Example 2**: Using [!DNL Handlebars] Built-in condition statement to wrap the HTML `img` tag:

```html
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

-->

### 手動フィールド名

その他のフィールド名はすべてユーザー定義であり、手動で入力されたフィールドとして扱われます。 例えば、フッターコンテンツ用のセクションを予約することができます。

編集可能なセクションを作成するには、セクション名の周りに二重括弧を追加します。

```html
<tbody>
    <tr>
        <td>
            <p><span class="footer-text">{{footerLegal}}</span></p>
        </td>
    </tr>
</tbody>
```

## セクションまたはグループ

フィールドのグループが 2～3 つある場合は、マーケティングメールテンプレートでセクションを使用できます。 _セクション_ このセクションのフィールドには高い一貫性が必要であることをGenStudio for Performance Marketingに伝えます。 この関係を確立すると、AI がセクションのクリエイティブ要素に一致するコンテンツを生成するのに役立ちます。


フィールドがセクションまたはグループの一部であることを示すプレフィックスとして、選択したグループ名を使用します。 アンダースコア（`_`）の後にフィールド名（`headline`、`body`、`image`、`cta` など）を使用します。

構文：`groupname_fieldname`

- _正解_ （👍）:`pod1_body`
- _不正確です_ （❌）: `pod1body`

各セクションは、各フィールドタイプの 1 つのみを使用できます。 例えば、次のフィールドは「`pod1`」セクションに属しています。

- `pod1_headline`
- `pod1_body`
- `pod1_image`
- `pod1_cta`

このルールのため、セクションをネストすることはできません。

メールやメタ広告などの各テンプレートタイプには、セクションの使用に関するチャネル固有の制約があります。 [ テンプレート使用のベストプラクティス ](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/best-practices-for-templates#follow-channel-specific-template-guidelines) トピックの _チャネル固有のガイドライン_ を参照してください。

例えば、1 つのメールテンプレートに最大 3 つのセクションを含めることができます。したがって、次の 3 つのヘッドラインと本文セクションを含めることができます。

- `pre_header`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`
- `pod3_headline`
- `pod3_body`
- `cta`

GenStudio for Performance Marketingは `pod1_headline` が `pod2_body` よりも `pod1_body` と密接に関係していることを理解しています。

>[!TIP]
>
>複数セクションのメールの各セクションに対して様々なコンテンツを生成するプロンプトを作成する方法については、[ 構造化プロンプト ](/help/user-guide/effective-prompts.md#structured-prompts) を参照してください。

## テンプレートのプレビュー

[ テンプレートをアップロード ](use-templates.md#upload-a-template) すると、GenStudio for Performance MarketingはHTML ファイルをスキャンして、認識されたフィールドを探します。 プレビューを使用して [ テンプレート要素 ](use-templates.md#template-elements) を確認し、それらが [ 認識されたフィールド名 ](#recognized-field-names) で正しく識別されたことを確認します。

メールテンプレートのプレビューの例：

![ 検出されたプレビューフィールド ](/help/assets/template-detected-fields.png " 検出されたフィールドを確認 "){zoomable="yes"}

[ テンプレートコードエディター ](/help/user-guide/content/code-editor.md) を参照してください。

### プレビューを制御

組み込みヘルパー（特定のアクションを実行する [!DNL Handlebars] テンプレート言語の特別な式）を使用して、特別なコンテンツの表示を制御できます。 例えば、プレビューリンクをクリーンに保ちながら、書き出されたテンプレート内のリンクにトラッキングパラメーターを追加する条件ステートメントを追加できます。

テンプレートのレンダリング時には `_genStudio.browser` の値が設定され、テンプレートの書き出し時には `genStudio.export` の値が設定されます。 条件付きラッパーを使用して、メールの上部に特定のコンテンツを含めることもできます。例えば、テンプレートを書き出しに使用する場合です。

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

もう 1 つの例として、GenStudio for Performance Marketingでテンプレートをプレビューする際に、トラッキングコードを使用しないようにすることがあります。 次の例では、プレビューリンクをクリーンな状態に保ちながら、書き出されたテンプレート内のリンクにトラッキングパラメーターを追加する方法を示します。

```html
<a class="button" {{#if _genStudio.browser }}
   href="{{link}}"{{/if}}{{#if _genStudio.export }}
   href="{{link}}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{cta}}</a>
```

## 静的コンテンツ

多くの場合、メールおよびメタテンプレートは、他のドメインでホストされている画像や CSS ファイルにリンクしています。 GenStudio for Performance Marketingは、テンプレートプレビューまたはそれらから派生したエクスペリエンスのサムネールを生成する際に、コンテンツソースを検証し、プレビュー目的でコピーを埋め込みます。

外部ファイルは、テンプレートプレビューを作成する目的でのみ一時的に埋め込まれます。これにより、プレビューで作成時に表示されるコンテンツが正確に反映されます。 これらの外部ファイルは、GenStudio for Performance Marketingに永続的に保存 **されません**。 テンプレートのプレビューが作成された後、GenStudio for Performance Marketingは引き続き、テンプレートで提供された元のソースリンクを参照します。

### コンテンツを更新

最初のプレビューの作成後にソースが変更された場合は、[refresh](/help/user-guide/content/use-templates.md#refresh-template) 関数を使用して、外部ソースからのコンテンツの最新バージョンでテンプレートプレビューを更新できます。

## テンプレートの例

+++例：1 つのセクションを持つメールテンプレート

以下は、1 つのセクションを含むメールのHTML テンプレートの基本的な例です。 ヘッドには、スタイル設定用のシンプルなインライン CSS が含まれています。 本文には、`pre_header`、`headline`、`image` [ プレースホルダー ](#content-placeholders) が含まれており、メール生成プロセス中にGenStudio for Performance Marketingでコンテンツを挿入するために使用されます。

```html {line-numbers="true" highlight="13"}
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
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p><a href="{{link}}">
            <img alt="{{headline}}"
                    src="{{image}}"
                    width="600" height="600"
                    border="0"/></a></p>
            <p>{{body}}</p>
        </div>
    </body>
</html>
```

+++

+++例：複数のセクションを持つメールテンプレート

以下は、上記の例と同じHTML テンプレートですが、さらに 2 つのセクションがあります。 ヘッドには、グループのスタイル設定に使用するインライン CSS が含まれています。 本文では、プレフィックスを使用して、[ コンテンツプレースホルダー ](#content-placeholders) を含む 2 つのグループを使用します。

```html
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
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p>{{body}}</p>
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="{{ headline }}" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="{{headline}}" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
        </div>
    </body>
</html>
```

+++

+++例：メタ広告テンプレート

次に、メタ広告テンプレートの基本的な例を示します。 ヘッドには、スタイル設定用のインライン CSS が含まれています。 本文では、`image` や `on_image_text` などの [ コンテンツプレースホルダー ](#content-placeholders) を使用して、GenStudio for Performance Marketingでコンテンツを生成できる場所を示します。

```html {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Adobe</title>
        <style>
            .ad-container {
            font-family: Helvetica, sans-serif;
            position: relative;
            text-align: center;
            height: 100%;
            }
            .ad-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            }
            .ad-text {
            position: absolute;
            top: 0;
            left: 0;
            margin: 1em;
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            padding: 1em;
            font-size: 75px;
            }
        </style>
    </head>
    <body>
        <div class="ad-container">
            <img src="{{image}}" alt="Ad Image" class="ad-image" />
            <div class="ad-text">{{on_image_text}}</div>
        </div>
    </body>
</html>
```

+++
