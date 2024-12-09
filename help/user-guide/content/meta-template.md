---
title: Adobe GenStudio for Performance Marketing用のメタ広告テンプレートの準備
description: Adobe GenStudio for Performance Marketingのカスタムメタ広告テンプレートを作成する方法について説明します。
level: Intermediate
hidefromtoc: true
feature: Templates, Content
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
source-git-commit: cf6e0679999614a4d14d224c9a8dce0b66f50262
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Adobe GenStudio for Performance Marketing用のメタ広告テンプレートの準備

メタ広告テンプレートを作成するには、ソーシャルメディア用にカスタマイズされた構造化アプローチが必要です。 メタ広告テンプレートを設計およびテストしたら、GenStudio for Performance Marketingでアップロードおよび使用できるように準備できます。

## ガイドラインの追加

メタ広告テンプレートを準備する前に、GenStudio for Performance Marketingに [ ガイドライン ](/help/user-guide/guidelines/overview.md) が追加され、関連するブランドの包括的な情報が入力されていることを確認します。 [ ブランドガイドライン ](/help/user-guide/guidelines/brands.md) は、生成されるコンテンツに直接影響します。

**例**：メタ広告テンプレートの本文を 500 文字以下にする場合は、「本文」フィールドの [ チャネルガイドライン ](/help/user-guide/guidelines/brands.md#channel-guidelines) にその要件を追加します。

ガイドラインがGenStudio for Performance Marketingに追加されていない場合は、デフォルトが使用されます。

## テンプレートのデザイン

通常、デザイナーは、Adobe XDなどのデザインプログラムでテンプレートのビジュアルデザインを作成します。

[ テンプレート要素 ](use-templates.md#template-elements) および [ テンプレート例 ](/help/user-guide/content/customize-template.md#template-examples) を参照してください。

### 広告仕様

GenStudio for Performance Marketingでは、メタ広告に対して次の縦横比をサポートしています。

* 正方形（1:1）: 1080 x 1080 ピクセル
* 縦長（4:5）: 1080 x 1350 ピクセル
* ストーリー（9:16）: 1080 x 1920 ピクセル

広告がこれらの縦横比のいずれかで設計されていない場合、GenStudio for Performance Marketingは画像を適切なサイズに自動的に切り抜きます。

## メタ広告テンプレートのテスト

Meta の Creative Hub を使用してテンプレートをテストし、フィードやストーリーなどの様々なプレースメントで広告がどのように表示されるかを確認します。

メール配信またはプルーフプラットフォームを使用して、メールをテストし、様々なメールクライアントやデバイスで正しくレンダリングされていることを確認します。

## 生成されたコンテンツ領域の定義

GenStudio for Performance Marketingのコンテンツを動的に入力するメールテンプレート内の領域を定義します。

生成されたコンテンツ領域を定義するには：

* GenStudio for Performance Marketingで自動生成するテンプレート内のテキスト要素（ヘッドラインやCTAなど）を指定します。
* Handlebars 構文を使用してプレースホルダーを挿入し、HTMLテンプレートを調整します。

[ コンテンツのプレースホルダー ](/help/user-guide/content/customize-template.md#content-placeholders) を参照してください。

## テンプレートのプレビュー

組み込みヘルパーを使用して、特定のコンテンツ領域の表示を制御します。 例えば、クリーンなプレビューリンクを維持しながら、書き出されたテンプレート内のリンクにトラッキングパラメーターを含めます。

[ テンプレートプレビュー ](/help/user-guide/content/customize-template.md#template-preview) を参照してください。

## テンプレートのアップロードと使用

テンプレートの設計、コーディング、テストおよびプレビューが完了したら、GenStudio for Performance Marketingにアップロードして新しいマーケティングコンテンツの生成に使用できます。

[ テンプレートの操作 ](use-templates.md) を参照してください。
