---
title: メールテンプレートガイドライン
description: Adobe GenStudio for Performance Marketingでメールテンプレートを使用する際は、ベストプラクティスに従ってください。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: d9d774f727b69b18af6114965fdb8ffb450f797b
workflow-type: tm+mt
source-wordcount: '406'
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

GenStudio for Performance Marketingによって、メールの「`subject`」フィールドが自動生成されます。 テンプレートをカスタマイズする場合、次の必須フィールドにコンテンツプレースホルダーを使用します。

- `pre_header` （リッチテキストが有効になっていません）
- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` （Content JPEG、PNG、GIFから選択）

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
