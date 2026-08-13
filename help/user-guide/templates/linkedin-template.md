---
title: LinkedIn テンプレートガイドライン
description: Adobe GenStudio for Performance MarketingでLinkedIn テンプレートを使用する場合は、ベストプラクティスに従ってください。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 85432185-8311-411b-b57b-f482c3d45854
TQID: https://experienceleague.adobe.com/YyG3WuMkdVAaACX03qLKzzw-fFA3WfT9K2ohjnQNPcI
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
source-git-commit: 242ab858144fd152fd55645143f869fddf7b6fe0
workflow-type: tm+mt
source-wordcount: 293
ht-degree: 2%

---

# LinkedIn テンプレートガイドライン

LinkedInのテンプレートは、LinkedInのキャンペーン用の広告クリエイティブを体系化された方法で作成、カスタマイズすることができます。 これらのガイドラインにより、GenStudio for Performance Marketingでクリエイティブなプロセスを合理化しながら、広告がLinkedInの仕様を満たすようにします。 このガイドでは、LinkedInのデスクトップとモバイルのプラットフォーム全体で一貫したブランディングと効果的なパフォーマンスを実現するための準備を整えるのに役立ちます。

LinkedIn広告テンプレートをGenStudio for Performance Marketingと連携するようにカスタマイズする場合は、次のデザインのベストプラクティスに従ってください。

- 1つの画像フィールドが必要です
- 画像の最大サイズ：5 MB
- 見出しの最大文字数70
- 入門用テキストの最大文字数：150文字
- 使用できるセクションは1つだけで、テンプレート要素のセットが1つ生成されます

## 認識されるフィールド名

LinkedIn テンプレートをカスタマイズする際には、次の必須フィールドにコンテンツプレースホルダーを適用します。

- `image` （必須、Content JPEG、PNGまたはGIFから選択）
- `on_image_text` （画像の上に表示されるテキスト）

GenStudio for Performance Marketingは、次のフィールドを自動生成します。 次の場合、コンテンツプレースホルダーを適用する必要はありません。

- `headline`
- `introductory_text`
- `cta` （Call to action）

テンプレートでのフィールド名の使用について詳しくは、[&#x200B; コンテンツプレースホルダー](/help/user-guide/templates/customize-template.md#content-placeholders)を参照してください。

## サポートされている縦横比

LinkedInのテンプレートの幅はすべて1200 ピクセルでハードコードされています。

| 縦横比 | プラットフォーム | 寸法（px） | メモ |
|-------------------|-----------------|------------|-------------------------------------------------------------------------------------|
| 正方形1:1 | デスクトップ，モバイル | 1200 x 1200 | 汎用性が高い： デバイスやプレースメント全体で一貫性のある外観を実現するのに最適です。 |
| 水平方向1.91:1 | デスクトップ | 1200 x 628 | 標準的な横向き形式： スポンサードコンテンツやニュースフィードの広告によく使用されます。 |
| 縦組み1:1.91 | モバイル | 1200 x 2292 | 縦長の書式。 モバイル表示向けに最適化され、より多くの画面プレゼンスを提供。 |
| 垂直方向2:3 | モバイル | 1200 x 1800 | 1:1.91より少し背が低くなります。 モバイルファーストの施策に最適： |
| 縦組み4:5 | モバイル | 1200 x 1500 | モバイル向け。 可視性とコンテンツのバランスを取ることができ、多くの場合、より高い効果をもたらします。 |

<!-- 
Potentially add an example

## Template example

+++Example: LinkedIn template

+++

-->
