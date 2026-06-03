---
title: Adobe GenStudio for Performance Marketingのユーザーの役割と権限
description: GenStudio for Performance Marketingのユーザーの役割と権限について説明します。
level: Beginner
feature: Generative AI, Guidelines
role: Admin
exl-id: 33ebcf9c-e5f8-4011-b449-5f73d151f221
TQID: https://experienceleague.adobe.com/H1MbYm5RniRbZBous-F4nBi-2h5RD1AG4IgydlP22-c
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 1155
ht-degree: 10%

---

# ユーザーの役割と権限

最新のマーケティングキャンペーンを構築、展開するには、さまざまな責任とスキルセットを持つ関係者の間でのコラボレーションが必要です。 _ユーザーの役割_&#x200B;は、GenStudio for Performance Marketingのさまざまな機能への関係者のアクセスを制御します。 割り当てられたユーザーの役割によって、このプラットフォームを使用して実行できるタスクが決まります。 Adobe システム管理者は、Adobe Admin ConsoleのGenStudio製品プロファイルのロールにあなたを割り当てます。 割り当てられた役割がウェルカムメールに記載されます。

>[!NOTE]
>
>ユーザーがこれらのロールにプロビジョニングされる前に、Adobe Admin ConsoleでAdobe システム管理者を指定して、1回限りのセットアップ タスクを実行する必要があります。 このAdobe管理者ロールは、Adobe Admin Consoleのコンテキストでのみ機能します。 GenStudio for Performance Marketingのプラットフォームインターフェイスでは役割を果たしません。 System managerの使用権限を必要とするAdobe システム管理者は、Adobe Admin ConsoleでGenStudio system managerとしてプロビジョニングする必要があります。 [GenStudio for Performance Marketingのプロビジョニング &#x200B;](product-provisioning.md)を参照してください。

## Adobe system administratorとGenStudio system managerの比較

これらのユーザーロールのタイトルは類似しているように思えるかもしれませんが、異なる環境で使用権限を提供する独自の役割を特定しています。

**Adobe system administrators**&#x200B;は、Adobe Admin Consoleでpower user権限を持ち、ユーザーの追加や削除など、すべてのユーザー管理タスクを実行します。 このシステム管理者ロールは、GenStudio for Performance Marketing アプリケーションで権限を提供しません。これは、Adobe システム管理者がGenStudioのライセンスを必要としない理由です。 Adobe システム管理者は通常、Admin Consoleを使用して、GenStudio デプロイメントからユーザーアカウントを追加および削除し、個々のユーザーまたはユーザーグループから使用権限または権限を割り当てまたは削除します。

**GenStudio system manager**&#x200B;は、GenStudio for Performance Marketing内のパワーユーザーですが、Adobe Admin Consoleでタスクを実行する権限はありません。 このSystem Manager ロールにはGenStudio製品ライセンスが必要で、[Adobe GenStudio for Performance Marketing製品説明](https://helpx.adobe.com/jp/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html)のPower Userに対応しています。 GenStudioのシステムマネージャーは、[!DNL Brands]、[!DNL Persona]、[!DNL Product]の作成、削除、更新、公開など、GenStudio for Performance Marketingの機能に対する完全な使用権限を持っています。 [Adobe GenStudio for Performance Marketing製品の説明](https://helpx.adobe.com/jp/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html)では、GenStudio ユーザーロールが製品ライセンスにどのように関連しているかを説明しています。

_エンタープライズおよびTeams管理ガイド_&#x200B;の[管理ロール &#x200B;](https://helpx.adobe.com/jp/enterprise/using/admin-roles.html#enterprise)を参照してください。

## 使用権限

_使用権限_&#x200B;は、特定のタスクを実行し、保護されたリソースにアクセスする権限を付与します。 使用権限（権限）は、製品プロファイル内のユーザーの役割で定義され、ユーザーはその役割に割り当てられたときに、これらの使用権限を受け取ります。

>[!IMPORTANT]
>
>既存の製品プロファイルを新規に追加したり、編集または削除したりしないでください。 デフォルトの製品プロファイルを変更すると、GenStudio for Performance Marketingのデプロイメントが大幅に中断される可能性があります。

## ユーザーの役割

GenStudio for Performance Marketingのユーザーロールには、次の3つのタイプがあります。 権限は、これらの各ユーザータイプに合わせて調整され、マーケティング組織における各ユーザーの責任をサポートします。 ユーザーの役割には、次の3つのタイプがあります。

* **GenStudio エディター**&#x200B;は、GenStudio for Performance Marketingの生成AI機能を使用して、マーケティングキャンペーンアセットを作成し、コンテンツのレビューと承認をリクエストし、このコンテンツの承認済みドラフトを公開します。 エディターがアセットを[!DNL Content]に保存すると、すべてのGenStudio for Performance Marketing ユーザーがアセットにアクセスして使用できます。 GenStudio エディターはGenStudio for Performance Marketingのパワーユーザーです。

* **GenStudioの共同作業者**&#x200B;は、最も幅広いGenStudio for Performance Marketing ユーザーです。 共同作業者はコンテンツを表示して承認することができ、生成するコンテンツが組織のニーズや基準に合致するようにするためのワークフローの重要な部分です。 GenStudioの共同作業者は、GenStudio for Performance Marketingの&#x200B;_共同作業者ユーザー_&#x200B;です。

* **GenStudio システムマネージャー**&#x200B;は、GenStudio for Performance Marketing内で最も幅広い使用権限または権限を持っています。 システムマネージャーは、キャンペーンアセットの制作と展開に関する基本的なガードレールを確立するという、オンボーディングの重要なタスクを実行します。 システムマネージャーは、[&#x200B; ブランドガイドライン &#x200B;](./guidelines/overview.md)などのブランドおよび組織固有の情報をアップロードすることで、これらのガードレールを実装します。 システム マネージャーには[!DNL Brands]を作成および公開する権限がありますが、ユーザー管理権限はありません。 GenStudioのシステムマネージャーは、GenStudio for Performance Marketingのパワーユーザーです。

### GenStudio エディター

_エディター_&#x200B;またはコンテンツ作成者には、GenStudio for Performance Marketing [!DNL Brands]、[!DNL Campaigns]および[!DNL Content]のアセットを作成するために必要なコア権限があります。 パワーユーザーは、作成したアセットを編集したり削除したりすることもできます。 GenStudio for Performance Marketingでは、数百ものコンテンツをすばやく制作できます。 こうした利用者は、コンテンツフラグメントやエクスペリエンス全体を生成して、特定のマーケティングキャンペーンのニーズに対応する、承認済みコンテンツの個別の要素を調整することができます。

編集者は、_プロンプト_&#x200B;を通じてGenStudio for Performance Marketingの生成AI テクノロジーを操作します。 カンバスのプロンプトドロワーには、特定のキャンペーンのガイドラインのコンテキストにプロンプトを配置するツールが用意されています。 その結果、生成されたコンテンツの品質と成功は、一部は、組織がアップロードしたブランドガイドラインの品質とプロンプトの特異性に依存します。 [効果的なプロンプトの作成](effective-prompts.md)を参照してください。

次の表に、デフォルトのエディター権限を示します。

| 機能 | 作成 | 更新 | 削除 | 表示 |
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

GenStudio システム マネージャーは、エディターに[!DNL Brand]の編集と削除の権限を付与できます。

### GenStudioの共同作業者

_共同作業者_&#x200B;は、GenStudio for Performance Marketingでアセットを表示できますが、これらのアセットを作成、編集、または削除することはできません。 例えば、共同作業者が[[!DNL Create]](/help/user-guide/create/overview.md)にアクセスしようとすると、「*このコンテンツにアクセスできません*」というメッセージが表示されます。

共同作業者には、コンテンツのレビューと承認プロセスの成功に不可欠だが、コンテンツを作成したり直接編集したりする必要がない関係者が含まれます。 クリエイターの法律専門家やマネージャーは、潜在的な協力者の例です。 GenStudio for Performance Marketingの共同作業者は、他のCreative Cloud製品でアセットを作成および表示する権限を持っている場合があります。

次の表に、デフォルトの共同作業者の権限を示します。

| 機能 | 作成 | 更新 | 削除 | 表示 |
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

### GenStudioの管理者

_GenStudio system manager_&#x200B;は、GenStudio for Performance Marketing内で最も強力な権限セットを持っています。 これらのパワーユーザーは、キャンペーンアセットの作成と展開のための基本的なガードレールを確立するという重要なオンボーディングタスクを実行します。 システムマネージャーは、[&#x200B; ブランドガイドライン &#x200B;](./guidelines/overview.md)などのブランドおよび組織固有の情報をアップロードすることで、これらのガードレールを実装します。 システム マネージャーには[!DNL Brands]を作成および公開する権限がありますが、ユーザー管理権限はありません。

次の表に、デフォルトのシステムマネージャー権限を示します。

| 機能 | 作成 | 更新 | 削除 | 表示 |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | はい | はい | はい | はい |
| [!DNL Campaigns] | はい | はい | はい | はい |
| [!DNL Content] | はい | はい | はい | はい |
| [!DNL Insights] | はい | はい | はい | はい |
| [!DNL Personas] | はい | はい | はい | はい |
| [!DNL Products] | はい | はい | はい | はい |
| [!DNL Reviews and approvals] | はい | はい | はい | はい |
| [!DNL Templates] | はい | はい | はい | はい |

また、システムマネージャーはテンプレートをアップロードできます。

事前設定タスクの概要については、[Adobe GenStudio for Performance Marketingの基本を学ぶ](get-started.md)を参照してください。
