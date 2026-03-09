---
title: メールエクスペリエンス
description: Adobe GenStudio for Performance Marketingでのメールエクスペリエンスについて説明します。
feature: Create Canvas, Media Templates
role: User
level: Beginner
exl-id: e2bddd02-914e-43a8-92b6-fdcbced94a6a
TQID: https://experienceleague.adobe.com/-lwSfvc0TnVd8byNT-5OfoEsXz7yaeIifcHOJtp-n4c
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2:
  - id: a8b28c00-da6e-4d27-8667-80f790ad8972
  - id: be495d08-ecd1-455f-951e-c22de504e667
  - id: dee4e9a9-78d1-4953-8179-f8da6117027d
  - id: ee4b6e5f-5b7a-421b-9859-0f964841a866
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 309
ht-degree: 0%

---

# メールエクスペリエンス

Adobe GenStudio for Performance Marketingでは、ジェネレーティブ AI を使用して [&#x200B; 効果的なメールエクスペリエンスの作成 &#x200B;](/help/user-guide/create/create-email-experience.md) を合理化できます。

[!DNL Create] を使用すると、最新のマーケターは [&#x200B; ガイドライン &#x200B;](/help/user-guide/guidelines/overview.md)、画像アセット、および [&#x200B; 適切に作成されたプロンプト &#x200B;](/help/user-guide/effective-prompts.md) を使用して、ブランドに合ったメールエクスペリエンスをすばやく [&#x200B; 作成 &#x200B;](/help/user-guide/create/create-email-experience.md) できます。

メールエクスペリエンスを生成する際には、4 つのバリエーションが作成され、キャンバスに表示されます。

メールエクスペリエンスの編集可能なセクションには、次のものが含まれます。

* プリヘッダー
* 見出し
* サブ見出し
* 本文
* Call to action（CTA）
* 画像

[&#x200B; テンプレート要素 &#x200B;](/help/user-guide/templates/use-templates.md#template-elements) を参照してください。

<!-- ## Email capabilities

Content creators and marketers can produce brand-consistent email experiences in GenStudio for Performance Marketing. -->

## 複数セクションのメール

メールエクスペリエンスには複数のセクションを含めることができるので、ブランドや目標に合わせて完全にカスタマイズできます。[&#x200B; [!DNL Products]  各セクションのアセットを選択して視覚的に表示し &#x200B;](/help/user-guide/create/create-email-experience.md#add-parameters) [&#x200B; 構造化プロンプト &#x200B;](/help/user-guide/effective-prompts.md#structured-prompts) を使用して一意のコンテンツを作成します。 各セクションは、1 つのビジュアルアセットをサポートします。

複数セクションのテンプレートを作成する方法については、[&#x200B; セクションを使用したテンプレートのカスタマイズ &#x200B;](/help/user-guide/templates/customize-template.md#sections-or-groups) を参照してください。

## プログレッシブロード

コンテンツ生成プロセスが開始すると、メールバリアント内の生成されたコンテンツの各セクションがキャンバスにプログレッシブに読み込まれます。 エクスペリエンス、アセット、エクスペリエンス内のフィールドとセクションは、生成されるとキャンバスに個別に表示されます。

「**[!UICONTROL 生成]**」をクリックすると、キャンバスの下部に読み込みインジケーターが表示され、生成の進行状況が更新されます。

メールエクスペリエンスの各フィールドとセクションは、次の順序で順に読み込まれます。

1. バリアント名
1. すべてのバリエーションの件名
1. プリヘッダー
1. 見出し、メール本文（単一セクションのメールの場合）、コールトゥアクション
1. 後続セクションのメール本文（複数セクションのメールの場合）
1. ブランドの検証

   ブランドの検証とコンテンツチェックプロセスが行われ、各バリアントに [_コンテンツチェック_ 概要 &#x200B;](/help/user-guide/guidelines/brand-validation.md#content-check-summary) が入力されます。

## 文字数

E メールバリアントのセットを生成したら、各セクションに表示される文字数を確認できます。 件名行や本文など、生成されたセクションにポインタを合わせるかクリックすると、そのセクションのセクション名と文字数が表示されます。

![&#x200B; 文字数 &#x200B;](/help/assets/character-count.png){width="500" zoomable="yes"}
