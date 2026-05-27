---
title: テンプレートのカスタマイズ
description: Adobe GenStudio for Performance Marketingの生成AIで認識されたコンテンツプレースホルダーを使用して、HTML テンプレートをカスタマイズする方法について説明します。
level: Intermediate
role: Developer
feature: Media Templates, Content Generation, Generative AI
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
TQID: https://experienceleague.adobe.com/6gHxPvfz-30X3w2MYIc2Aj5SiGZokzOqSvOHYTQ-u7I
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2: id: be495d08-ecd1-455f-951e-c22de504e667id: f54ee13b-9545-4d68-9842-a12026e60aaf
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
source-git-commit: e8e0898054576454bad9ecdbd1a48b17f955e138
workflow-type: tm+mt
source-wordcount: 1646
ht-degree: 0%

---

# テンプレートのカスタマイズ

GenStudio for Performance Marketingで使用するテンプレートをカスタマイズするには、生成AIがコンテンツの挿入に使用するコンテンツプレースホルダー（フィールド）を挿入します。

次のいくつかのセクションでは、_[!DNL Handlebars]_テンプレート言語を使用してGenStudio for Performance Marketing用にHTML テンプレートを適応させる方法について説明します。 [!DNL Handlebars]構文では、コンテンツのプレースホルダーとして、二重中括弧を含む通常のテキストが使用されます。 テンプレートの準備方法については、_ Handlebars言語ガイド _の[What is [!DNL Handlebars]](https://handlebarsjs.com/guide/#what-is-handlebars)を参照してください。

テンプレートの準備が整ったら、[GenStudio for Performance Marketing](use-templates.md#upload-a-template)にアップロードし、カスタムテンプレートに基づいてパーソナライズされたメールの作成を開始できます。

[ アクセシビリティガイドライン ](accessibility-for-templates.md)と[ ベストプラクティス ](/help/user-guide/templates/best-practices-for-templates.md)に従って、より多くのオーディエンスにリーチし、最適なエクスペリエンスを提供してください。

## コンテンツのプレースホルダー

>[!TIP]
>
>コンテンツのプレースホルダーは、後でユーザーが入力するコンテンツのプレースホルダーテキストと&#x200B;**not**&#x200B;同じです。 テンプレート ](/help/user-guide/templates/best-practices-for-templates.md#using-placeholder-text-in-templates)でのプレースホルダーテキストの使用について詳しくは、[を参照してください。

GenStudio for Performance Marketingは、テンプレート内の特定の種類のコンテンツまたは[要素](use-templates.md#template-elements)を認識しますが、[認識されたフィールド名](#recognized-field-names)で特定する場合に限ります。

HTML テンプレートの先頭または本文では、[!DNL Handlebars]構文を使用して、GenStudio for Performance Marketingに実際のコンテンツを入力させるように求めるコンテンツプレースホルダーを挿入できます。 GenStudio for Performance Marketingは、認識された[ フィールド _名](#recognized-field-names)に基づいて、これらのプレースホルダーを認識および解釈します。_&#x200B;各フィールド名は、コンテンツを生成してテンプレートに挿入する方法を決定する、特定のルールと動作に関連付けられます。

例えば、`{{headline}}`と[!DNL Handlebars]構文を使用して、メールの見出しを配置する場所を示すことができます。 GenStudioはこのフィールドを認識し、ガイドラインとプロンプトの基準に基づいて関連する見出しを生成し、見出しを次の場所に挿入します。

```handlebars
<div>{{headline}}</div>
```

### 認識されるフィールド名

次の表は、テンプレートにプレースホルダーを追加するためにGenStudio for Performance Marketingで認識されるフィールド名を示しています。 各フィールドは、特定のチャネルガイドライン、LLM手順、ロールベースのルールに従います。 特定の種類のコンテンツを生成するためにGenStudio for Performance Marketingが必要なテンプレートに、[!DNL Handlebars]構文を使用してこれらのフィールド名を追加します。

| フィールド | 役割 | チャネルテンプレート |
| ----------------------- | ------------------------- | ------------------------------------------------ |
| `{{pre_header}}` | プリヘッダー | メール |
| `{{headline}}` | Headline | メール <br>Meta広告<br> バナーとディスプレイ広告<br>LinkedIn広告 |
| `{{sub_headline}}` | Sub-Headline | email<br> バナーとディスプレイ広告 |
| `{{introductory_text}}` | 概要テキスト | LinkedIn広告 |
| `{{body}}` | 本文 | メール <br>Meta広告<br> バナーとディスプレイ広告 |
| `{{cta}}` | Call to action<br>[行動喚起](#calls-to-action)を参照 | メール <br>Meta広告<br> バナーとディスプレイ広告<br>LinkedIn広告 |
| `{{image}}` | 画像 – [!DNL Content]から選択 | メール <br>Meta広告<br> バナーとディスプレイ広告<br>LinkedIn広告 |
| `{{on_image_text}}` | 画像テキスト <br>画像テキスト ](#on-image-text)の[を参照してください。 | Meta広告<br>LinkedIn広告 |
| `{{link}}` | Call to actionの画像<br>画像の[ リンク ](#link-on-image)を参照してください。 | メール |

<!-- | `{{brand_logo}}`        | Logo of selected brand<br>See [Brand logo field name](#brand-logo-field-name). | email<br>Meta ad <br>LinkedIn ad | -->

GenStudio for Performance Marketingでは、次のテンプレートで特定のフィールドが自動的に生成されます。

- **電子メールテンプレート**&#x200B;では、`subject` フィールドを識別する必要はありません
- **Meta広告テンプレート**&#x200B;では、`headline`、`body`、`CTA`のフィールドを特定する必要はありません
- **バナーとディスプレイ広告テンプレート**&#x200B;では、`CTA` フィールドを識別する必要はありません
- **LinkedIn広告テンプレート**&#x200B;では、`headline`、`introductory_text`、`CTA`のフィールドを識別する必要はありません

>[!WARNING]
>
>Instagram広告の場合、生成された見出しは最終的なエクスペリエンスに表示されません。

テンプレートをGenStudio for Performance Marketingにアップロードする場合、フィールドの数は20件までという制限があります。 `subject` フィールドはメールで自動的に生成されるので、1つのフィールドとしてカウントされます。 つまり、メールテンプレートには19のフィールドを使用できます。

>[!TIP]
>
>GenStudio for Performance Marketingの[ テンプレートのプレビュー](#template-preview)を使用して、テンプレートを確認できます。

### CTA

Call to action（CTA）には、フレーズとリンクが含まれます。 バリエーション生成プロセス中に&#x200B;_[!UICONTROL 言い換え]_&#x200B;および&#x200B;_[!UICONTROL リンクを追加]_&#x200B;機能が適切に機能するには、リンクとフレーズのプレースホルダーをテンプレートに含める必要があります。

次のガイダンスを使用して、CTAのプレースホルダーを設定します。

- CTAの言い換えが使用可能で、リンクは編集可能です

  ```html
  <a class="button" href="{{pod1_link}}" >{{cta}}</a>
  ```

- CTAの言い換えは使用できますが、実際のリンクがテンプレートに指定されているため、リンクは&#x200B;**編集可能ではありません**

  ```html
  <a align="center" href="https://link">{{cta}}</a>
  ```

- CTA リンクは編集可能ですが、テンプレートにフレーズが指定されているため、リフレーズは&#x200B;**利用できません**

  ```html
  <a class="button" href="{{pod1_link}}" >Register now</a>
  ```

GenStudio for Performance Marketingでは、CTA フレーズのバリエーションを提供することもできます。 [Call to actionの修正](/help/user-guide/create/manage-variants.md#revise-call-to-action)を参照してください。

### 画像上のリンク

メールテンプレートをカスタマイズして、クリエイターが画像にリンクを追加できるようにすることができます。 CTA リンクと同様に、次のガイダンスを使用して`link` プレースホルダーを画像タグに適用します。

```html
<a href="{{link}}"><img src="image-source.jpg" alt="{{imageDescription}}"></a>
```

この例では、次のようになります。

- `{{link}}`は、実際のURLのプレースホルダーです。
- `src="image-source.jpg"`は、実際の画像ソース URLに置き換える必要があります。
- `{{imageDescription}}`は、画像の代替テキストのプレースホルダーを提供するユーザー定義のフィールド名です。アクセシビリティとSEOに役立ちます。

### 代替テキスト

ユーザー定義のフィールド名をプレースホルダーとして使用して、画像の代替テキスト（HTML `alt="text"`属性）説明を生成します。 次の`{{imageDescription}}` プレースホルダーは、同じ`<img>` タグ内の`{{image}}` フィールドで使用され、画像とその説明の関係が維持されます。

```html
<img src="{{image}}" alt="{{imageDescription}}">
```

この例では、次のようになります。

- `{{image}}`は、画像ソース URLのプレースホルダーです。
- `{{imageDescription}}`は、アクセシビリティとSEOの目的で画像の説明を提供する代替テキストのプレースホルダーです。

### アクセシビリティラベル

`aria-label`属性は、表示ラベルを持たない要素にアクセス可能な名前を定義するために使用されます。 この属性は、CTA ボタンなど、インタラクティブな要素のコンテキストを提供することが重要なテンプレートで特に便利です。

```html
<a class="button" href="{{link}}" aria-label="{{CTAAriaLabel}}">{{cta}}</a>
```

### 画像テキスト上

`{{on_image_text}}` プレースホルダーは、エクスペリエンスの画像に直接配置された、短いインパクトのあるメッセージのテキストオーバーレイを指定するために使用されます。

```html
<div class="image-text">{{on_image_text}}</div>
```

<!-- 
this field does not work in Create canvas 2025/03

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

その他のすべてのフィールド名はユーザー定義であり、手作業で入力されたフィールドとして扱われます。 例えば、フッターコンテンツ用のセクションを予約することができます。

編集可能なセクションを作成するには、セクション名の周りに二重角括弧を追加します。

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

リッチテキスト編集を使用して、[!DNL Create] プロセス中にクリエイティブコンテンツを強化します。 キャンバスは、コンテンツプレースホルダーの場所に基づいてリッチテキスト機能を決定します。 リッチテキスト機能は、コンテンツプレースホルダーをスタンドアロン要素として使用する場合、または`<p>`、`<div>`、`<span>`などのブロックレベルのHTML タグ内で使用する場合にのみ使用できます。

リッチテキスト編集は、段落内の独立したコンテンツで使用できます。

```html
<p>{{body}}</p>
```

HTML属性内のコンテンツプレースホルダー（`alt`、`href`、`src`など）を使用する場合、そのフィールドではリッチテキスト編集はサポートされていません。

リッチテキスト編集は、`alt` コンテンツで利用できる&#x200B;**not**&#x200B;です：

```html
<img src="image.jpg" alt="{{image_description}}">
```

フィールドが複数表示される場合、リッチテキスト機能は、いずれかのインスタンスでHTML属性として使用されているかどうかに基づいて決定されます。 例えば、見出しを見出しとして使用し、画像の代替テキストとして使用する場合、`alt` タグが優先されます。

リッチテキスト編集は`alt` コンテンツとして使用されているため、`headline`では&#x200B;**not**&#x200B;利用できます。

```html
<h1>{{headline}}</h1>
<img src="image.jpg" alt="{{headline}}">
```

リッチテキスト編集は、ソーシャルチャネル（Meta、LinkedIn）の`on_image_text`など、特定のチャネル内の特定のフィールドで使用できます。

## セクションまたはグループ

メールテンプレートに複数のオファーやストーリーなどの複数のコンテンツ領域が必要な場合は、セクションやグループを使用してこれらを整理できます。 _セクション_&#x200B;は、このセクションのフィールドに高度な一貫性が必要であることをGenStudio for Performance Marketingに通知します。 この関係を確立することで、AIがセクションのクリエイティブ要素に一致するコンテンツを生成できるようになります。

フィールドがセクションまたはグループの一部であることを示す接頭辞として、任意のグループ名を使用します。 アンダースコア（`_`）の後にフィールド名（`headline`、`body`、`image`、または`cta`など）を使用します。

構文：`groupname_fieldname`

- _正解_ （👍）: `pod1_body`
- _正しくない_ （❌）: `pod1body`

各セクションで使用できるフィールドタイプは1つだけです。 例えば、次のフィールドは`pod1` セクションに属しています。

- `pod1_headline`
- `pod1_body`
- `pod1_image`
- `pod1_cta`

このルールにより、セクションはネストできません。

メールやMeta広告などの各テンプレートタイプには、セクションの使用に関するチャネル固有の制約があります。 _テンプレートの使用に関するベストプラクティス_&#x200B;のトピックの[ チャネル固有のガイドライン ](/help/user-guide/templates/best-practices-for-templates.md)を参照してください。

たとえば、メールテンプレートには最大3つのセクションを含めることができます。したがって、見出しと本文のセクションを3つ含めることができます。

- `pre_header`
- `pod1_headline`, `pod1_body`
- `pod2_headline`, `pod2_body`
- `pod3_headline`, `pod3_body`
- `cta`

GenStudio for Performance Marketingは、`pod1_headline`が`pod2_body`よりも`pod1_body`に近いことを理解しています。

>[!TIP]
>
>複数セクションのメールの各セクションに対して様々なコンテンツを生成するプロンプトを作成する方法については、[構造化プロンプト ](/help/user-guide/effective-prompts.md#structured-prompts)を参照してください。

## テンプレートプレビュー

テンプレート ](use-templates.md#upload-a-template)を[ アップロードすると、GenStudio for Performance MarketingはHTML ファイルをスキャンして、認識されたフィールドを探します。 プレビューを使用して[ テンプレート要素](use-templates.md#template-elements)を確認し、[認識済みのフィールド名](#recognized-field-names)で正しく識別されていることを確認します。

メールテンプレートのプレビューの例：

![ プレビューフィールドが検出されました](/help/assets/template-detected-fields.png "検出されたフィールドを確認してください"){zoomable="yes"}

[ テンプレート コード エディター](/help/user-guide/templates/code-editor.md)を参照してください。

### プレビューを制御

組み込みヘルパー（特定のアクションを実行する[!DNL Handlebars] テンプレート言語の特殊表現）を使用して、特殊コンテンツの表示を制御できます。 例えば、プレビューリンクをクリーンに保ちながら、書き出されたテンプレート内のリンクにトラッキングパラメーターを追加する条件付きステートメントを追加できます。

テンプレートのレンダリング時には`_genStudio.canvas`値が設定され、テンプレートのエクスポート時には`genStudio.export`値が設定されます。 コンディショナルラッパーを使用して、メールの上部に特定のコンテンツを含めることができます。例えば、テンプレートを書き出しに使用する場合は、次のようになります。

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

別の例として、GenStudio for Performance Marketingでテンプレートをプレビューする際にトラッキングコードが使用されないようにすることができます。 次の例は、プレビューリンクをクリーンに保ちながら、書き出されたテンプレート内のリンクにトラッキングパラメーターを追加する方法を示しています。

```html
<a class="button" {{#if _genStudio.canvas }}
   href="{{link}}"{{/if}}{{#if _genStudio.export }}
   href="{{link}}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{cta}}</a>
```

## 静的コンテンツ

電子メールやMetaのテンプレートは、多くの場合、他のドメインでホストされている画像やCSS ファイルにリンクします。 GenStudio for Performance Marketingは、テンプレートのプレビューまたはそこから派生したエクスペリエンスのサムネールを生成すると、コンテンツソースを検証し、プレビュー用にコピーを埋め込みます。

外部ファイルは、テンプレートのプレビューを作成する目的でのみ一時的に埋め込まれます。これにより、プレビューは作成時に表示されるコンテンツを正確に反映します。 これらの外部ファイルは、GenStudio for Performance Marketingに完全に保存されている&#x200B;**not**&#x200B;です。 テンプレートのプレビューを作成した後も、GenStudio for Performance Marketingは引き続きテンプレートで提供された元のソースリンクを参照します。

### コンテンツを更新

最初のプレビューの作成後にソースが変更された場合は、[refresh](/help/user-guide/templates/use-templates.md#refresh-template)関数を使用して、外部ソースのコンテンツの最新バージョンでテンプレートプレビューを更新します。
