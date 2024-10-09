---
title: Adobe GenStudio for Performance Marketing用のメールテンプレートの準備
description: Adobe GenStudio for Performance Marketingのカスタムメールテンプレートを作成する方法について説明します。
level: Intermediate
feature: Templates, Content
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: ce08231cb723bec3d80a732837b72a435d3b552d
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Adobe GenStudio for Performance Marketing用メールテンプレートの準備

通常、デザイナーは、Adobe XDなどのデザインプログラムでテンプレートのビジュアルデザインを作成します。 メールテンプレートを設計、コーディング、テストしたら、GenStudio for Performance Marketingでアップロードおよび使用できるように準備できます。

[ テンプレート要素 ](use-templates.md#template-elements) を参照してください。

## ガイドラインの追加

メタ広告テンプレートを準備する前に、GenStudio for Performance Marketingに [ ガイドライン ](/help/user-guide/guidelines/overview.md) が追加され、関連するブランドの包括的な情報が入力されていることを確認します。 [ ブランドガイドライン ](/help/user-guide/guidelines/brands.md) は、生成されるコンテンツに直接影響します。

**例**：メールテンプレートの本文を 500 文字以下にする場合は、「本文」フィールドの [ チャネルガイドライン ](/help/user-guide/guidelines/brands.md#channel-guidelines) にその要件を追加します。

ガイドラインがGenStudio for Performance Marketingに追加されていない場合は、デフォルトが使用されます。

## メールテンプレートのコーディング

テンプレートは、デザイン後、HTMLとインライン CSS を使用してコーディングされます。 コードは、様々なデバイスに対してクリーンでレスポンシブである必要があります。

[ テンプレートの例 ](/help/user-guide/content/customize-template.md#template-examples) を参照してください。

### 複数セクションのメール

コンテンツ生成時に [ 構造化プロンプト ](/help/user-guide/effective-prompts.md#structured-prompts) を使用して、メールのセクションごとに様々なコンテンツを生成するようGenStudio for Performance Marketingに指示できます。

例えば、メールテンプレート内のセクションの先頭に `Pod`—`Pod1` と `Pod2` が付いている場合、コンテンツ生成の構造化されたプロンプトには、これらのメールセクションの特定のディレクティブを含めることができます。 GenStudio for Performance Marketingは、プロンプトでセクション固有のディレクティブを関連するメールセクションに一致させ、ディレクティブに合わせたコンテンツを生成します。

[ 構造化プロンプト ](/help/user-guide/effective-prompts.md#structured-prompts) を参照してください。

## メールテンプレートのテスト

メール配信またはプルーフプラットフォームを使用して、メールをテストし、様々なメールクライアントやデバイスで正しくレンダリングされていることを確認します。

メールテンプレートが次の条件を満たしていることをテストで確認します。

* レイアウトは、CSS メディアクエリを使用して様々な画面サイズに合わせて調整します
* ボタンをクリックして目的の場所に移動できます
* メールテンプレートは読みやすく、モバイルデバイスでも使用できます

## 生成されたコンテンツ領域の定義

GenStudio for Performance Marketingのコンテンツを動的に入力するメールテンプレート内の領域を定義します。

生成されたコンテンツ領域を定義するには：

* GenStudio for Performance Marketingで自動生成するテンプレート内のテキスト要素（ヘッドラインやCTAなど）を指定します。
* Handlebars 構文を使用してプレースホルダーを挿入し、HTMLテンプレートを調整します。

[ コンテンツのプレースホルダー ](/help/user-guide/content/customize-template.md#content-placeholders) を参照してください。

## テンプレートのプレビュー

組み込みヘルパーを使用して、特定のコンテンツ領域の表示を制御します。 例えば、クリーンなプレビューリンクを維持しながら、書き出されたテンプレート内のリンクにトラッキングパラメーターを含めることができます。

[ テンプレートプレビュー ](/help/user-guide/content/customize-template.md#template-preview) を参照してください。

## テンプレートのアップロードと使用

テンプレートの設計、コーディング、テストおよびプレビューが完了したら、GenStudio for Performance Marketingにアップロードして、まったく新しいマーケティングコンテンツの生成に使用できます。

[ テンプレートの操作 ](use-templates.md) を参照してください。
