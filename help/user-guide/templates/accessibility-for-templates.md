---
title: アクセシブルなテンプレートの作成
description: Adobe GenStudio for Performance Marketingでテンプレートを作成して、より多くのオーディエンスにリーチし、最適なエクスペリエンスを提供できるようにします。
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
source-wordcount: 369
ht-degree: 0%

---

# アクセシブルなテンプレートの作成

Adobeは、すべてのオーディエンスに最適なエクスペリエンスを提供するよう取り組んでいます。 詳しくは、[Adobeでのアクセシビリティイニシアチブ &#x200B;](https://www.adobe.com/trust/accessibility/initiatives.html) を参照してください。

GenStudio for Performance Marketingでは、様々なエクスペリエンスのコンテンツを作成できるアセットとテンプレートをアップロードできます。 アクセシビリティ標準に準拠することで、コンテンツが対象オーディエンスの上限に到達することができます。

最適なアクセシビリティ標準を使用してテンプレートを準備するには、次の推奨事項を使用します。

## 代替テキスト

画像など、テキスト以外のコンテンツには代替テキストを提供します。

```html
<img alt="Collage of ideas, books, man holding giant pencil, computer" src="card-create-assets.png">
```

![&#x200B; アイデア、本、巨大な鉛筆を持つ男、コンピュータのコラージュ &#x200B;](/help/assets/card-create-assets.png){width="400"}

テンプレートをカスタマイズする場合は、`alt` 属性と `aria-label` 属性のコンテンツプレースホルダーを使用します。

- [&#x200B; 代替テキスト &#x200B;](/help/user-guide/templates/customize-template.md#alternative-text)
- [&#x200B; アクセシビリティラベル &#x200B;](/help/user-guide/templates/customize-template.md#accessibility-label)

## フォント

読みやすいフォントを使用します。 例えば、サンセリフフォントはクリーンなブロック状の外観をしており、読みやすさが向上します。

テキストと背景の間に適切なコントラストを指定します。 暗い背景に暗いテキスト、明るい背景に明るいテキストを生成するフォントカラーを使用しないでください。 最適な比率を得るには、コントラストのガイドラインを考慮してください。

- テキストおよびテキストの画像：4.5:1 以上のコントラスト比
- 大きなテキストと大きなテキストの画像：3:1 以上のコントラスト比

## リンクの目的（リンクのみ）

リンクの目的と場所を説明する明確なリンクテキストを作成します。

例えば、「ここをクリック」や「詳細を読む」などのリンクテキストを使用しても、リンクの目的が明確に説明されるわけではありません。

```html
<a href="product-site.html">Click here</a>
```

ベストプラクティスとして、リンクの移動先を明確に説明するテキストを使用する必要があります。 より良い例としては、リンクソースのタイトルと目的を使用できます。

```html
<a href="product-site.html">Explore Product Site</a>
```

## 言語

多くの製品やサービスは、クリエイティブなまたは独自の方法で言語を使用しています。 専門用語、長い文、複雑な語句を避けます。 ターゲットオーディエンスと互換性のある、明確で簡潔で読みやすい言語を使用します。

- 可能な場合は、明確な説明、インライン定義または関連可能な例を使用します。 ユニークな言葉を翻訳するのは難しい場合があります。

- 頭字語または略語の最初のインスタンスの定義を入力するか、定義へのリンクを設定します。 略語の翻訳は難しい場合があります。

- 可能な場合は、視覚要素を使用して、テキストや複雑なアイデアを補います。
