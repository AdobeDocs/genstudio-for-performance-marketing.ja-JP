---
title: Adobe GenStudio for Performance Marketingの概要
description: GenStudio for Performance Marketingを設定して、ブランドに合わせた新しいマーケティングコンテンツを生成する方法を説明します。
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: bcb03198-bbcb-45ae-af01-25c1e834b563
source-git-commit: ce08231cb723bec3d80a732837b72a435d3b552d
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 8%

---

# Adobe GenStudio for Performance Marketingの概要

Adobe GenStudio for Performance Marketingは、ブランドアイデンティティを反映し遵守するマーケティングエクスペリエンスを作成、評価および管理するための包括的なプラットフォームです。

関係者のその多くの機能へのアクセスは、割り当てられた _ユーザーの役割_ によって制御されます。 割り当てられたユーザーの役割によって、GenStudio for Performance Marketing内で実行できるタスクが決まります。 Adobeシステム管理者は、Adobe Admin ConsoleのGenStudio for Performance Marketing製品プロファイルで権限を割り当てます。 お知らせメールは、割り当てられた役割を識別します。

ジェネレーティブ AI ベースのツールを初めて使用する場合、またはGenStudio for Performance Marketingの基本原則に興味がある場合は、[ 概念 ](concepts.md) および [ 効果的なプロンプトの記述 ](effective-prompts.md) を参照してください。

## ユーザーの役割

最新のマーケティングキャンペーンを作成してデプロイするには、様々な責任やスキルセットを持つ利害関係者間の共同作業が必要です。

このような様々な組織的な役割をサポートするのは、GenStudio for Performance Marketingの 3 種類のユーザーの役割です。 権限は、これらの各ユーザータイプに合わせて調整され、マーケティング組織での各ユーザーの責任をサポートします。

**次の 3 つのユーザーロールタイプがあります**。

* **エディター** GenStudio for Performance Marketingの生成 AI 機能を使用して、マーケティングキャンペーンアセットを作成し、コンテンツのレビューと承認をリクエストし、このコンテンツの承認済みドラフトを公開します。 作成者がアセットをコンテンツに保存すると、すべてのGenStudio for Performance Marketing ユーザーがアセットにアクセスして使用できます。

* **共同作業者** は、GenStudio for Performance Marketingのユーザーの中で最も幅広い範囲です。 共同作業者は、コンテンツを表示および承認できます。共同作業者は、生成するコンテンツが組織のニーズと標準に一致することを確認するワークフローの重要な役割を果たします。

* **システムマネージャー** は、GenStudio for Performance Marketing内で最も広範な権限を持っています。 システムマネージャーは、キャンペーンアセットの作成とデプロイメントのための基本的なガードレールの確立という、基本的なオンボーディングタスクを実行します。 システムマネージャーは、ブランドや組織固有の情報（[ ブランドガイドライン ](/help/user-guide/guidelines/overview.md) などをアップロードして、これらのガードレールを実装します。 GenStudio for Performance Marketing システムマネージャーは、ブランドを作成して公開する権限を持っていますが、ユーザー管理者権限はありません。

>[!NOTE]
>これらのロールにユーザーをプロビジョニングする前に、Adobe Admin ConsoleでAdobeシステム管理者を指定して、1 回限りの設定タスクを実行する必要があります。 このAdobe管理者ロールは、Adobe Admin Consoleのコンテキストでのみ機能します。 GenStudio for Performance Marketingのプラットフォームインターフェイスでは機能しません。

### GenStudio for Performance Marketing エディター

**エディター** は、GenStudio for Performance Marketing [!DNL Brands]、[!DNL Campaigns] および [!DNL Content] アセットを作成するために必要なコア権限を持っています。 また、作成したアセットを編集および削除することもできます。 GenStudio for Performance Marketingでは、数百ものコンテンツをすばやく作成することができます。 これらのユーザーは、特定のマーケティングキャンペーンのニーズを満たすために、承認済みのコンテンツの個別の部分を調整するコンテンツセクションまたはエクスペリエンス全体を生成できます。

編集者は、_プロンプト_ を通じてGenStudio for Performance Marketingの生成 AI テクノロジーとやり取りします。 キャンバスのプロンプト領域には、特定のキャンペーンのガイドラインのコンテキストでプロンプトを配置するツールが用意されています。 その結果、生成されるコンテンツの品質と成功は、組織がアップロードしたブランドガイドラインの品質と、プロンプトの特異性に部分的に依存します。

[ 有効なプロンプトの記述 ](effective-prompts.md) を参照してください。

エディターのデフォルトの権限を次の表に示します。

| 機能 | 作成 | アップデート | 削除 | 表示 |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | いいえ | いいえ | いいえ | はい |
| [!DNL Campaigns] | はい | はい | はい | はい |
| [!DNL Content] | はい | はい | はい | はい |
| [!DNL Insights] | ad コネクタのみを設定できます |    |     | はい |
| [!DNL Personas] | はい | はい | はい | はい |
| [!DNL Products] | はい | はい | はい | はい |
| [!DNL Reviews and approvals] | はい | はい | はい | はい |

### GenStudio for Performance Marketing共同作業者

