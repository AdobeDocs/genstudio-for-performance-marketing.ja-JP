---
title: メールテンプレートガイドライン
description: Adobe GenStudio for Performance Marketingでメールテンプレートを使用する際は、ベストプラクティスに従ってください。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: 4760da26d20e91489a74bb238e07f0d3b426c0a1
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# メールテンプレートガイドライン

マーケティングメールテンプレートは、視覚的に魅力的でレスポンシブなメールキャンペーンの基盤となります。 一般に、HTML テンプレートでは、ブランドガイドラインに合わせてレイアウト、タイポグラフィ、カラーおよび画像を制御できます。 GenStudio for Performance Marketingで使用するテンプレートを準備する際には、スタイル設定にセマンティック HTMLとインライン CSS を使用し、スクリプトや外部依存関係を避けます。 HTML テンプレートが適切に構造化されることで、受信者のエクスペリエンスが向上し、配信品質とエンゲージメント率が向上します。

GenStudio for Performance Marketingと連携するようにメールテンプレートをカスタマイズする場合は、次のデザインのベストプラクティスに従います。

- AdobeまたはGoogle フォントの使用
- クリーンでレスポンシブなHTMLとインライン CSS の使用
- JavaScript **使用しない**
- 本文 **コンテナ** は固定幅を使用しないでください
- 画像には base64 エンコーディングを使用しないでください **使用すると** テンプレートサイズが大幅に増加する可能性があります
- HTMLの最大ファイルサイズは 102 KB です

## 認識されたフィールド名

メールテンプレートをカスタマイズする場合は、次の必須フィールドにコンテンツプレースホルダーを使用します。

- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` （Content JPEG、PNG、GIFから選択）

GenStudio for Performance Marketingでは、次のフィールドが自動的に生成されます。 リッチテキストが有効になっていません。 次の場合は、コンテンツプレースホルダーを適用する必要はありません。

- `pre_header`
- `subject`

テンプレートで許可される最大フィールド数は 20 です。 テンプレートでのフィールド名の使用について詳しくは、[ コンテンツプレースホルダー ](/help/user-guide/content/customize-template.md#content-placeholders) を参照してください。

## 複数セクションのメール

_セクション_ を使用すると、コンテンツを個別のグループに整理して、より複雑なレイアウトに対応できます。 Genstudio for Performance Marketing では、グループ命名規則を使用して各セクションを定義できます。 [ テンプレートセクションのカスタマイズ ](/help/user-guide/content/customize-template.md#sections-or-groups) を参照してください。

複数セクションのテンプレートには、0 個、2 個、または 3 個のセクションがあります。

- 基本テンプレート（ゼロセクション）は、グループ命名規則を必要としない単一のテンプレート要素セットを生成できます。
- 複雑なテンプレート（複数のセクション）では、最大 3 つのテンプレート要素セットを生成できます。そのため、グループ命名規則（`groupname_fieldname`）に従う必要があります。

2 つのセクションのフィールド名の例：

- `pod1_headline`、`pod1_body`、`pod1_cta`
- `pod2_headline`、`pod2_body`、`pod2_cta`

## テンプレートの例

+++例：1 つのセクションを持つメールテンプレート

以下は、1 つのセクションを持つHTML メールテンプレートの基本的な例です。 `<head>` には、スタイル設定用のシンプルなインライン CSS が含まれており、`<body>` では、`pre_header`、`headline`、`sub_headline`、`body`、`cta`、`image` with link などのコンテンツプレースホルダーを使用します。 これらのプレースホルダーを使用すると、GenStudio for Performance Marketingでメール生成時に動的コンテンツを挿入できます。

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
            <h1>{{headline}}</h1>
            <p>{{body}}</p>
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
