---
title: テンプレートのカスタマイズ
description: Adobe GenStudio for Performance Marketing生成 AI で認識されるコンテンツプレースホルダーを使用して、HTML テンプレートをカスタマイズする方法について説明します。
level: Intermediate
role: Developer
feature: Media Templates, Content Generation, Generative AI
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: 9f4cfd470590b2971c615a6437e6ae730cde5c18
workflow-type: tm+mt
source-wordcount: '1633'
ht-degree: 0%

---

# テンプレートのカスタマイズ

生成 AI がコンテンツの挿入に使用するコンテンツプレースホルダー（フィールド）を挿入することで、GenStudio for Performance Marketingで使用するテンプレートをカスタマイズできます。

以降の節では、_[!DNL Handlebars]_テンプレート言語を使用してHTML テンプレートをGenStudio for Performance Marketingに適応させる方法について説明します。 [!DNL Handlebars] の構文では、コンテンツのプレースホルダーとして中括弧を使用した通常のテキストを使用します。 テンプレートの準備方法については、[Handlebars 言語ガイド  [!DNL Handlebars] の ](https://handlebarsjs.com/guide/#what-is-handlebars) 概要__を参照してください。

テンプレートの準備が整ったら、[GenStudio for Performance Marketingにアップロード ](use-templates.md#upload-a-template)、カスタムテンプレートに基づいてパーソナライズされたメールの生成を開始できます。

[ アクセシビリティガイドライン ](accessibility-for-templates.md) および [ ベストプラクティス ](/help/user-guide/templates/best-practices-for-templates.md) に従って、より多くのオーディエンスにリーチし、最適なエクスペリエンスを提供できるようにします。

## コンテンツプレースホルダー

>[!TIP]
>
>コンテンツのプレースホルダーは **ユーザーが後で入力するコンテンツ内のプレースホルダーテキストと同じではありま** ん。 詳しくは、[ テンプレートでのプレースホルダーテキストの使用 ](/help/user-guide/templates/best-practices-for-templates.md#using-placeholder-text-in-templates) を参照してください。

GenStudio for Performance Marketingは、テンプレート内の特定の種類のコンテンツや [ 要素 ](use-templates.md#template-elements) を認識しますが、それは [ 認識されたフィールド名 ](#recognized-field-names) で識別した場合に限られます。

HTML テンプレートの先頭または本文内では、[!DNL Handlebars] の構文を使用して、GenStudio for Performance Marketingに実際のコンテンツをテンプレートに入力させる必要があるコンテンツプレースホルダーを挿入できます。 GenStudio for Performance Marketingは、これらのプレースホルダーを [ 認識された _field_ name](#recognized-field-names) に基づいて認識および解釈します。 各フィールド名は、コンテンツの生成方法とテンプレートへの挿入方法を決定する特定のルールと動作に関連付けられています。

例えば、`{{headline}}` 構文で [!DNL Handlebars] を使用して、メールのヘッドラインを配置する場所を示すことができます。 GenStudioはこのフィールドを認識し、ガイドラインとプロンプトの条件に基づいて関連するヘッドラインを生成して、この場所にヘッドラインを挿入します。

```handlebars
<div>{{headline}}</div>
```

### 認識されたフィールド名

次の表に、テンプレートにプレースホルダーを追加するためにGenStudio for Performance Marketingで認識されるフィールド名を示します。 各フィールドは、特定のチャネルガイドライン、LLM の手順、役割ベースのルールに従います。 GenStudio for Performance Marketingで特定のタイプのコンテンツを生成する必要があるテンプレートに、[!DNL Handlebars] 構文を使用してこれらのフィールド名を追加します。

| フィールド | 役割 | チャネルテンプレート |
| ----------------------- | ------------------------- | ------------------------------------------------ |
| `{{pre_header}}` | プリヘッダー | メール |
| `{{headline}}` | 見出し | メール <br>Meta広告 <br> バナーとディスプレイ広告 <br>LinkedIn 広告 |
| `{{sub_headline}}` | サブ見出し | メールバナ <br> とディスプレイ広告 |
| `{{introductory_text}}` | 紹介テキスト | LinkedIn 広告 |
| `{{body}}` | 本文コピー | <br>Meta広告 <br> バナーおよびディスプレイ広告をメールで送信 |
| `{{cta}}` | Call to action<br>[ コールトゥアクション ](#calls-to-action) を参照 | メール <br>Meta広告 <br> バナーとディスプレイ広告 <br>LinkedIn 広告 |
| `{{image}}` | 画像 – [!DNL Content] から選択 | メール <br>Meta広告 <br> バナーとディスプレイ広告 <br>LinkedIn 広告 |
| `{{on_image_text}}` | 画像テキスト上 <br>[ 画像テキスト上 ](#on-image-text) を参照してください。 | Meta広告 <br>LinkedIn 広告 |
| `{{link}}` | 画像のCall to action<br> 画像のリンク [ を参照してください ](#link-on-image)。 | メール |

<!-- | `{{brand_logo}}`        | Logo of selected brand<br>See [Brand logo field name](#brand-logo-field-name). | email<br>Meta ad <br>LinkedIn ad | -->

GenStudio for Performance Marketingでは、特定のフィールドが次のテンプレートで自動的に生成されます。

- **メールテンプレート** では、`subject` フィールドを識別する必要はありません
- **Meta広告テンプレート** では、`headline`、`body`、`CTA` の各フィールドを特定する必要はありません
- **バナーとディスプレイ広告テンプレート** では、`CTA` フィールドを識別する必要はありません
- **LinkedIn 広告テンプレート** では、「`headline`」、「`introductory_text`」、「`CTA`」フィールドを識別する必要はありません

>[!WARNING]
>
>Instagram 広告の場合、生成されたヘッドラインは最終的なエクスペリエンスには表示されません。

テンプレートをGenStudio for Performance Marketingにアップロードできるフィールドは 20 個までです。 メールでは `subject` フィールドが自動的に生成されるので、1 つのフィールドとしてカウントされます。 つまり、メールテンプレートでは 19 個のフィールドを使用できます。

>[!TIP]
>
>GenStudio for Performance Marketingの [ テンプレートプレビュー ](#template-preview) を使用して、テンプレートを検証できます。

### コールトゥアクション

call to action（CTA）には、フレーズとリンクが含まれます。 バリアントの生成プロセスで _[!UICONTROL 再フレーズ]_ および _[!UICONTROL リンクを追加]_ の機能が正しく機能するには、テンプレートにリンクとフレーズのプレースホルダーを含める必要があります。

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

ユーザー定義のフィールド名をプレースホルダーとして使用して、画像の代替テキスト（HTML `alt="text"` 属性）説明を生成します。 次の `{{imageDescription}}` プレースホルダーは、同じ `{{image}}` タグ内の `<img>` フィールドで使用され、画像とその説明の間の関係が保持されます。

```html
<img src="{{image}}" alt="{{imageDescription}}">
```

この例では、次のようになります。

- `{{image}}` は、画像のソース URL のプレースホルダーです。
- `{{imageDescription}}` は代替テキストのプレースホルダーで、アクセシビリティおよび SEO のために画像の説明が提供されます。

### アクセシビリティラベル

`aria-label` 属性は、表示ラベルのない要素に対して、アクセス可能な名前を定義するために使用されます。 この属性は、CTA ボタンなどのインタラクティブ要素のコンテキストを提供することが重要なテンプレートで特に役立ちます。

```html
<a class="button" href="{{link}}" aria-label="{{CTAAriaLabel}}">{{cta}}</a>
```

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

### リッチテキスト編集

リッチテキスト編集を使用して、リッ [!DNL Create] プロセス中にクリエイティブコンテンツを強化します。 キャンバスは、コンテンツプレースホルダーの場所に基づいてリッチテキスト機能を決定します。 リッチテキスト機能は、コンテンツプレースホルダーをスタンドアロン要素として使用するか、ブロックレベルのHTML タグ（`<p>`、`<div>`、`<span>` など）内で使用する場合にのみ使用できます。

段落内のスタンドアロンコンテンツに対して、リッチテキスト編集を使用できます。

```html
<p>{{body}}</p>
```

HTML属性内でコンテンツプレースホルダー（`alt`、`href`、`src` など）を使用する場合、そのフィールドではリッチテキストの編集はサポートされません。

**のコンテンツではリッチテキスト編集は使用** できません `alt`

```html
<img src="image.jpg" alt="{{image_description}}">
```

1 つのフィールドが複数回表示される場合、リッチテキスト機能は、いずれかのインスタンスでHTML属性として使用されているかどうかに基づいて決定されます。 例えば、ヘッドラインが見出しとして、また画像の代替テキストとして使用される場合、`alt` タグが優先されます。

リッチテキスト編集は、リッ **コンテンツとして使用されるので、** では使用 `headline` できません `alt`。

```html
<h1>{{headline}}</h1>
<img src="image.jpg" alt="{{headline}}">
```

リッチテキスト編集は、ソーシャルチャネル（Meta、LinkedIn）の `on_image_text` など、特定のチャネル内の特定のフィールドで使用できます。

## セクションまたはグループ

メールテンプレートに複数のコンテンツ領域（複数のオファーやストーリーなど）が必要な場合は、セクションやグループを使用して整理できます。 _セクション_ このセクションのフィールドには高い一貫性が必要であることをGenStudio for Performance Marketingに伝えます。 この関係を確立すると、AI がセクションのクリエイティブ要素に一致するコンテンツを生成するのに役立ちます。

フィールドがセクションまたはグループの一部であることを示すプレフィックスとして、選択したグループ名を使用します。 アンダースコア（`headline`）の後にフィールド名（`body`、`image`、`cta`、`_` など）を使用します。

構文：`groupname_fieldname`

- _正解_ （👍）:`pod1_body`
- _不正確です_ （❌）: `pod1body`

各セクションは、各フィールドタイプの 1 つのみを使用できます。 例えば、次のフィールドは「`pod1`」セクションに属しています。

- `pod1_headline`
- `pod1_body`
- `pod1_image`
- `pod1_cta`

このルールのため、セクションをネストすることはできません。

メールやMeta広告などの各テンプレートタイプには、セクションの使用に関するチャネル固有の制約があります。 [ テンプレート使用のベストプラクティス ](/help/user-guide/templates/best-practices-for-templates.md) トピックの _チャネル固有のガイドライン_ を参照してください。

例えば、1 つのメールテンプレートに最大 3 つのセクションを含めることができます。したがって、次の 3 つのヘッドラインと本文セクションを含めることができます。

- `pre_header`
- `pod1_headline`、`pod1_body`
- `pod2_headline`、`pod2_body`
- `pod3_headline`、`pod3_body`
- `cta`

GenStudio for Performance Marketingは `pod1_headline` が `pod1_body` よりも `pod2_body` と密接に関係していることを理解しています。

>[!TIP]
>
>複数セクションのメールの各セクションに対して様々なコンテンツを生成するプロンプトを作成する方法については、[ 構造化プロンプト ](/help/user-guide/effective-prompts.md#structured-prompts) を参照してください。

## テンプレートのプレビュー

[ テンプレートをアップロード ](use-templates.md#upload-a-template) すると、GenStudio for Performance MarketingはHTML ファイルをスキャンして、認識されたフィールドを探します。 プレビューを使用して [ テンプレート要素 ](use-templates.md#template-elements) を確認し、それらが [ 認識されたフィールド名 ](#recognized-field-names) で正しく識別されたことを確認します。

メールテンプレートのプレビューの例：

![ 検出されたプレビューフィールド ](/help/assets/template-detected-fields.png " 検出されたフィールドを確認 "){zoomable="yes"}

[ テンプレートコードエディター ](/help/user-guide/templates/code-editor.md) を参照してください。

### プレビューを制御

組み込みヘルパー（特定のアクションを実行する [!DNL Handlebars] テンプレート言語の特別な式）を使用して、特別なコンテンツの表示を制御できます。 例えば、プレビューリンクをクリーンに保ちながら、書き出されたテンプレート内のリンクにトラッキングパラメーターを追加する条件ステートメントを追加できます。

テンプレートのレンダリング時には `_genStudio.canvas` の値が設定され、テンプレートの書き出し時には `genStudio.export` の値が設定されます。 条件付きラッパーを使用して、メールの上部に特定のコンテンツを含めることもできます。例えば、テンプレートを書き出しに使用する場合です。

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

もう 1 つの例として、GenStudio for Performance Marketingでテンプレートをプレビューする際に、トラッキングコードを使用しないようにすることがあります。 次の例では、プレビューリンクをクリーンな状態に保ちながら、書き出されたテンプレート内のリンクにトラッキングパラメーターを追加する方法を示します。

```html
<a class="button" {{#if _genStudio.canvas }}
   href="{{link}}"{{/if}}{{#if _genStudio.export }}
   href="{{link}}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{cta}}</a>
```

## 静的コンテンツ

多くの場合、メールおよびMetaのテンプレートは、他のドメインでホストされている画像や CSS ファイルにリンクされています。 GenStudio for Performance Marketingは、テンプレートプレビューまたはそれらから派生したエクスペリエンスのサムネールを生成する際に、コンテンツソースを検証し、プレビュー目的でコピーを埋め込みます。

外部ファイルは、テンプレートプレビューを作成する目的でのみ一時的に埋め込まれます。これにより、プレビューで作成時に表示されるコンテンツが正確に反映されます。 これらの外部ファイルは、GenStudio for Performance Marketingに永続的に保存 **されません**。 テンプレートのプレビューが作成された後、GenStudio for Performance Marketingは引き続き、テンプレートで提供された元のソースリンクを参照します。

### コンテンツを更新

最初のプレビューの作成後にソースが変更された場合は、[refresh](/help/user-guide/templates/use-templates.md#refresh-template) 関数を使用して、外部ソースからのコンテンツの最新バージョンでテンプレートプレビューを更新できます。
