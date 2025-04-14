---
title: Adobe GenStudio for Performance Marketingの概要
description: パフォーマンスマーケティング用の GenStudio の使用を開始して、ブランドに合わせた新しいマーケティングコンテンツを生成する方法について説明します。
level: Beginner
role: User
feature: Media Templates, Guidelines, Generative AI
exl-id: bcb03198-bbcb-45ae-af01-25c1e834b563
source-git-commit: ac166245f5358c3bd050227b3ba9c53caa0e3622
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 2%

---

# Adobe GenStudio for Performance Marketingの概要

Adobe GenStudio for Performance Marketingは、コンテンツの作成、管理、分析を合理化するように設計された包括的なツールスイートを提供します。 内容作成ライフサイクルに、内容の作成、レビュー、共有、分析の方法を変革するジェネレーティブ マーケティング AI 機能が組み込まれています。

## 内容の作成、共有、レビュー開始

ジェネレーティブ AI ベースのツールを初めて使用する場合、または単に GenStudio for Performance Marketing のコア原則に興味がある場合は、「 [概念](concepts.md) および [効果的なプロンプトの作成](effective-prompts.md)を参照してください。 クリエイティブプロセスでのジェネレーティブAIテクノロジーの使用に関するAdobe Systemsのオンライン学習プラットフォームである [Adobe Systems GenStudio Academy](https://learningmanager.adobe.com/genstudioacademy)をご覧ください。

## パフォーマンスマーケティングのためのGenStudioのトレーニング

パフォーマンスマーケティングのためのGenStudioは、ブランドと市場に関する情報を使用して、ブランドに準拠した内容の作成を強化します。 トレーニング資料には、例、顧客 [ペルソナ](/help/user-guide/guidelines/personas.md) と [製品](/help/user-guide/guidelines/products.md)の説明、および [ブランドガイドライン](/help/user-guide/guidelines/overview.md)が含まれています。

システム管理者はAdobe Systems組織固有の情報を入力またはアップロードすることにより、パフォーマンスマーケティング用にGenStudioをセットアップします。 この準備により、コンテンツ編集者と共同作業者が生成 AI 機能を効果的に使用して、キャンペーンアセットを作成およびレビューできるようになります。 Adobe システム管理者が組織の製品インスタンスをプロビジョニングし、GenStudio システムマネージャーの権限を割り当てると、GenStudio システムマネージャーはガイドラインを使用して製品の基盤となる生成 AI フレームワークを準備できます。

### 手順 1：ガイドラインの追加

組織のブランド ID の主要な構成要素を設定することは、コンテンツ編集者や共同作業者の作業にとって不可欠な前提条件です。 [ ガイドライン ](./guidelines/overview.md) ロゴ、声のトーン、カラーパレットなど、ブランドの特徴を取り込みます。 [[!DNL Brands]  ガイドライン ](./guidelines/brands.md) ドキュメントをアップロードするか、ブランド情報を手動で入力できます。 [[!DNL Personas]  ガイドライン ](./guidelines/personas.md) と [[!DNL Products]  ガイドライン ](./guidelines/products.md) も重要です。 GenStudio for Performance Marketingの基盤となるジェネレーティブAI機能は、これらのガイドラインを使用して、内容世代ガイドガードレールを確立します。

#### ガイドラインドキュメントを準備する

包括的で焦点を絞った [[!DNL Brands]](./guidelines/brands.md)、 [[!DNL Products]](./guidelines/products.md)、および [[!DNL Personas]](./guidelines/personas.md) ガイドラインは、組織のマーケティングキャンペーンの中核的な側面を定義します。 パフォーマンスマーケティングのためのGenStudioは、これらのガイドラインから情報を抽出して、ブランドの構築を開始します。 ガイドラインドキュメントアップロードしたり、パフォーマンスマーケティングのためにGenStudioに手動で情報を入力するときに参照したりできます。 この情報のアップロードまたは入力に関するガイダンスについては [追加ガイドライン](./guidelines/overview.md) を参照してください。

#### ガイドラインの改訂

GenStudio システムマネージャーは、組織固有のブランド要件を手動で入力またはアップロードすることで、製品の基盤となるジェネレーティブ AI フレームワークを準備できます。 組織のブランド ガイドラインの設定は 1 回限りのアクションですが、組織の変動性、成長、および変化するマーケット状況に基づいて、これらのガイドラインを改訂および強化できます。

### 手順 2:GenStudio [!DNL Brands] 用のAdobe Admin Console プロジェクトの設定

システム管理者は、共同作業者が [!DNL Brands] を編集または作成する前に、追加のセットアップ タスクを完了する必要があります。 Adobe システム管理者は、Adobe Admin Consoleで次のタスクを実行します。

* 資格を編集および作成する必要があるすべてのユーザーを含んだ新しいユーザーグループ [!DNL Brands] 作成します。

* Adobe Admin Consoleで新規プロジェクトを作成します。

[ブランド権限の割り当て](configure-brand-permissions.md)を参照してください。

### 手順 3:テンプレートのアップロード

テンプレート内容作成を加速します。 テンプレートには、ヘッダーやフッターなどの承認済みの機能が含まれ、特定のチャネル用に最適化されています。 システム管理者は通常、組織のテンプレートアップロードおよび管理します。 コンテンツ編集者は、テンプレートを使用して、組織ブランドの確立された境界内で内容作成プロセスをジャンプ開始します。

詳しくは [テンプレートの操作](./content/use-templates.md)を参照してください。

### 手順 4：承認されたアセットのアップロード

[!DNL Content] の承認済みアセットは、すべてのGenStudio for Performance Marketing エディターが使用できます。 コンテンツエディターが新しいエクスペリ [!DNL Content] ンスやアセットの作成に使用するアセットを、アセットに入力することができます。

[ 承認済みアセットのアップロード ](./content/manage-assets.md) を参照してください。

### 手順 5:Meta （Facebook）アカウントへの接続

GenStudio for Performance Marketingと組織のソーシャルアカウントの間の接続を設定して、アクティブなマーケティングキャンペーン、アセットおよびエクスペリエンスからデータを受け取ります。 [!DNL Insights] チャネル派生データを分析するためのツールを提供します。 [メタに接続(Facebook)アカウント](/help/user-guide/connectors/connect-channel.md#meta-ads-connect)を参照してください。
