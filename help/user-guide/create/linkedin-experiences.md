---
title: LinkedIn エクスペリエンス
description: Adobe GenStudio for Performance Marketingの LinkedIn エクスペリエンスについて説明します。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="この機能は現在Betaにあるので、一部の機能が制限されるか、変更される可能性があります。"
role: User
level: Beginner
exl-id: 4d43a214-c635-440f-9dbb-f371bc253195
source-git-commit: 8d79c2bd2347bebb18ecb432a7087fb3d1ac1356
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# LinkedIn エクスペリエンス

Adobe GenStudio for Performance Marketingでは、ジェネレーティブ AI を活用して、効率的に [ 強力な LinkedIn エクスペリエンスを作成 ](/help/user-guide/create/create-linkedin.md) できます。

[!DNL Create] を使用すると、コンテンツ作成者やマーケターは、[ ガイドライン ](/help/user-guide/guidelines/overview.md)、画像アセット、[ 指示プロンプト ](/help/user-guide/effective-prompts.md) を使用して、ブランドに準拠した LinkedIn エクスペリエンスを [ 生成 ](/help/user-guide/create/create-email-experience.md) できます。

LinkedIn エクスペリエンスを生成する際には、4 つのバリエーションが作成され、キャンバスに表示されます。

LinkedIn エクスペリエンスの編集可能なセクションは次のとおりです。

* 見出し
* 紹介テキスト
* 説明
* Call to action（CTA）
* 画像

[ テンプレート要素 ](/help/user-guide/content/use-templates.md#template-elements) を参照してください。

## プログレッシブロード

コンテンツ生成プロセスが開始すると、生成されたコンテンツの各セクションがバリアントとしてキャンバスにプログレッシブに読み込まれます。 エクスペリエンス、アセット、エクスペリエンス内のフィールドとセクションは、生成されるとキャンバスに個別に表示されます。

「**[!UICONTROL 生成]**」をクリックすると、キャンバスの下部に読み込みインジケーターが表示され、生成の進行状況が更新されます。

LinkedIn エクスペリエンスの各フィールドとセクションは、次の順序で順に読み込まれます。

1. すべてのバリエーションのプライマリテキスト
1. Call-to-actionと関連する URL
1. 見出し
1. 画像上のテキスト
1. ブランドの検証

   ブランドの検証とコンテンツチェックプロセスが行われ、各バリアントに [_コンテンツチェック_ 概要 ](/help/user-guide/guidelines/brand-validation.md#content-check-summary) が入力されます。

## 文字数

LinkedIn バリアントのセットを生成すると、各セクションの文字数が表示されます。 件名行や本文など、生成されたセクションにポインタを合わせるかクリックすると、そのセクションのセクション名と文字数が表示されます。

![ 文字数 ](/help/assets/character-count.png){width="500" zoomable="yes"}
