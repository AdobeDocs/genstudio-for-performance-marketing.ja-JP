---
title: LinkedIn エクスペリエンス
description: Adobe GenStudio for Performance Marketingの LinkedIn エクスペリエンスについて説明します。
feature: Experiences, Content Generation, Create, Generative AI, Variant Generation
badgeBeta: label="Beta" tooltip="この機能は現在Betaにあるので、一部の機能が制限されるか、変更される可能性があります。"
role: User
level: Beginner
source-git-commit: e4f552016fe17d2d7eb61792b62859475f107094
workflow-type: tm+mt
source-wordcount: '252'
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
* コールトゥアクション（CTA）
* 画像
* ブランドロゴ

[ テンプレート要素 ](/help/user-guide/content/use-templates.md#template-elements) を参照してください。

## プログレッシブロード

コンテンツ生成プロセスが開始すると、生成されたコンテンツの各セクションがバリアントとしてキャンバスにプログレッシブに読み込まれます。 エクスペリエンス、アセット、エクスペリエンス内のフィールドとセクションは、生成されるとキャンバスに個別に表示されます。

「**[!UICONTROL 生成]**」をクリックすると、キャンバスの下部に読み込みインジケーターが表示され、生成の進行状況が更新されます。

LinkedIn エクスペリエンスの各フィールドとセクションは、次の順序で順に読み込まれます。

1. すべてのバリエーションのプライマリテキスト
1. コールトゥアクションと関連する URL
1. 見出し
1. 画像上のテキスト
1. ブランドの検証

   ブランドの検証とコンテンツチェックプロセスが行われ、各バリアントに [_コンテンツチェック_ 概要 ](/help/user-guide/guidelines/brand-validation.md#content-check-summary) が入力されます。

## 文字数

LinkedIn バリアントのセットを生成すると、各セクションの文字数が表示されます。 件名行や本文など、生成されたセクションにポインタを合わせるかクリックすると、そのセクションのセクション名と文字数が表示されます。

![ 文字数 ](/help/assets/character-count.png){width="500" zoomable="yes"}
