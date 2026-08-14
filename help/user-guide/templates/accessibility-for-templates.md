---
title: アクセス可能なテンプレートの作成
description: Adobe Adobe GenStudio for Performance Marketingなら、より多くのオーディエンスにリーチし、最適なエクスペリエンスを提供できます。
feature: Media Templates
exl-id: eaaa5d9f-ad45-4fd0-826d-c250deb6d238
TQID: https://experienceleague.adobe.com/b56YHJsOAunGenV-F3u7Y2mo56f6CnnX4qPXyzczPJY
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 371
ht-degree: 0%

---

# アクセス可能なテンプレートの作成

Adobeは、あらゆるオーディエンスに最適な体験を提供することに尽力しています。 詳しくは、[Adobeのアクセシビリティイニシアチブ &#x200B;](https://www.adobe.com/trust/accessibility/initiatives.html)を参照してください。

GenStudio for Performance Marketingにアセットとテンプレートをアップロードすれば、さまざまな体験に対応したコンテンツ制作が可能になります。 アクセシビリティ基準を遵守することで、コンテンツが意図する最大限のオーディエンスにリーチできるようになります。

最適なアクセシビリティ標準を使用してテンプレートを準備するには、次の推奨事項を使用します。

## 代替テキスト

画像など、テキスト以外のコンテンツに代替テキストを提供します。

```html
<img alt="Collage of ideas, books, man holding giant pencil, computer" src="card-create-assets.png">
```

![&#x200B; アイデア、本、巨大な鉛筆を持つ男性、コンピューターのコラージュ &#x200B;](/help/assets/card-create-assets.png){width="400"}

テンプレートをカスタマイズするときは、`alt`および`aria-label`属性にコンテンツプレースホルダーを使用します。

- [代替テキスト &#x200B;](/help/user-guide/templates/customize-template.md#alternative-text)
- [&#x200B; アクセシビリティラベル &#x200B;](/help/user-guide/templates/customize-template.md#accessibility-label)

## フォント

読みやすいフォントを使う： 例えば、サンセリフ体のフォントは、ブロックのようなクリーンな外観を持つため、読みやすさが向上します。

テキストと背景の適切なコントラストを指定します。 暗い背景に暗いテキスト、明るい背景に明るいテキストが生成されるフォントカラーは使用しないでください。 最適な比率のコントラストガイドラインを検討します。

- テキストとテキストの画像：少なくとも4.5:1のコントラスト比
- 大きなテキストと大きなサイズのテキストの画像：少なくとも3:1のコントラスト比

## リンクの目的（リンクのみ）

リンクの目的と場所を説明する明確なリンクテキストを作成します。

例えば、「ここをクリック」や「詳細を読む」などのリンクテキストを使用しても、リンクの目的は明確に説明されません。

```html
<a href="product-site.html">Click here</a>
```

ベストプラクティスとして、リンク先を明確に説明するテキストを使用する必要があります。 より良い例としては、リンクソースのタイトルと目的を使用できます。

```html
<a href="product-site.html">Explore Product Site</a>
```

## 言語

多くの製品やサービスは、クリエイティブまたはユニークな方法で言語を使用しています。 専門用語、長い文章、複雑なフレーズは避けます。 ターゲットオーディエンスに対応した、明確で簡潔で読みやすい言語を使用しましょう。

- 可能であれば、明確な説明、インライン定義、関連する例を使用する。 独特の言語を翻訳するのは難しいかもしれません。

- 略語または略語の最初のインスタンスの定義にスペルアウトまたはリンクします。 略語を翻訳するのは難しいかもしれません。

- 可能であれば、ビジュアル要素を使用してテキストや複雑なアイデアを補完します。
