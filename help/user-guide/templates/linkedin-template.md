---
title: LinkedIn テンプレートのガイドライン
description: Adobe GenStudio for Performance Marketingで LinkedIn テンプレートを使用する際は、ベストプラクティスに従ってください。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 85432185-8311-411b-b57b-f482c3d45854
source-git-commit: 3251d81a6bfb0c1f7d2bf3c5bd319ad4e2237699
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 3%

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

テンプレートでのフィールド名の使用について詳しくは、[&#x200B; コンテンツプレースホルダー &#x200B;](/help/user-guide/templates/customize-template.md#content-placeholders) を参照してください。

## サポートされる縦横比

| 縦横比 | プラットフォーム | 最小サイズ （px） | 最大サイズ （px） | メモ |
|-------------------|-----------------|---------------|----------------|-------------------------------------------------------------------------------------|
| 正方形 1:1 | デスクトップ、モバイル | 360 x 360 | 4320 x 4320 | 最も用途が広い。 デバイスやプレースメント間で一貫した外観に最適です。 |
| 水平 1.91:1 | デスクトップ | 640 x 360 | 7680 x 4320 | 標準（横置き）。 スポンサー付きコンテンツおよびニュースフィード広告に一般的に使用されます。 |
| 縦 1:1.91 | モバイル | 360 x 640 | 2430 x 4320 | 縦長の縦書き書式。 モバイル表示用に最適化され、より多くの画面が表示されます。 |
| 縦 2:3 | モバイル | 360 x 640 | 2430 x 4320 | 1:1.91 より少し背が低い。モバイルファーストキャンペーンに適しています。 |
| 縦 4:5 | モバイル | 360 x 640 | 2430 x 4320 | モバイルにおすすめします。 表示とコンテンツのバランスを取ることができます。これにより、多くの場合、より大きな影響が生じます。 |

<!-- Potentially add an example

## Template example

+++Example: LinkedIn template

+++

-->
