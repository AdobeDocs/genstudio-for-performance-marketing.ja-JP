---
title: Adobe GenStudio for Performance Marketing ユーザーの役割と権限
description: GenStudio for Performance Marketingのユーザーの役割と権限について説明します。
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
source-git-commit: 3e9a2a4f42ba79389691705c571bf6bbd0b990c5
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 12%

---

# ユーザーの役割と権限

最新のマーケティングキャンペーンを作成してデプロイするには、様々な責任やスキルセットを持つ利害関係者間の共同作業が必要です。 _ユーザーの役割_ は、GenStudio for Performance Marketingの多くの機能への関係者のアクセスを制御します。 割り当てられたユーザーの役割によって、このプラットフォームを使用して実行できるタスクが決まります。 Adobeシステム管理者によって、Adobe Admin ConsoleのGenStudio製品プロファイルの役割が割り当てられます。 お知らせメールは、割り当てられた役割を識別します。

>[!NOTE]
>
>これらのロールにユーザーをプロビジョニングする前に、Adobe Admin ConsoleでAdobeシステム管理者を指定して、1 回限りの設定タスクを実行する必要があります。 このAdobe管理者ロールは、Adobe Admin Consoleのコンテキストでのみ機能します。 GenStudio for Performance Marketingのプラットフォームインターフェイスでは機能しません。 Adobe管理者の権限が必要なシステムシステム管理者は、Adobe Admin ConsoleでGenStudio システムマネージャーとして自分自身をプロビジョニングする必要があります。 [GenStudio for Performance Marketingのプロビジョニング ](product-provisioning.md) を参照してください。

## 使用権限

_使用権限_ 特定のタスクを実行する権限と保護されたリソースにアクセスする権限を付与します。 エンタイトルメントは、製品プロファイル内のユーザーの役割で定義され、ユーザーはその役割に割り当てられると、これらのエンタイトルメントを受け取ります。

## ユーザーの役割

このような様々な組織的な役割をサポートするのは、GenStudio for Performance Marketingの 3 種類のユーザーの役割です。 権限は、これらの各ユーザータイプに合わせて調整され、マーケティング組織での各ユーザーの責任をサポートします。 次の 3 つのユーザーの役割タイプがあります。

* **GenStudio エディター** GenStudio for Performance Marketingの生成 AI 機能を使用して、マーケティングキャンペーンアセットを作成し、コンテンツのレビューと承認をリクエストし、このコンテンツの承認済みドラフトを公開します。 すべてのGenStudio for Performance Marketing ユーザーは、エディターがアセットを [!DNL Content] に保存すると、アセットにアクセスして使用できます。

* **GenStudio共同作業者** は、GenStudio for Performance Marketingのユーザーの中で最も幅広い範囲です。 共同作業者は、コンテンツを表示および承認できます。共同作業者は、生成するコンテンツが組織のニーズと標準に一致することを確認するワークフローの重要な役割を果たします。

* **GenStudio システムマネージャー** は、GenStudio for Performance Marketing内で最も広範な権限を持っています。 システムマネージャーは、キャンペーンアセットの作成とデプロイメントのための基本的なガードレールの確立という、基本的なオンボーディングタスクを実行します。 システムマネージャーは、ブランドや組織固有の情報（[ ブランドガイドライン ](./guidelines/overview.md) などをアップロードして、これらのガードレールを実装します。 システムマネージャーには、[!DNL Brands] ータを作成して公開する権限がありますが、ユーザー管理権限はありません。

### GenStudio エディター

_編集者_ またはコンテンツ作成者は、GenStudio for Performance Marketing [!DNL Brands]、[!DNL Campaigns] および [!DNL Content] アセットの作成に必要なコア権限を持っています。 また、作成したアセットを編集および削除することもできます。 GenStudio for Performance Marketingでは、数百ものコンテンツをすばやく作成することができます。 これらのユーザーは、特定のマーケティングキャンペーンのニーズを満たすために、承認済みのコンテンツの個別の部分を調整するコンテンツフラグメントまたはエクスペリエンス全体を生成できます。

