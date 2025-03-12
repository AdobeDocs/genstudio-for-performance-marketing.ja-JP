---
title: GenStudio for Performance Marketingの概要  [!DNL Create]
description: Adobe GenStudio for Performance Marketing [!DNL Create] のジェネレーティブ AI を使用して、高パフォーマンスのオンブランドコンテンツを迅速に生成します。
feature: Create, Prompt, Guidelines, Experiences, Content Generation, Approval
exl-id: ca5ee31c-d2c2-42fb-a6bf-05fd63fe86d2
source-git-commit: 11d86ddddd1289c0bd198f21fe75a84b1459253e
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 1%

---

# GenStudio for Performance Marketing [!DNL Create]

GenStudio for Performance Marketing [!DNL Create] は、Adobe GenAI の機能を活用して、マーケターや分散型チームが高パフォーマンスのオンブランドエクスペリエンスを作成できるようにします。

![ ダッシュボードを作成 ](/help/assets/create.png){width="600" zoomable="yes"}

[!DNL Create] を使用すると、次のチャネルのコンテンツを生成できます。

* [メール](email-experiences.md)
* [ メタ広告 ](meta-experiences.md)
* [ 広告を表示 ](display-ad-experiences.md)

[ ガイドライン ](/help/user-guide/guidelines/overview.md) （[!DNL Brands]、[!DNL Products]、[!DNL Personas]） [ コンテンツ ](/help/user-guide/content/overview.md)、[ レビューと承認 ](/help/user-guide/approvals/overview.md)、[ インサイト ](/help/user-guide/insights/overview.md) の機能に加えて、効果的なブランドに合致したマーケティングコンテンツの作成 [!DNL Create] 容易になります。

編集者とシステムマネージャーは [!DNL Create] に対するフルアクセス権を持ちます。 役割へのアクセス情報について詳しくは、[ ユーザーの役割と権限 ](/help/user-guide/user-roles.md) を参照してください。

## [!DNL Create] のユースケース

<table style="table-layout:fixed">

<tr style="border: 0;">

   <td align="center" valign="top" width="100">

      <a href="/help/user-guide/create/create-email-experience.md">

      <img alt="コンテンツを新規作成" src="../../assets/icons/icon-create.svg" width="35">

      </a>

      <div>

         <a href="/help/user-guide/create/create-email-experience.md">

         <strong> メールエクスペリエンスの作成 </strong>

         </a>

      </div>

   </td>

   <td align="center" valign="top" width="100">

      <a href="/help/user-guide/create/create-meta-ad.md">

      <img alt="メタ広告エクスペリエンスの作成" src="../../assets/icons/icon-asset.svg" width="35">

      </a>

      <div>

         <a href="/help/user-guide/create/create-meta-ad.md">

         <strong> メタ広告エクスペリエンスの作成 </strong>

         </a>

      </div>

   </td>

   <td align="center" valign="top" width="100">

      <a href="/help/user-guide/create/create-display-ad.md">

      <img alt="ディスプレイとエクスペリエンスの作成" src="../../assets/icons/icon-addTemplate.svg" width="35">

      </a>

      <div>

         <a href="/help/user-guide/create/create-display-ad.md">

         <strong> ディスプレイ広告エクスペリエンスの作成 </strong>

         </a>

      </div>

   </td>

</tr>

</table>

GenStudio for Performance Marketingを使用すると、マーケターは **新しいマーケティングコンテンツを作成** できます。 このユースケースでは、定義済みの [ ガイドライン ](/help/user-guide/guidelines/overview.md) とインスピレーション画像を使用して、ブランドに合わせたコンテンツの作成を通知します。

## [!DNL Create] 機能

GenStudio for Performance Marketingの様々なコンポーネントを統合して、コンテンツの生成を支援で [!DNL Create] ます。

### テンプレート

_今日は何を作成しますか？_ のセクションでは、コンテンツ生成で使用する、ブランド承認済みのテンプレートにアクセスできます。 テンプレートを使用すると、コンテンツ作成プロセスを即座に開始でき、定義済みのブランドアイデンティティとの連携が保たれます。

