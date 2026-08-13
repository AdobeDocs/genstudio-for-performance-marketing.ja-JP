---
title: 広告テンプレートのガイドラインの表示
description: Adobe GenStudio for Performance Marketingでディスプレイ広告とバナーテンプレートを使用する場合は、ベストプラクティスに従ってください。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
TQID: https://experienceleague.adobe.com/HjkLWiyqK1quHoZB5lEE-qyB3zci12KlRAZC8ME-9Ao
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 300
ht-degree: 4%

---

# ディスプレイ広告テンプレートのガイドライン

ディスプレイテンプレートとは、視覚的に魅力的なバナーやディスプレイ広告を作成するために使用される、あらかじめデザインされたレイアウトです。 画像、テキスト、call to actionを組み込むための柔軟なフレームワークを提供し、複数の広告バリエーションを制作する際の一貫性と効率性を確保します。 GenStudio for Performance Marketingで使用するテンプレートを準備する際には、すべてのアセットがweb表示用に最適化され、必要なファイル形式とサイズを満たしていることを確認します。

GenStudio for Performance Marketingを使用してバナー広告とディスプレイ広告テンプレートをカスタマイズする場合は、次のデザインのベストプラクティスに従ってください。

- アドビフォントまたは Google フォントを使用する
- スリムなサイズで適切に表示されるアセットを準備する
- 1つの画像フィールドが必要です
- 埋め込み画像またはエンコードされた背景画像を&#x200B;**使用しない**
- GenStudio for Performance Marketing コンテンツリポジトリーにアップロードされた背景画像（`image` フィールド）を使用します。 最適な結果を得るには、[ ディスプレイ広告用の画像のアップロード ](#uploading-images-for-display-ads)のガイドラインに従ってください
- JavaScript を&#x200B;**使用しない**
- 使用できるセクションは1つだけで、テンプレート要素のセットが1つ生成されます

## 認識されるフィールド名

バナーまたはディスプレイ広告テンプレートをカスタマイズする場合は、次の必須フィールドにコンテンツプレースホルダーを使用します。

- `headline`
- `sub_headline`
- `body`
- `image` （必須、Content JPEG、PNGまたはGIFから選択）

GenStudio for Performance Marketingは、次のフィールドを自動生成します。 次の場合、コンテンツプレースホルダーを適用する必要はありません。

- `cta`

テンプレートでのフィールド名の使用について詳しくは、[ コンテンツプレースホルダー](/help/user-guide/templates/customize-template.md#content-placeholders)を参照してください。

## サポートされているディメンション

幅×高さ（ピクセル）を設定する必要があります。

| オリエンテーション | 寸法（ピクセル） | メモ |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| 垂直方向 | 300 x 600<br>160 x 600 | 高層ビルやハーフページバナーによく見られます。 |
| 水平方向 | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | 標準リーダーボード、中長方形、バナーサイズ。 |
| カスタム | 50 x 50 ～ 2000 x 2000 | 非標準または一意のプレースメントに使用します。プラットフォームの制限を確認してください。 |

