---
title: Meta広告テンプレートのガイドライン
description: Adobe GenStudio for Performance MarketingでMeta広告テンプレートを使用する場合は、ベストプラクティスに従ってください。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
TQID: https://experienceleague.adobe.com/-WHH1xjWFaizXTKjuF-K9UtaR12V3QpMezSqRfwbMIU
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2: id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 380
ht-degree: 2%

---

# Meta広告テンプレートのガイドライン

Metaの広告テンプレートは、Metaのプラットフォーム全体で視覚的に一貫性のある効果的な広告を作成するのに役立ちます。 推奨されるデザイン方法に従い、サポートされているフィールドを使用することで、テンプレートがGenStudio for Performance Marketing向けに最適化されていることを確認できます。 このガイドでは、シームレスな統合とインパクトの大きい結果を実現するために、Meta広告テンプレートを構成、カスタマイズ、準備する方法を説明します。

GenStudio for Performance Marketingを使用してMeta広告テンプレートをカスタマイズする場合は、次のデザインのベストプラクティスに従ってください。

- 列レイアウトに360 ピクセル幅を使用
- 画像に1080 x 1080 ピクセルの最小解像度を使用する
- 1つの画像フィールドが必要です
- **not**&#x200B;は相対フォントサイズを使用しません
- **not**&#x200B;はビューポートを定義しません
- JavaScript を&#x200B;**使用しない**
- CSSのHTML要素を&#x200B;**not**&#x200B;上書きする
- `background-image`の代わりに`<img>` タグを使用
- マスクを使用して、背景画像のテキストの読みやすさを向上させる
- 使用できるセクションは1つだけで、テンプレート要素のセットが1つ生成されます

## 認識されるフィールド名

Meta広告テンプレートをカスタマイズする場合は、次の必須フィールドにコンテンツプレースホルダーを適用します。

- `image` （必須、Content JPEG、PNGまたはGIFから選択）
- `on_image_text` （画像の上に表示されるテキスト）

GenStudio for Performance Marketingは、次のフィールドを自動生成します。 次の場合、コンテンツプレースホルダーを適用する必要はありません。

- `headline`
- `body`
- `cta`

テンプレートでのフィールド名の使用について詳しくは、[ コンテンツプレースホルダー](/help/user-guide/templates/customize-template.md#content-placeholders)を参照してください。

## サポートされている縦横比

| 縦横比 | 寸法（ピクセル） | メモ |
|------------------|----------------------------|-----------------------------------------------------------------------|
| 正方形1:1 | 1080 x 1080 | ほとんどのMeta プレースメントに対して標準です。幅広い互換性を保つために推奨されます。 |
| 縦4:5 | 1080 x 1350 | モバイルフィード向けに最適化され、より垂直なスペースを提供します。 |
| ストーリー9:16 | 1080 x 1920 | ストーリーとリールに最適。モバイル画面全体を満たします。 |
| 横1.91:1 | 1080 x 566 | リンク広告とニュースフィードの配置に最適です。幅広い形式です。 |
| カスタム | 最小50 x 50 （幅） | 必要な場合にのみ使用してください。切り抜きや拡大・縮小が発生する可能性があります。 |

広告がこれらの縦横比のいずれかでデザインされていない場合、GenStudio for Performance Marketingは自動的に画像を適切なサイズに切り抜きます。

## テンプレートの例

+++例：Meta広告テンプレート

<!-- Does this need to be a precise size? -->

次に、Metaの広告テンプレートの基本的な例を示します。 ヘッドには、スタイル設定のためのインライン CSSが含まれています。 本文では、`image`や`on_image_text`など、[ コンテンツプレースホルダー](#content-placeholders)を使用して、GenStudio for Performance Marketingがコンテンツを生成できる場所を示します。

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
