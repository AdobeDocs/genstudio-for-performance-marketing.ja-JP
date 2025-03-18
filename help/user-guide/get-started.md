---
title: Adobe GenStudio for Performance Marketingの概要
description: パフォーマンスマーケティング用の GenStudio の使用を開始して、ブランドに合わせた新しいマーケティングコンテンツを生成する方法について説明します。
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: bcb03198-bbcb-45ae-af01-25c1e834b563
source-git-commit: 462834fb622dae4680a64e3de5c370b9268ee4cb
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 2%

---

# Adobe GenStudio for Performance Marketingの概要

Adobe GenStudio for Performance Marketingは、コンテンツの作成、管理、分析を合理化するように設計された包括的なツールスイートを提供します。 マーケティングコンテンツの作成、確認、共有、分析の方法を変換する生成 AI 機能をコンテンツ作成ライフサイクルに組み込みます。

## コンテンツの作成、共有、レビューを開始

ジェネレーティブ AI ベースのツールを初めて使用する場合、またはGenStudio for Performance Marketingの基本原則に興味がある場合は、[ 概念 ](concepts.md) および [ 効果的なプロンプトの記述 ](effective-prompts.md) を参照してください。 クリエイティブなプロセスでジェネレーティブ AI テクノロジーを活用する方法については、Adobeのオンライン ラーニング プラットフォームである ](https://learningmanager.adobe.com/genstudioacademy)0}Adobe GenStudio Academy} をご覧ください。[

## GenStudio for Performance Marketingのトレーニング

GenStudio for Performance Marketingは、ブランドと市場に関する情報を使用して、ブランドに準拠したコンテンツ作成を強化します。 トレーニング資料には、例、顧客 [ ペルソナ ](/help/user-guide/guidelines/personas.md) および [ 製品 ](/help/user-guide/guidelines/products.md) の説明、および [ ブランドガイドライン ](/help/user-guide/guidelines/overview.md) が含まれます。

システム管理者は、組織固有の情報を入力またはアップロードすることでAdobe GenStudio for Performance Marketingを設定します。 この準備により、コンテンツ編集者と共同作業者が生成 AI 機能を効果的に使用して、キャンペーンアセットを作成およびレビューできるようになります。 Adobe システム管理者が組織の製品インスタンスをプロビジョニングし、GenStudio システムマネージャーの権限を割り当てると、GenStudio システムマネージャーはガイドラインを使用して製品の基盤となる生成 AI フレームワークを準備できます。

### 手順 1：ガイドラインの追加

組織のブランド ID の主要な構成要素を設定することは、コンテンツ編集者や共同作業者の作業にとって不可欠な前提条件です。 [ ガイドライン ](./guidelines/overview.md) ロゴ、声のトーン、カラーパレットなど、ブランドの特徴を取り込みます。 [[!DNL Brands]  ガイドライン ](./guidelines/brands.md) ドキュメントをアップロードするか、ブランド情報を手動で入力できます。 [[!DNL Personas]  ガイドライン ](./guidelines/personas.md) と [[!DNL Products]  ガイドライン ](./guidelines/products.md) も重要です。 GenStudio for Performance Marketingの基盤となるジェネレーティブ AI 機能では、これらのガイドラインを使用して、コンテンツの生成をガイドするガードレールを確立します。

#### ガイドライン文書の準備

包括的で焦点を当てた [[!DNL Brands]](./guidelines/brands.md)、[[!DNL Products]](./guidelines/products.md)、[[!DNL Personas]](./guidelines/personas.md) のガイドラインにより、組織のマーケティングキャンペーンの中心的側面が定義されます。 GenStudio for Performance Marketingでは、ブランドの構築を開始するために、これらのガイドラインから情報を抽出します。 ガイドラインのドキュメントをアップロードすることも、GenStudio for Performance Marketingに手動で情報を入力する際に参照することもできます。 この情報をアップロードまたは入力する方法については、[ ガイドラインの追加 ](./guidelines/overview.md) を参照してください。

#### ガイドラインの改訂

GenStudio システムマネージャーは、組織固有のブランド要件を手動で入力またはアップロードすることで、製品の基盤となるジェネレーティブ AI フレームワークを準備できます。 組織のブランドガイドラインの設定は 1 回限りのアクションですが、組織のボラティリティ、成長および市場状況の変化に基づいて、これらのガイドラインを改訂および強化することができます。

### 手順 2:GenStudio [!DNL Brands] 用のAdobe Admin Console プロジェクトの設定

システム管理者は、共同作業者が [!DNL Brands] を編集または作成する前に、追加のセットアップ タスクを完了する必要があります。 Adobe システム管理者は、Adobe Admin Consoleで次のタスクを実行します。

* 資格を編集および作成する必要があるすべてのユーザーを含んだ新しいユーザーグループ [!DNL Brands] 作成します。

* Adobe Admin Consoleで新規プロジェクトを作成します。

[ ブランド権限の割り当て ](configure-brand-permissions.md) を参照してください。

### 手順 3：テンプレートのアップロード

テンプレートを使用すると、コンテンツを迅速に作成できます。 テンプレートには、ヘッダーやフッターなど、承認済みの機能が含まれており、特定のチャネル用に最適化されています。 通常、システムマネージャーは組織のテンプレートをアップロードおよび管理します。 コンテンツエディターは、テンプレートを使用して、組織ブランドの確立された境界内でコンテンツ作成プロセスを開始します。

[ テンプレートの操作 ](./content/use-templates.md) を参照してください。

### 手順 4：承認されたアセットのアップロード

[!DNL Content] の承認済みアセットは、すべてのGenStudio for Performance Marketing エディターが使用できます。 コンテンツエディターが新しいエクスペリ [!DNL Content] ンスやアセットの作成に使用するアセットを、アセットに入力することができます。

[ 承認済みアセットのアップロード ](./content/manage-assets.md) を参照してください。

### 手順 5:Meta （Facebook）アカウントへの接続

GenStudio for Performance Marketingと組織のソーシャルアカウントの間の接続を設定して、アクティブなマーケティングキャンペーン、アセットおよびエクスペリエンスからデータを受け取ります。 [[!DNL Insights]](./insights/overview.md) は、チャネルから派生したデータを分析するツールを提供します。 [Meta （Facebook）アカウントへの接続 ](./insights/connect-channel.md#meta-ads-connect) を参照してください。
