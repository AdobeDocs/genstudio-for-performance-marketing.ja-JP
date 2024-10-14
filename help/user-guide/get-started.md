---
title: Adobe GenStudio for Performance Marketingの概要
description: GenStudio for Performance Marketingの使用を開始して、ブランドに合わせた新しいマーケティングコンテンツを生成する方法を説明します。
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: bcb03198-bbcb-45ae-af01-25c1e834b563
source-git-commit: 6454090c9fffb4b288b615680597b80e5b71a89c
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---

# Adobe GenStudio for Performance Marketingの概要

Adobe GenStudio for Performance Marketingは、コンテンツの作成、管理、分析を合理化するように設計された包括的なツールスイートを提供します。 マーケティングコンテンツの作成、確認、共有、分析の方法を変換する生成 AI 機能をコンテンツ作成ライフサイクルに組み込みます。

## コンテンツの作成、共有、レビューを開始

ジェネレーティブ AI ベースのツールを初めて使用する場合、またはGenStudio for Performance Marketingの基本原則に興味がある場合は、[ 概念 ](concepts.md) および [ 効果的なプロンプトの記述 ](effective-prompts.md) を参照してください。 クリエイティブなプロセスでジェネレーティブ AI テクノロジを活用する方法について、Adobeのオンライン ラーニング プラットフォームである ](https://learningmanager.adobe.com/genstudioacademy)0}Adobe GenStudioアカデミー } をご覧ください。[

## GenStudio for Performance Marketingのトレーニング

GenStudio for Performance Marketingは、ブランドと市場に関する情報を使用して、ブランドに準拠したコンテンツ作成を強化します。 トレーニング資料には、例、顧客 [ ペルソナ ](/help/user-guide/guidelines/personas.md) および [ 製品 ](/help/user-guide/guidelines/products.md) の説明、および [ ブランドガイドライン ](/help/user-guide/guidelines/overview.md) が含まれます。

システム管理者は、組織固有の情報を入力またはアップロードすることでAdobe GenStudio for Performance Marketingを設定します。 この準備により、コンテンツ編集者と共同作業者が生成 AI 機能を効果的に使用して、キャンペーンアセットを作成およびレビューできるようになります。 Adobeシステム管理者が組織の製品インスタンスをプロビジョニングし、GenStudio システムマネージャーの権限を割り当てると、GenStudio システムマネージャーはガイドラインを使用して製品の基盤となる生成 AI フレームワークを準備できます。

### 手順 1：ガイドラインの追加

組織のブランド ID の主要な構成要素を設定することは、コンテンツ編集者や共同作業者の作業にとって不可欠な前提条件です。 [ ガイドライン ](./guidelines/overview.md) ロゴ、声のトーン、カラーパレットなど、ブランドの特徴を取り込みます。 [[!DNL Brands]  ガイドライン ](./guidelines/brands.md) ドキュメントをアップロードするか、ブランド情報を手動で入力できます。 [[!DNL Personas]  ガイドライン ](./guidelines/personas.md) と [[!DNL Products]  ガイドライン ](./guidelines/products.md) も重要です。 GenStudio for Performance Marketingの基盤となるジェネレーティブ AI 機能では、これらのガイドラインを使用して、コンテンツの生成をガイドするガードレールを確立します。

#### ガイドライン文書の準備

包括的で焦点を当てた [[!DNL Brands]](./guidelines/brands.md)、[[!DNL Products]](./guidelines/products.md)、[[!DNL Personas]](./guidelines/personas.md) のガイドラインにより、組織のマーケティングキャンペーンの中心的側面が定義されます。 GenStudio for Performance Marketingでは、ブランドの構築を開始するために、これらのガイドラインから情報を抽出します。

ガイドラインを準備する際は、次のベストプラクティスに従います。

* 特定の言語を使用します。

* キャンペーンアセットで具現化するスタイルとトーンの最適な例を含めます。

* 冗長性を避けます。 ディレクティブを複数回繰り返したくなるかもしれませんが、ガイドラインの冗長性は、基になる LLM がブランドガイドラインを取り込んで実装するのに役立つわけではありません。

* コンテンツ生成時に LLM で除外する要素を識別します（テキスト内の感嘆符など）

ガイドラインのドキュメントをアップロードすることも、GenStudio for Performance Marketingに手動で情報を入力する際に参照することもできます。 この情報をアップロードまたは入力する方法については、[ ガイドラインの追加 ](./guidelines/overview.md) を参照してください。

#### ガイドラインの改訂

GenStudio システムマネージャーは、組織固有のブランド要件を手動で入力またはアップロードすることで、製品の基盤となるジェネレーティブ AI フレームワークを準備できます。 組織のブランドガイドラインの設定は 1 回限りのアクションですが、組織のボラティリティ、成長および市場状況の変化に基づいて、これらのガイドラインを改訂および強化することができます。

### 手順 2：テンプレートのアップロード

テンプレートを使用すると、コンテンツを迅速に作成できます。 テンプレートには、ヘッダーやフッターなど、承認済みの機能が含まれており、特定のチャネル用に最適化されています。 通常、システムマネージャーは組織のテンプレートをアップロードおよび管理します。 コンテンツエディターは、テンプレートを使用して、組織ブランドの確立された境界内でコンテンツ作成プロセスを迅速に開始します。

テンプレートのカスタマイズとアップロードについては、[ テンプレートの操作 ](./content/use-templates.md) を参照してください。

### 手順 3：承認されたアセットのアップロード

[!DNL Content] の承認済みアセットは、すべてのGenStudio for Performance Marketing エディターが使用できます。 コンテンツエディターが新しいエクスペリ [!DNL Content] ンスやアセットの作成に使用するアセットを、アセットに入力することができます。 アセットのアップロードと管理については、[ 承認済みアセットのアップロード ](./content/manage-assets.md) を参照してください。

### 手順 4:Meta （Facebook）アカウントへの接続

GenStudio for Performance Marketingと組織のソーシャルアカウントの間の接続を設定して、アクティブなマーケティングキャンペーン、アセットおよびエクスペリエンスからデータを受け取ります。 [[!DNL Insights]](./insights/overview.md) は、チャネルから派生したデータを分析するツールを提供します。 [Meta （Facebook）アカウントへの接続 ](./insights/connect-channel.md#meta-ads-connect) を参照してください。
