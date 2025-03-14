---
title: メタエクスペリエンス
description: Adobe GenStudio for Performance Marketingのメタエクスペリエンスについて説明します。
feature: Experiences, Content Generation, Create, Generative AI, Variant Generation
role: User
level: Beginner
exl-id: c1265a9d-8205-4abc-9652-1d8b88397f14
source-git-commit: e4f552016fe17d2d7eb61792b62859475f107094
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# メタエクスペリエンス

Adobe GenStudio for Performance Marketingでは、ジェネレーティブ AI を使用して [ 効果的なメタエクスペリエンスの作成 ](/help/user-guide/create/create-meta-ad.md) を効率化できます。

[!DNL Create] を使用すると、コンテンツ作成者は [ ガイドライン ](/help/user-guide/guidelines/overview.md)、画像アセット、[ 適切に作成されたプロンプト ](/help/user-guide/effective-prompts.md) を使用して、メタ広告エクスペリエンスをすばやく [ 作成 ](/help/user-guide/create/create-meta-ad.md) できます。

メタエクスペリエンスを生成する際には、4 つのバリエーションが作成され、キャンバスに表示されます。

GenStudio for Performance Marketingは、[ 標準サイズとカスタムサイズのメタ広告 ](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) の両方をサポートしています。

メールエクスペリエンスの編集可能なセクションには、次のものが含まれます。

* 見出し
* 本文
* コールトゥアクション（CTA）
* 画像上のテキスト
* 画像
* ブランドロゴ

[ テンプレート要素 ](/help/user-guide/content/use-templates.md#template-elements) を参照してください。

<!-- ## Meta ad capabilities

Content creators and marketers can produce brand-consistent Meta ad experiences in GenStudio for Performance Marketing. -->

## メタ広告チャネル

メタ広告エクスペリエンスを作成する場合は、Facebook と Instagram の両方のチャネルのバリアントを生成できます。 Facebook 広告と Instagram 広告を切り替えて、各チャネルのバリアントをプレビューします。

[ メタ広告チャネルの選択 ](/help/user-guide/create/create-meta-ad.md#choose-meta-ads-channel) を参照してください。

## プログレッシブロード

コンテンツ生成プロセスが開始すると、生成されたコンテンツの各セクションがバリアントとしてキャンバスにプログレッシブに読み込まれます。 エクスペリエンス、アセット、エクスペリエンス内のフィールドとセクションは、生成されるとキャンバスに個別に表示されます。

「**[!UICONTROL 生成]**」をクリックすると、キャンバスの下部に読み込みインジケーターが表示され、生成の進行状況が更新されます。

メタ広告エクスペリエンスの各フィールドとセクションは、次の順序で順に読み込まれます。

1. すべてのバリエーションのプライマリテキスト
1. コールトゥアクションと関連する URL
1. 見出し
1. 画像上のテキスト
1. ブランドの検証

   ブランドの検証とコンテンツチェックプロセスが行われ、各バリアントに [_コンテンツチェック_ 概要 ](/help/user-guide/guidelines/brand-validation.md#content-check-summary) が入力されます。

## 文字数

一連の Meta バリアントを生成すると、各セクションの文字数が表示されます。 件名行や本文など、生成されたセクションにポインタを合わせるかクリックすると、そのセクションのセクション名と文字数が表示されます。

![ 文字数 ](/help/assets/character-count.png){width="500" zoomable="yes"}
