---
title: メールテンプレートガイドライン
description: Adobe GenStudio for Performance Marketingでメールテンプレートを使用する場合は、ベストプラクティスに従ってください。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
TQID: https://experienceleague.adobe.com/v8DZ2ubNwArTNws12FxsJKNbGbsRB-f0IJk39Y3PgXU
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 445
ht-degree: 0%

---

# メールテンプレートガイドライン

マーケティングメールテンプレートは、視覚的に魅力的でレスポンシブなメール施策を展開するための基盤となります。 一般的に、HTMLのテンプレートでは、ブランドガイドラインに合わせてレイアウト、タイポグラフィ、カラー、画像を調整できます。 GenStudio for Performance Marketingで使用するテンプレートを準備する際には、セマンティック HTMLとインライン CSSを使用してスタイル設定を行い、スクリプトや外部の依存関係を避けます。 適切に構造化されたHTMLテンプレートは、受信者の体験を向上させ、配信品質とエンゲージメント率を向上させることができます。

GenStudio for Performance Marketingを使用してメールテンプレートをカスタマイズする場合は、次のデザインのベストプラクティスに従ってください。

- Adobe フォントまたはGoogle フォントの使用
- クリーンでレスポンシブなHTMLとインライン CSSの使用
- JavaScriptを&#x200B;**使用しない**&#x200B;人
- **not**&#x200B;は、本文またはコンテナで固定幅を使用しないでください
- テンプレートのサイズを大幅に増やすことができるため、**not**&#x200B;は画像にbase64 エンコーディングを使用しないでください
- HTMLの最大ファイルサイズは102 KBです

## 認識されるフィールド名

メールテンプレートをカスタマイズする際には、次の必須フィールドにコンテンツプレースホルダーを使用します。

- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` （Content JPEG、PNGまたはGIFから選択）

GenStudio for Performance Marketingは、次のフィールドを自動生成します。 リッチテキストが有効になっていません。 次の場合、コンテンツプレースホルダーを適用する必要はありません。

- `pre_header`
- `subject`

テンプレートで許可される最大フィールドは20です。 テンプレートでのフィールド名の使用について詳しくは、[&#x200B; コンテンツプレースホルダー](/help/user-guide/templates/customize-template.md#content-placeholders)を参照してください。

## マルチセクションメール

_セクション_&#x200B;を使用すると、コンテンツを個別のグループに整理し、より複雑なレイアウトをサポートできます。 GenStudio for Performance Marketingでは、グループ命名規則を使用して各セクションを定義できます。 [&#x200B; テンプレートセクションのカスタマイズ &#x200B;](/help/user-guide/templates/customize-template.md#sections-or-groups)を参照してください。

複数セクションのテンプレートには、0、2、または3つのセクションを含めることができます。

- 基本的なテンプレート（0個のセクション）は、テンプレート要素のセットを1つ生成できますが、グループ命名規則は必要ありません。
- 複雑なテンプレート （複数のセクション）は、最大3つのテンプレート要素セットを生成できます。これには、グループの命名規則`<groupname_fieldname>`に従う必要があります。
- 複数のセクションを使用する場合、1つのセクションの外でスタンドアロンのままになっている要素は入力されません。

次に、グループ命名規則を使用したフィールド名の例を2つのセクションに示します。

- セクション 1:`pod1_headline`、`pod1_body`、`pod1_cta`内
- セクション 2:`pod2_headline`、`pod2_body`、`pod2_cta`で

## テンプレートの例

+++例：1つのセクションを含むメールテンプレート

以下は、1つのセクションを含むHTML メールテンプレートの基本的な例です。 `<head>`にはスタイル設定のためのシンプルなインライン CSSが含まれており、`<body>`には`pre_header`、`headline`、`sub_headline`、`body`、`cta`、`image`などのコンテンツ プレースホルダーがリンクと共に使用されています。 これらのプレースホルダーを使用すると、GenStudio for Performance Marketingでメール作成中に動的コンテンツを挿入できます。

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Marketing Email</title>
        <style>
            .container {
                width: 100%;
                padding: 20px;
                font-family: Arial, sans-serif;
            }
            .cta-button {
                display: inline-block;
                background-color: #fff;
                color: #000;
                border: 2px solid #000;
                padding: 10px 20px;
                text-decoration: none;
                font-family: 'Source Sans Pro', Arial, sans-serif;
                font-weight: 600;
                font-size: 14px;
                margin-top: 20px;
                text-align: center;
            }
        </style>
    </head>
    <body>
        <div class="container">
            {{pre_header}}
            <h1>{{headline}}</h1>
            <p>
                <a href="{{link}}">
                    <img alt="banner headline" src="{{image}}" width="600" height="600">
                </a>
            </p>
            <h2>{{sub_headline}}</h2>
            <p>{{body}}</p>
            <a href="#" class="cta-button">{{cta}}</a>
        </div>
    </body>
</html>
```

+++

+++例：複数のセクションを含むメールテンプレート

上記の例と同じHTML テンプレートですが、さらに2つのセクションがあります。 ヘッドには、グループをスタイル設定するためのインライン CSSが含まれています。 本文では、接頭辞を使用して[&#x200B; コンテンツプレースホルダー](#content-placeholders)を持つ2つのグループを使用します。

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
            .cta-button {
            display: inline-block;
            background-color: #fff; /* Background color to white */
            color: #000; /* Text color to black */
            border: 2px solid #000; /* Border color to black */
            padding: 10px 20px;
            text-decoration: none;            
            font-family: 'Source Sans Pro', Arial, sans-serif;
            font-weight: 600; /* Semibold */
            font-size: 14px;
            margin-top: 20px;
            text-align: center;
            }
        </style>
    </head>
    <body>{{pre_header}}
        <div class="container">
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="pic1" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="pic2" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
            <a href="#" class="cta-button">{{cta}}</a>
        </div>
    </body>
</html>
```

+++
