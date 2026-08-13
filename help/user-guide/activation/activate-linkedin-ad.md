---
title: LinkedIn広告を有効にする
description: LinkedInの広告エクスペリエンスをアクティベートする方法について説明します。
feature: Ad Activation
exl-id: edc95319-36c3-4cbf-a5c0-865b49482b50
TQID: https://experienceleague.adobe.com/1mcxWePqYd8tYp3e1D2UTSeBHSvPj4WrqeSyiUCxD8c
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
subfeature_v2: id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 863
ht-degree: 0%

---

# LinkedIn広告を有効にする

Adobe GenStudio for Performance Marketingでは、[LinkedIn Campaign Manager](https://business.linkedin.com/marketing-solutions)およびLinkedIn ページへの1つのアセットを含むLinkedIn エクスペリエンスのアクティブ化をサポートしています。

GenStudio for Performance Marketingで[LinkedIn エクスペリエンスを作成](/help/user-guide/create/create-linkedin.md)し、アクティベーション用に選択するか、[!DNL Activate]で承認済みアセットから新しいエクスペリエンスを作成できます。

LinkedIn広告のアクティベーションは、他の有料チャネルへのアクティベーションに必要な[同じ一般的な手順](create-activation.md)に従います。 このアクティベーションプロセスでは、LinkedInの特定の要件に対応するための広告エクスペリエンスの準備を支援します。 GenStudio for Performance MarketingでLinkedIn エクスペリエンスをアクティベートした後、LinkedIn Campaign Managerを使用して、最終的な公開前に特定のLinkedIn広告プレースメントのエクスペリエンスを微調整します。

GenStudioのシステムマネージャーやエディターは、

## ステップ 1:LinkedIn アカウントの設定

アクティベーションを開始する前に、LinkedIn Campaign Manager アカウントに[ ログインして](https://www.linkedin.com/campaignmanager/login)ください。

>[!BEGINSHADEBOX]

**前提条件**:

* キャンペーングループ、キャンペーン、広告を管理するための完全な権限を持つLinkedIn Campaign Manager アカウント。 このアカウントには、キャンペーングループとキャンペーンが含まれている必要があります。

* LinkedIn広告アカウントは、LinkedIn ページに広告を作成し、コンテンツを投稿するための完全な権限を持っています。

>[!ENDSHADEBOX]

## ステップ 2:LinkedIn アカウントに接続する

エクスペリエンスを活用するには、GenStudioのシステムマネージャーがLinkedInのアカウントをGenStudio for Performance Marketingに接続する必要があります。 これにより、Adobe GenStudioとLinkedInなどの外部マーケティングツール間でデータを転送し、アクティベーションプロセスを実現できます。

同期が完了したら、追加されたアカウントを表示できます。 大量のデータは同期に時間がかかります。

## ステップ 3：エクスペリエンスの準備

事前定義された設定を持つ1つ以上の承認済みエクスペリエンスを[!DNL Content]から選択して、アクティベーションを開始できます。

_エクスペリエンス設定_ ビューは、アクティベーション前にエクスペリエンスを調整およびレビューするためのワークスペースです。 複数のエクスペリエンスを選択してアクティブ化する場合、このビューには、選択したすべてのエクスペリエンスのサムネールが表示される左側のサイドバーが含まれます。 この左側のサイドバーを使用して、選択したエクスペリエンスの詳細に&#x200B;_エクスペリエンス設定_ ビューをフォーカスします。

_プレビューパネル_&#x200B;では、特定の広告プレースメントのコンテキストで、テキストとアセットのインタラクティブなビューをサポートしています。 _プレースメントを選択_ ドロップダウンメニューを使用して、サポートされている広告プレースメントを切り替えます。 プレビューを使用すると、特定のプレースメントの広告要素に関する決定を確定できます。 _プレビュー_ パネルでプレースメントを選択すると、広告の表示のみが影響を受けます。 _プレビュー_ パネルでのプレースメントの選択は保存されません。

### コンテンツから承認済みエクスペリエンスをアクティベート

1つ以上のエクスペリエンスを選択して、1つの有料チャネルにアクティベートできます。 エクスペリエンスに含めることができるアセットは1つだけです。 選択した承認済みエクスペリエンスから詳細が読み込まれます。

編集可能なエクスペリエンスの詳細は次のとおりです。

* Call-to-action（CTA）テキスト
* Web サイト URL
* リンクを表示

**エクスペリエンスを選択するには**:

1. [!DNL Content] ギャラリーの検索ツールとフィルターツールを使用して、アクティブ化するエクスペリエンスを特定し、**[!UICONTROL アクティブ化]**&#x200B;をクリックします。 または、1つのエクスペリエンスを選択して、その他（。..）から&#x200B;**[!UICONTROL アクティブ化]**&#x200B;を選択することもできます メニュー：

   このエクスペリエンスのLinkedIn広告&#x200B;_エクスペリエンス設定_ ページが開きます。 選択したエクスペリエンスの詳細が事前に入力されます。 アクティベーションを続行する前に、プラットフォームを選択するように求められる場合があります。

1. （オプション）編集可能なフィールド（**[!UICONTROL Call to action]**、**[!UICONTROL Web サイト URL]**、*[!UICONTROL 表示リンク ]**）の値を編集します。

1. （オプション）「**[!UICONTROL エクスペリエンスを追加]**」をクリックして、このアクティベーショングループにエクスペリエンスを追加します。

1. 「**[!UICONTROL 次へ]**」をクリックして、エクスペリエンスの設定を確定します。

## 手順4:LinkedIn アカウント設定の確認

広告体験を準備したら、LinkedInのアカウント情報を確認する必要があります。 _LinkedIn広告設定_ ビューには、設定されたLinkedIn アカウントから派生したオプションが入力されます。

_キャンペーングループ_&#x200B;は、LinkedIn Campaign Managerの必須コンポーネントです。 キャンペーングループは、共通の目標の下で個別のキャンペーンを整理します。 キャンペーンは、予算の制限、目的、スケジュールを、属するキャンペーングループから継承できます。

**アカウントの設定を確認するには**:

1. 「**[!UICONTROL アカウント]**」ドロップダウンメニューからアカウントを選択します。 オプションは、GenStudio for Performance Marketingに接続されたLinkedIn アカウントです。

1. **[!UICONTROL キャンペーングループ]** ドロップダウンメニューからキャンペーングループを選択します。 エクスペリエンスが公開されるLinkedIn キャンペーングループです。

1. 「**[!UICONTROL キャンペーン]**」ドロップダウンメニューからキャンペーンを選択します。 これは、広告体験の配信先となるLinkedInのキャンペーンです。

1. 各エクスペリエンスの「**[!UICONTROL 広告名]**」フィールドに広告名を入力します。 LinkedIn Campaign Managerでは、エクスペリエンスがこの名前で識別されます。

1. 「**[!UICONTROL 次へ]**」をクリックして、LinkedIn広告の設定を確定します。

## 手順5：広告のプレビューとアクティベート

_レビュー_ ページでは、公開前にアクティベーションをレビューする最後の機会を提供します。

**エクスペリエンスをレビューして公開するには**:

1. （オプション）編集するエクスペリエンスまたはプラットフォームの詳細の横にある「**[!UICONTROL セクションを編集]**」をクリックします。
選択したセクションに応じて、_エクスペリエンスの設定_&#x200B;または&#x200B;_プラットフォームの設定_ ビューが開きます。

1. （オプション）詳細を編集し、**[!UICONTROL 次へ]**&#x200B;をクリックして&#x200B;_レビュー_&#x200B;表示に戻ります。

1. 「**[!UICONTROL 公開する]**」をクリックします。

   LinkedInの広告エクスペリエンス全体とその関連メタデータは、指定されたLinkedIn Campaigns Manager キャンペーンに直接送信されます。 エクスペリエンスは非アクティブな状態で配信されます。 LinkedIn Campaign Managerでは、広告エクスペリエンスとLinkedIn キャンペーンのデプロイの最終手順を管理できます。

## 手順6：広告体験の公開を完了する

1. LinkedIn Campaign Manager アカウントに[ ログインして](https://www.linkedin.com/campaignmanager/login)広告エクスペリエンスを確認し、特定のLinkedIn ページへの公開を確定します。
