---
title: LinkedIn テンプレートのガイドライン
description: Adobe GenStudio for Performance Marketingで LinkedIn テンプレートを使用する際は、ベストプラクティスに従ってください。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 85432185-8311-411b-b57b-f482c3d45854
TQID: https://experienceleague.adobe.com/YyG3WuMkdVAaACX03qLKzzw-fFA3WfT9K2ohjnQNPcI
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 287
ht-degree: 2%

---

# LinkedIn テンプレートのガイドライン

LinkedIn テンプレートは、LinkedIn キャンペーン用の広告クリエイティブを構造化された方法で作成およびカスタマイズします。 これらのガイドラインは、広告が LinkedIn の仕様を満たしながら、GenStudio for Performance Marketingのクリエイティブプロセスを合理化することを保証します。 このガイドは、LinkedIn のデスクトップおよびモバイルプラットフォーム全体で一貫したブランディングと効果的なパフォーマンスを準備するのに役立ちます。

LinkedIn 広告テンプレートをカスタマイズしてGenStudio for Performance Marketingと連携させる場合は、次のデザインのベストプラクティスに従います。

- 1 つの画像フィールドのみが必要です
- 最大画像サイズは 5 MB
- 最大見出し 70 文字
- 150 文字以内の紹介文
- 使用できるセクションは 1 つだけで、単一のテンプレート要素セットが生成されます

## 認識されたフィールド名

LinkedIn テンプレートをカスタマイズする場合は、次の必須フィールドにコンテンツプレースホルダーを適用します。

- `image` （必須、コンテンツJPEG、PNG またはGIFから選択）
- `on_image_text` （画像上に表示されるテキスト）

GenStudio for Performance Marketingでは、次のフィールドが自動的に生成されます。 次の場合は、コンテンツプレースホルダーを適用する必要はありません。

- `headline`
- `introductory_text`
- `cta` （Call to action）

テンプレートでのフィールド名の使用について詳しくは、[ コンテンツプレースホルダー ](/help/user-guide/templates/customize-template.md#content-placeholders) を参照してください。

## サポートされる縦横比

すべての LinkedIn テンプレートの幅は、1200 ピクセルでハードコードされています。

| 縦横比 | プラットフォーム | ディメンション （px） | メモ |
|-------------------|-----------------|------------|-------------------------------------------------------------------------------------|
| 正方形 1:1 | デスクトップ、モバイル | 1200 x 1200 | 最も用途が広い。 デバイスやプレースメント間で一貫した外観に最適です。 |
| 水平 1.91:1 | デスクトップ | 1200 x 628 | 標準（横置き）。 スポンサー付きコンテンツおよびニュースフィード広告に一般的に使用されます。 |
| 縦 1:1.91 | モバイル | 1200 x 2292 | 縦長の縦書き書式。 モバイル表示用に最適化され、より多くの画面が表示されます。 |
| 縦 2:3 | モバイル | 1200 x 1800 | 1:1.91 より少し背が低い。 モバイルファーストキャンペーンに適しています。 |
| 縦 4:5 | モバイル | 1200 x 1500 | モバイルにおすすめします。 表示とコンテンツのバランスを取ることができます。これにより、多くの場合、より大きな影響が生じます。 |

<!-- Potentially add an example

## Template example

+++Example: LinkedIn template

+++

-->
