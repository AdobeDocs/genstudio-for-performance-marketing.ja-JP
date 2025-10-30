---
title: Adobe GenStudio for Performance Marketing ユーザーの役割と権限
description: GenStudio for Performance Marketingのユーザーの役割と権限について説明します。
level: Beginner
feature: Generative AI, Guidelines
role: Admin
exl-id: 33ebcf9c-e5f8-4011-b449-5f73d151f221
source-git-commit: 4bef680734ee3369c13b10088fd39f22995a5f0f
workflow-type: tm+mt
source-wordcount: '1123'
ht-degree: 10%

---

# ユーザーの役割と権限

最新のマーケティングキャンペーンを作成してデプロイするには、様々な責任やスキルセットを持つ利害関係者間の共同作業が必要です。 _ユーザーの役割_ は、GenStudio for Performance Marketingの多くの機能への関係者のアクセスを制御します。 割り当てられたユーザーの役割によって、このプラットフォームを使用して実行できるタスクが決まります。 Adobe システム管理者によって、Adobe Admin ConsoleのGenStudio製品プロファイルの役割に割り当てられます。 お知らせメールは、割り当てられた役割を識別します。

>[!NOTE]
>
>これらのロールにユーザーをプロビジョニングする前に、1 回限りの設定タスクを実行できるように、Adobe Admin ConsoleでAdobe システム管理者を指定する必要があります。 このAdobe管理者ロールは、Adobe Admin Consoleのコンテキストでのみ機能します。 GenStudio for Performance Marketingのプラットフォームインターフェイスでは機能しません。 システムマネージャーの権限が必要なAdobe システム管理者は、Adobe Admin ConsoleでGenStudio システムマネージャーとして自分自身をプロビジョニングする必要があります。 [GenStudio for Performance Marketingのプロビジョニング &#x200B;](product-provisioning.md) を参照してください。

## Adobe system administrator とGenStudio system manager の比較

これらのユーザーの役割のタイトルは似ているように見えるかもしれませんが、異なる環境で使用権限を付与する一意の役割を識別します。

**Adobe システム管理者** Adobe Admin Consoleのパワーユーザー権限を持ち、ユーザーの追加や削除などのすべてのユーザー管理タスクを実行します。 このシステム管理者の役割は、GenStudio for Performance Marketing アプリケーションに権限を提供しません。このため、Adobe システム管理者はGenStudioのライセンスを必要としません。 Adobe システム管理者は、通常、Admin Consoleを使用して、GenStudio デプロイメントのユーザーアカウントを追加および削除し、個々のユーザーまたはユーザーグループに対する使用権限や権限を割り当てまたは削除します。

**GenStudio システムマネージャー** は、GenStudio for Performance Marketing内のパワーユーザーですが、Adobe Admin Consoleでタスクを実行する権限はありません。 この System Manager の役割にはGenStudio製品ライセンスが必要で、[Adobe GenStudio for Performance Marketing製品の説明 &#x200B;](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html) のパワーユーザーに対応しています。 GenStudio システムマネージャーは、[!DNL Brands] 成、[!DNL Persona] 除、[!DNL Product] ージの作成、削除、更新、公開など、GenStudio for Performance Marketingの機能を完全に利用できます。 [Adobe GenStudio for Performance Marketing製品説明 &#x200B;](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html) では、GenStudioのユーザーロールと製品ライセンスとの関係を説明します。

[&#x200B; エンタープライズおよびチーム管理ガイド &#x200B;](https://helpx.adobe.com/enterprise/using/admin-roles.html#enterprise) の _管理者の役割_ を参照してください。

## 使用権限

_使用権限_ 特定のタスクを実行する権限と保護されたリソースにアクセスする権限を付与します。 エンタイトルメント（権限）は、製品プロファイル内のユーザーの役割で定義され、ユーザーはその役割に割り当てられると、これらのエンタイトルメントを受け取ります。

>[!IMPORTANT]
>
>既存の製品プロファイルを新規作成したり、編集または削除したりしないでください。 デフォルトの製品プロファイルを変更すると、GenStudio for Performance Marketingのデプロイメントが大幅に中断する可能性があります。

## ユーザーの役割

このような様々な組織的な役割をサポートするのは、GenStudio for Performance Marketingの 3 種類のユーザーの役割です。 使用権限は、これらの各ユーザータイプに合わせて調整され、マーケティング組織での各ユーザーの責任をサポートします。 次の 3 つのユーザーの役割タイプがあります。

* **GenStudio エディター** GenStudio for Performance Marketingの生成 AI 機能を使用して、マーケティングキャンペーンアセットを作成し、コンテンツのレビューと承認をリクエストし、このコンテンツの承認済みドラフトを公開します。 すべてのGenStudio for Performance Marketing ユーザーは、エディターがアセットを [!DNL Content] に保存すると、アセットにアクセスして使用できます。 GenStudio エディターは、GenStudio for Performance Marketingのパワーユーザーです。

* **GenStudio共同作業者** は、GenStudio for Performance Marketingのユーザーの中で最も幅広い範囲です。 共同作業者は、コンテンツを表示および承認できます。共同作業者は、生成するコンテンツが組織のニーズと標準に一致することを確認するワークフローの重要な役割を果たします。 GenStudio共同作業者は、GenStudio for Performance Marketingの _共同作業者ユーザー_ です。

* **GenStudio システムマネージャー** は、GenStudio for Performance Marketing内で最も幅広い使用権限または権限を持っています。 システムマネージャーは、キャンペーンアセットの作成とデプロイメントのための基本的なガードレールの確立という、基本的なオンボーディングタスクを実行します。 システムマネージャーは、ブランドや組織固有の情報（[&#x200B; ブランドガイドライン &#x200B;](./guidelines/overview.md) などをアップロードして、これらのガードレールを実装します。 システムマネージャーには、[!DNL Brands] ータを作成して公開する権限がありますが、ユーザー管理権限はありません。 GenStudio システムマネージャーは、GenStudio for Performance Marketingのパワーユーザーです。

### GenStudio エディター

_編集者_ またはコンテンツ作成者は、GenStudio for Performance Marketing [!DNL Brands]、[!DNL Campaigns] および [!DNL Content] アセットの作成に必要なコア権限を持っています。 これらのパワーユーザーは、作成したアセットを編集および削除することもできます。 GenStudio for Performance Marketingでは、数百ものコンテンツをすばやく作成することができます。 これらのユーザーは、特定のマーケティングキャンペーンのニーズを満たすために、承認済みのコンテンツの個別の部分を調整するコンテンツフラグメントまたはエクスペリエンス全体を生成できます。

編集者は、_プロンプト_ を通じてGenStudio for Performance Marketingの生成 AI テクノロジーとやり取りします。 キャンバスのプロンプトドロワーには、特定のキャンペーンのガイドラインのコンテキストでプロンプトを配置するツールが用意されています。 その結果、生成されるコンテンツの品質と成功は、組織がアップロードしたブランドガイドラインの品質と、プロンプトの特異性に部分的に依存します。 [&#x200B; 有効なプロンプトの記述 &#x200B;](effective-prompts.md) を参照してください。

エディターのデフォルトの権限を次の表に示します。

| 機能 | 作成 | アップデート | 削除 | 表示 |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | いいえ | いいえ | いいえ | はい |
| [!DNL Campaigns] | はい | はい | はい | はい |
| [!DNL Content] | はい | はい | はい | はい |
| [!DNL Create] | はい | はい | はい | はい |
| [!DNL Insights] | コネクタのみを設定できます |    |     | はい |
| [!DNL Personas] | はい | はい | はい | はい |
| [!DNL Products] | はい | はい | はい | はい |
| [!DNL Reviews and approvals] | はい | はい | はい | はい |
| [!DNL Templates] | いいえ | いいえ | いいえ | はい |

GenStudioのシステムマネージャーは、エディターに [!DNL Brand] ージの編集および削除権限を付与できます。

### GenStudio共同作業者

_共同作業者_ は、GenStudio for Performance Marketingでアセットを表示できますが、作成、編集、削除はできません。 例えば、共同作業者がコンテンツにアクセスしようとすると、「*このコンテンツへのアクセス権がありません*」というメッセージが表示さ [[!DNL Create]](/help/user-guide/create/overview.md) ます。

共同作業者には、コンテンツのレビューと承認のプロセスを成功させるために不可欠な関係者で、コンテンツを作成する必要がない人や、直接編集する必要がない人が含まれます。 クリエイティブの法務エキスパートやマネージャーは、潜在的な共同作業者の例です。 GenStudio for Performance Marketingの共同作業者には、他のCreative Cloud製品のアセットを作成および表示する権限が付与されている場合があります。

次の表に、デフォルトのコラボレータ権限を示します。

| 機能 | 作成 | アップデート | 削除 | 表示 |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | いいえ | いいえ | いいえ | はい |
| [!DNL Campaigns] | はい | はい | はい | はい |
| [!DNL Content] | いいえ | いいえ | いいえ | はい |
| [!DNL Create] | いいえ | いいえ | いいえ | はい |
| [!DNL Insights] | いいえ | いいえ | いいえ | はい |
| [!DNL Personas] | はい | はい | はい | はい |
| [!DNL Products] | はい | はい | はい | はい |
| [!DNL Reviews and approvals] | いいえ | いいえ | いいえ | はい |
| [!DNL Templates] | いいえ | いいえ | いいえ | はい |

### GenStudio システムマネージャー

_GenStudio システムマネージャー_ は、GenStudio for Performance Marketing内で最も強力な権限セットを持っています。 これらのパワーユーザーは、キャンペーンアセットの作成とデプロイメントのための基本的なガードレールの確立という、基本的なオンボーディングタスクを実行します。 システムマネージャーは、ブランドや組織固有の情報（[&#x200B; ブランドガイドライン &#x200B;](./guidelines/overview.md) などをアップロードして、これらのガードレールを実装します。 システムマネージャーには、[!DNL Brands] ータを作成して公開する権限がありますが、ユーザー管理権限はありません。

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
| [!DNL Templates] | はい | はい | はい | はい |

システムマネージャーはテンプレートをアップロードすることもできます。

事前の設定作業の概要については、[Adobe GenStudio for Performance Marketingの基本を学ぶ &#x200B;](get-started.md) を参照してください。