**共同作業者** は、GenStudio for Performance Marketingでアセットを表示できますが、作成、編集、削除はできません。 共同作業者には、コンテンツのレビューと承認のプロセスを成功させるために不可欠な関係者で、コンテンツを作成する必要がない人や、直接編集する必要がない人が含まれます。 法律専門家やクリエイターのマネージャーは、潜在的な共同作業者の例です。 GenStudio for Performance Marketingの共同作業者には、他のCreative Cloud製品のアセットを作成および表示する権限がある場合があります。

次の表に、デフォルトのコラボレータ権限を示します。

| 機能 | 作成 | アップデート | 削除 | 表示 |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | いいえ | いいえ | いいえ | はい |
| [!DNL Campaigns] | いいえ | いいえ | いいえ | はい |
| [!DNL Content] | いいえ | いいえ | いいえ | はい |
| [!DNL Insights] | いいえ | いいえ | いいえ | はい |
| [!DNL Personas] | いいえ | いいえ | いいえ | はい |
| [!DNL Products] | いいえ | いいえ | いいえ | はい |
| [!DNL Reviews and approvals] | いいえ | いいえ | いいえ | はい |

### GenStudio for Performance Marketing システムマネージャー

**GenStudio システムマネージャー** GenStudio for Performance Marketingをデプロイするための初期作業を行います。

次の表に、GenStudio for Performance Marketing system manager のデフォルトの権限を示します。

| 機能 | 作成 | アップデート | 削除 | 表示 |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | はい | はい | はい | はい |
| [!DNL Campaigns] | はい | はい | はい | はい |
| [!DNL Content] | はい | はい | はい | はい |
| [!DNL Insights] | はい | はい | はい | はい |
| [!DNL Personas] | はい | はい | はい | はい |
| [!DNL Products] | はい | はい | はい | はい |
| [!DNL Reviews and approvals] | はい | はい | はい | はい |


## コンテンツを生成するためのGenStudio for Performance Marketingの準備

GenStudio for Performance Marketing システムマネージャーは、編集者と共同作業者がキャンペーンアセットを作成できるように、組織のGenStudio for Performance Marketing環境を準備します。 これらの準備的なセットアップ作業には、次のものが含まれます。

1. [!DNL Brands]、[!DNL Products] および [!DNL Personas] に関する [ ガイドラインを追加 ](./guidelines/overview.md) します。 組織のブランドアイデンティティの主要な構成要素を設定することは、クリエイターや共同作業者の作業に不可欠な前提条件です。 ブランドガイドラインドキュメントをアップロードするか、ブランド情報を手動で入力できます。
   * **ガイドラインのドキュメントを準備します**。 ブランドガイドラインが説明的で包括的であればあるほど、出力は良くなります。 ブランドに不可欠と考えられる機能の簡単な例を含め、コンテンツの作成から除外する行動の説明を追加します。 GenStudio for Performance Marketingは、アップロードされたこれらのドキュメントから情報を抽出し、ブランドの構築を開始します。 GenStudio for Performance Marketingがアップロードされたドキュメントから各ガイドラインを組み立てると、ブランドボイス、チャネル、画像ガイドラインなどの情報が入力されます。
   * **必要に応じて、ブランドガイドラインフィールドを編集または入力** します。 包括的なブランドガイドラインは、組織のブランドをGenStudio for Performance Marketingで理解するための基礎となります。 GenStudio for Performance Marketingがブランドガイドラインドキュメントから必要な情報を抽出したら、抽出した情報のフィールドを手動で編集または入力するよう求められます。 コンテン [!DNL Product] を追加して、コンテンツ作成の個々の製品フォーカス領域を指定します。 [!DNL Personas] のガイドラインは、定義された顧客セグメント向けにコンテンツを作成する際の調整に役立ちます。

   組織のブランドガイドラインの設定は 1 回限りのアクションですが、組織のボラティリティ、成長および市場状況の変化に基づいて、これらのガイドラインを改訂および強化する必要が生じる場合があります。

1. **[テンプレートのアップロード](./content/use-templates.md)**. テンプレートにはショートカットが用意されており、コンテンツを短時間で作成できます。 テンプレートには、ヘッダーやフッターなどの承認済み機能が含まれており、コンテンツを作成するためのガードレールを設定します。 通常、システムマネージャーは組織のテンプレートをアップロードおよび管理します。 作成者は、テンプレートを使用して、組織ブランドの確立された境界内でコンテンツ作成プロセスを素早く開始します。

1. **[承認済みアセットのアップロード](./content/manage-assets.md)**. [!DNL Content] の承認済みアセットは、すべてのGenStudio for Performance Marketing作成者が使用できます。 作成者が新しいエクスペリエンスやアセットの作成に使用できるアセットで [!DNL Content] ーザーをシードすることができます。

1. **[Meta （Facebook）アカウントへの接続](./insights/connect-channel.md)**。 GenStudio for Performance Marketingと組織のソーシャルアカウントの間の接続を設定して、アクティブなマーケティングキャンペーン、アセットおよびエクスペリエンスからデータを受け取ります。 [[!DNL Insights]](./insights/overview.md) は、チャネルから派生したデータを分析するツールを提供します。