テンプレートは [ にアップロードおよび保存  [!DNL Content]](/help/user-guide/content/overview.md) され、[!DNL Create] からアクセスできます。

### パラメーター

プロンプトドロワーでは、[!DNL Brands]、[!DNL Products]、[!DNL Personas] （ガイドライン）などの _パラメーター_ と [!DNL Content] （アセット）を追加して、生成されたエクスペリエンスを形作ることができます。

これらの追加されたパラメーターは、生成プロセスに [ ガイドライン ](/help/user-guide/guidelines/overview.md) とアセットを挿入し、ブランドの包括的な ID に合わせてコンテンツをカスタマイズできるようにします。 GenStudio for Performance Marketingにガイドラインを追加し、コンテンツ作成プロセス中に使用することをお勧めします。ガイドラインは適切なオンブランドコンテンツの作成を大幅に向上させるからです。

_パラメーター_ 内のコンテンツ（アップロードまたは追加された画像アセット）は、生成されたバリアントで使用され、バリアント用に生成されたコピーコンテンツ（テキスト）に通知されます。 アセットをアップロードすることも、[!DNL Content] または接続されたAEM Content Hub リポジトリに既に存在するアセットを選択することもできます。

### プロンプト

[ 効果的なプロンプトの作成 ](/help/user-guide/effective-prompts.md) は、[!DNL Create] の生成プロセスの重要な部分です。

AI で生成されたコンテンツを作成するには、生成するコンテキストまたはエクスペリエンスを記述した [ 説明プロンプト ](/help/user-guide/effective-prompts.md) と、[ ガイドライン ](/help/user-guide/guidelines/overview.md) および [_パラメーター_](#parameters) をプロンプトドロワーに入力し、「**[!UICONTROL 生成]**」をクリックします。

### ブランドの検証

GenStudio for Performance Marketingは、（[ ガイドライン ](/help/user-guide/guidelines/overview.md) で定義されている）ブランドの ID の様々な側面に対してブランド検証を実行します。 [ ブランドの検証 ](/help/user-guide/guidelines/brand-validation.md) 生成されたコンテンツの情報を確認できます。これは、ブランドガイドラインへの準拠と、テキストと画像の一貫性を示します。 この情報を使用して、生成されたエクスペリエンスを改訂または改善し、ブランドとさらに良く一致させることができます。

### レビューと承認

組み込みの [ レビューと承認 ](/help/user-guide/approvals/overview.md) 機能を使用して、作成プロセス中にレビューを勧誘、レビューのコメントを追跡、承認を取得します。

コンテンツバリエーションの生成が完了したら、関係者の承認を得るためにドラフトを送信します。これにより、関係者はドラフトを保存して、マーケティング活動に実装で [!DNL Content] ます。

### ドラフト

[!DNL Create] の _最近の作業_ セクションで、最近のすべてのドラフトにアクセスして管理します。 以前の作業を表示して完了し、[[!DNL Content]](/help/user-guide/content/overview.md) への公開や使用するための書き出しの準備を行います。

進行中のドラフトは自動的に保存されます。 [!DNL Create] ホームに戻ると、「_最近の作業_ セクションが更新され、最新のドラフトが表示されます。 このセクションの各ドラフトには、「ドラフト _、「承認済み_ などのステータスが表示 _れ_ す。

並べ替えアイコン（グリッドまたはテーブル）をクリックして、_最近の作業_ 項目をグリッドまたはテーブル表示に表示します。

### バリアントの管理

GenStudio for Performance Marketingでは [ 個々のバリアントのセクションを包括的に制御 ](/help/user-guide/create/manage-variants.md) できます。

単一のバリアントのセクションを改訂し、個々のセクションのコンテンツを再生成し、提案された編集内容を使用して、メッセージ、サイズ、アセットなどをキャンバス内ですべて改善できます。
