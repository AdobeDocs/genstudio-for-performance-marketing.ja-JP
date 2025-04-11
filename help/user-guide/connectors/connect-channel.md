---
title: 有料メディアを接続
description: Connect a channel account to activate and monitor your ads and media with Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
source-git-commit: 2844914d25d9bc3a2be7f47d0cd7f26f7c921555
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Connect paid media accounts

_[!DNL Data connectors]_enable seamless integration between GenStudio for Performance Marketing and your paid media network accounts. By connecting to third-party channel accounts, you can exchange critical data, such as campaign performance metrics in [[!DNL Insights]](/help/user-guide/insights/overview.md), and you can deliver fresh ad placements with [[!DNL Activate]](/help/user-guide/activation/overview.md). This integration allows GenStudio for Performance Marketing to manage your media and ads while receiving valuable insights, including impressions, clicks, and conversions, from your active campaigns.

**有料メディアアカウントに接続するには**:

1. 省略記号 **[!UICONTROL ...をクリックします。その他]** 左下のナビゲーションにあります。

1. 歯車アイコンで **[!UICONTROL 設定]** を選択します。

1. _[!UICONTROL 設定]_ で、「_[!UICONTROL Data connectors]_」セクションからコネクタタイプを選択し、「**[!UICONTROL 接続]**」をクリックします。

   オプションで、接続されているアカウントがある場合、「_接続されているアカウント_」をクリックして、アカウント名、詳細およびステータスのリストを表示できます。

1. 選択した [ コネクタタイプ ](#connector-types) を確認し、前提条件を確認して、接続手順を続行します。

## 有料メディア接続

GenStudio for Performance Marketing supports various connector types to integrate with your preferred marketing platforms. Each connector type has specific prerequisites and set-up steps to complete for a successful connection.

### メタ広告接続

>[!BEGINSHADEBOX]

**前提条件**:

- Facebook/メタ広告アカウント
- レポートへのアクセスと広告の表示 `View performance` 行う権限レベルを持つメタ広告アカウントへのアクセス
- ブラウザーでポップアップブロッカーを削除します

>[!ENDSHADEBOX]

**Meta 広告アカウントを接続するには**:

1. 「_Data Connectors_」セクションで、**[!UICONTROL メタ広告]** カードの _接続_ をクリックします。

1. Facebook アカウントにログインします。

   ポップアップ ブロックを削除してから、[**[!UICONTROL 更新]**] を使用して再試行してください。

1. Facebook 認証の手順に従います。

1. In the _[!UICONTROL Facebook Login for Business]_ pop-up (Meta to Adobe symbol), step through the following selections.

   - Verify the account information and click **[!UICONTROL Continue as]**
   - Grant access to select Pages and click **[!UICONTROL Continue]**
   - 一部のビジネスへのアクセス権を付与し、「**[!UICONTROL 続行]**」をクリックします
   - 1 つ以上の Instagram アカウントをオプトインし、**[!UICONTROL 続行]** をクリックします
   - 選択内容を確認し、「**[!UICONTROL 保存]**」をクリックします

1. _[!UICONTROL メタ広告]_ 表示で、1 つ以上のアカウントを選択し、**[!UICONTROL 選択]** をクリックします。

_[!UICONTROL メタ広告アカウント]_ ビューには、`Account name`、`Added by`、`Date added` および `Status` が一覧表示されます。 リストにさらにアカウントを追加するには、「**[!UICONTROL アカウントを追加]**」を使用します。

## データ取り込み

GenStudio for Performance Marketingは、最初に、最新の 6 か月間の履歴データを読み込みます。 これにより、トレンドの分析、パフォーマンスの評価、十分な情報に基づいた意思決定を行うための関連するインサイトにすぐにアクセスできます。 The ingestion process may take one to five days depending on the volume of data in your account.

>[!BEGINSHADEBOX]

**データの取り込みと保持のポリシー**

GenStudio for Performance Marketingはチャネルデータを 13 か月間保持します。 この保持ポリシーには、最初の接続中に取り込まれた 6 か月のデータが含まれており、包括的な履歴データの分析とレポートを確実に行います。

>[!ENDSHADEBOX]