編集者は、_プロンプト_ を通じてGenStudio for Performance Marketingの生成 AI テクノロジーとやり取りします。 キャンバスのプロンプトドロワーには、特定のキャンペーンのガイドラインのコンテキストでプロンプトを配置するツールが用意されています。 その結果、生成されるコンテンツの品質と成功は、組織がアップロードしたブランドガイドラインの品質と、プロンプトの特異性に部分的に依存します。 [ 有効なプロンプトの記述 ](effective-prompts.md) を参照してください。

エディターのデフォルトの権限を次の表に示します。

| 機能 | 作成 | アップデート | 削除 | 表示 |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | いいえ | いいえ | いいえ | はい |
| [!DNL Campaigns] | はい | はい | はい | はい |
| [!DNL Content] | はい | はい | はい | はい |
| [!DNL Create] | はい | はい | はい | はい |
| [!DNL Insights] | ad コネクタのみを設定できます |    |     | はい |
| [!DNL Personas] | はい | はい* | はい* | はい |
| [!DNL Products] | はい | はい* | はい* | はい |
| [!DNL Reviews and approvals] | はい | はい | はい | はい |

編集者は、自分が作成した [!DNL Personas] と [!DNL Products] を編集および削除できます。

GenStudioのシステムマネージャーは、エディターに [!DNL Brand] ージの編集および削除権限を付与できます。

### GenStudio共同作業者

_共同作業者_ は、GenStudio for Performance Marketingでアセットを表示できますが、作成、編集、削除はできません。 共同作業者には、コンテンツのレビューと承認のプロセスを成功させるために不可欠な関係者で、コンテンツを作成する必要がない人や、直接編集する必要がない人が含まれます。 クリエイティブの法務エキスパートやマネージャーは、潜在的な共同作業者の例です。 GenStudio for Performance Marketingの共同作業者には、他のCreative Cloud製品のアセットを作成および表示する権限が付与されている場合があります。

次の表に、デフォルトのコラボレータ権限を示します。

| 機能 | 作成 | アップデート | 削除 | 表示 |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | いいえ | いいえ | いいえ | はい |
| [!DNL Campaigns] | いいえ | いいえ | いいえ | はい |
| [!DNL Content] | いいえ | いいえ | いいえ | はい |
| [!DNL Create] | いいえ | いいえ | いいえ | はい |
| [!DNL Insights] | いいえ | いいえ | いいえ | はい |
| [!DNL Personas] | いいえ | いいえ | いいえ | はい |
| [!DNL Products] | いいえ | いいえ | いいえ | はい |
| [!DNL Reviews and approvals] | いいえ | いいえ | いいえ | はい |

### GenStudio システムマネージャー

_GenStudio システムマネージャー_ は、GenStudio for Performance Marketing内で最も強力な権限セットを持っています。 システムマネージャーは、キャンペーンアセットの作成とデプロイメントのための基本的なガードレールの確立という、基本的なオンボーディングタスクを実行します。 システムマネージャーは、ブランドや組織固有の情報（[ ブランドガイドライン ](./guidelines/overview.md) などをアップロードして、これらのガードレールを実装します。 システムマネージャーには、[!DNL Brands] ータを作成して公開する権限がありますが、ユーザー管理権限はありません。

次の表に、デフォルトのシステムマネージャー権限を示します。

| 機能 | 作成 | アップデート | 削除 | 表示 |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | はい | はい | はい | はい |
| [!DNL Campaigns] | はい | はい | はい | はい |
| [!DNL Content] | はい | はい | はい | はい |
| [!DNL Insights] | はい | はい | はい | はい |
| [!DNL Personas] | はい | はい | はい | はい |
| [!DNL Products] | はい | はい | はい | はい |
| [!DNL Reviews and approvals] | はい | はい | はい | はい |

事前の設定作業の概要については、[Adobe GenStudio for Performance Marketingの基本を学ぶ ](get-started.md) を参照してください。