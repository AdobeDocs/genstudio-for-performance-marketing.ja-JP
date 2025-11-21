---
title: Meta広告テンプレートガイドライン
description: Adobe GenStudio for Performance MarketingでMeta広告テンプレートを使用する際は、ベストプラクティスに従ってください。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
source-git-commit: 3251d81a6bfb0c1f7d2bf3c5bd319ad4e2237699
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 1%

---

# Meta広告テンプレートガイドライン

Meta広告テンプレートを使用すると、Meta プラットフォーム間で視覚的に一貫性のある効果的な広告を作成できます。 推奨されるデザインプラクティスに従い、サポートされるフィールドを使用することにより、テンプレートがGenStudio for Performance Marketing用に最適化されるようになります。 このガイドでは、シームレスな統合と効果的な結果を得るためのMeta広告テンプレートの構造化、カスタマイズおよび準備方法について説明します。

GenStudio for Performance Marketingと連携するようにMetaとテンプレートをカスタマイズする場合は、次のデザインのベストプラクティスに従います。

- 列レイアウトには 360 ピクセルの幅を使用
- 画像には 1080 x 1080 ピクセルの最小解像度を使用します
- 1 つの画像フィールドのみが必要です
- 相対的 **フォントサイズを使用しない**
- ビューポートを定義し **い** でください
- JavaScript **使用しない**
- CSS **HTML要素を上書きし** い
- `<img>` の代わりに `background-image` タグを使用します
- マスクを使用して、背景画像のテキスト読みやすさを向上させます
- 使用できるセクションは 1 つだけで、単一のテンプレート要素セットが生成されます

## 認識されたフィールド名

Meta広告テンプレートをカスタマイズする場合は、次の必須フィールドにコンテンツプレースホルダーを適用します。

- `image` （必須、コンテンツJPEG、PNG またはGIFから選択）
- `on_image_text` （画像上に表示されるテキスト）

GenStudio for Performance Marketingでは、次のフィールドが自動的に生成されます。 次の場合は、コンテンツプレースホルダーを適用する必要はありません。

- `headline`
- `body`
- `cta`

テンプレートでのフィールド名の使用について詳しくは、[ コンテンツプレースホルダー ](/help/user-guide/templates/customize-template.md#content-placeholders) を参照してください。

## サポートされる縦横比

| 縦横比 | 寸法（ピクセル） | メモ |
|------------------|----------------------------|-----------------------------------------------------------------------|
| 正方形 1:1 | 1080 x 1080 | ほとんどのMeta プレースメントの標準。幅広い互換性を実現するために推奨されます。 |
| 縦 4:5 | 1080 x 1350 | モバイルフィード用に最適化され、より垂直方向のスペースを提供します。 |
| ストーリー 9:16 | 1080 x 1920 | ストーリーやリールに最適です。モバイル画面全体を埋めます。 |
| 横 1.91:1 | 1080 x 566 | リンク広告やニュースフィードのプレースメントに最適（ワイドフォーマット）。 |
| カスタム | 最小 50 x 50 （幅） | 必要な場合にのみ使用してください。切り抜きや拡大縮小が行われる可能性があります。 |

広告がこれらの縦横比のいずれかで設計されていない場合、GenStudio for Performance Marketingは画像を適切なサイズに自動的に切り抜きます。

## テンプレートの例

+++例：Meta広告テンプレート

<!-- Does this need to be a precise size? -->

次に、Meta広告テンプレートの基本的な例を示します。 ヘッドには、スタイル設定用のインライン CSS が含まれています。 本文では、[ や ](#content-placeholders) などの `image` コンテンツプレースホルダー `on_image_text` を使用して、GenStudio for Performance Marketingでコンテンツを生成できる場所を示します。

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
