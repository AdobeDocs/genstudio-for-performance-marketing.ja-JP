---
title: 広告テンプレートガイドラインの表示
description: Adobe GenStudio for Performance Marketingでディスプレイ広告とバナーテンプレートを使用する際は、ベストプラクティスに従ってください。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
source-git-commit: 4760da26d20e91489a74bb238e07f0d3b426c0a1
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 1%

---

# 広告テンプレートガイドラインの表示

ディスプレイテンプレートは、視覚的に魅力的なバナーやディスプレイ広告の作成に使用される事前に設計されたレイアウトです。 画像、テキスト、call to actionを組み込むための柔軟なフレームワークが提供されるので、複数の広告バリエーションを作成する際に一貫性と効率を確保できます。 GenStudio for Performance Marketingで使用するテンプレートを準備する場合は、すべてのアセットが web 表示用に最適化され、必要なファイル形式とサイズを満たしていることを確認します。

GenStudio for Performance Marketingと連携するようにバナーとディスプレイ広告のテンプレートをカスタマイズする場合は、次のデザインのベストプラクティスに従ってください。

- AdobeまたはGoogle フォントの使用
- スリムなサイズで適切に表示されるアセットの準備
- 1 つの画像フィールドのみが必要です
- 埋め込み画像またはエンコードされた背景画像は使用し **い**
- GenStudio for Performance Marketing コンテンツリポジトリにアップロードされた背景画像（`image` フィールド）を使用
- JavaScript **使用しない**
- 使用できるセクションは 1 つだけで、単一のテンプレート要素セットが生成されます

## 認識されたフィールド名

バナーやディスプレイ広告テンプレートをカスタマイズする場合は、次の必須フィールドにコンテンツプレースホルダーを使用します。

- `headline`
- `sub_headline`
- `body`
- `image` （必須、コンテンツJPEG、PNG またはGIFから選択）

GenStudio for Performance Marketingでは、次のフィールドが自動的に生成されます。 次の場合は、コンテンツプレースホルダーを適用する必要はありません。

- `cta`

テンプレートでのフィールド名の使用について詳しくは、[ コンテンツプレースホルダー ](/help/user-guide/content/customize-template.md#content-placeholders) を参照してください。

## サポートされるディメンション

幅 x 高さ（ピクセル）を設定する必要があります。

| オリエンテーション | 寸法（ピクセル） | メモ |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| 垂直方向 | 300 x 600<br>160 x 600 | 超高層ビルやハーフページバナーに共通 |
| 水平方向 | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | 標準のリーダーボード、中程度の長方形、バナーのサイズ |
| カスタム | 50 x 50 ～ 2000 x 2000 | 非標準または一意のプレースメントに使用、プラットフォームの制限を確認 |

<!-- Potentially add an example

## Template example

+++Example: Display ad template

+++

-->
