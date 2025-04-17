---
title: 有料メディアを接続
description: チャネルアカウントを連携して、Adobe GenStudio for Performance Marketingで広告やメディアをアクティブ化およびモニタリングします。
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
source-git-commit: af354448ef609db3c51026ee0e9991ac5cedeba5
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# 有料メディアアカウントの接続

GenStudio for Performance Marketing _[!DNL Data connectors]_有料メディアネットワークアカウントとのシームレスな統合を有効にします。 サードパーティのチャネルアカウントに接続することで、[[!DNL Insights]](/help/user-guide/insights/overview.md) でのキャンペーンのパフォーマンス指標などの重要なデータを交換し、[[!DNL Activate]](/help/user-guide/activation/overview.md) で新しい広告プレースメントを配信できます。 この統合により、GenStudio for Performance Marketingでは、アクティブなキャンペーンからインプレッション数、クリック数、コンバージョン数などの貴重なインサイトを受け取りながら、メディアおよび広告を管理できます。

**有料メディアアカウントに接続するには**:

1. 省略記号 **[!UICONTROL ...をクリックします。その他]** 左下のナビゲーションにあります。

1. 歯車アイコンで **[!UICONTROL 設定]** を選択します。

1. _[!UICONTROL 設定]_ で、「_[!UICONTROL Data connectors]_」セクションからコネクタタイプを選択し、「**[!UICONTROL 接続]**」をクリックします。

   オプションで、接続されているアカウントがある場合、「_接続されているアカウント_」をクリックして、アカウント名、詳細およびステータスのリストを表示できます。

1. 選択した [ コネクタタイプ ](#connector-types) を確認し、前提条件を確認して、接続手順を続行します。

## 有料メディア接続

GenStudio for Performance Marketingは、好みのマーケティングプラットフォームと統合するために、様々なコネクタタイプをサポートしています。 各コネクタタイプには、特定の前提条件と、接続を正常に完了するために実行するセットアップ手順があります。

### Google Campaign Manager 360 の接続

>[!BEGINSHADEBOX]

**前提条件**:

- Google Campaign Manager 360 アカウント
- ブラウザーでポップアップブロッカーを削除します

>[!ENDSHADEBOX]

**Google Campaign Manager 360 アカウントを接続するには**:

1. 「_Data Connectors_」セクションで、_Google Campaign Manager 360 **[!UICONTROL カードの「_ 接続]**」をクリックします。

1. Google Campaign Manager 360 アカウントにログインします。

   ポップアップ ブロックを削除してから、[**[!UICONTROL 更新]**] を使用して再試行してください。

1. 利用条件を読み、「**[!UICONTROL 許可]**」をクリックしてアクセスを許可します。

1. _[!UICONTROL Google Campaign Manager 360]_ ビューで、1 つ以上の広告主を選択し、**[!UICONTROL 選択]** をクリックします。

_[!UICONTROL Google Campaign Manager 360 アカウント]_ ビューには、`Account name`、`Added by`、`Date added` および `Status` がリストされます。 リストにさらにアカウントを追加するには、「**[!UICONTROL アカウントを追加]**」を使用します。

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

1. _[!UICONTROL Facebook Login for Business]_ ポップアップ（Meta to Adobe シンボル）で、以下の選択項目を順に実行します。

   - アカウント情報を確認し、「**[!UICONTROL 次の形式で続行]**」をクリックします
   - 選択したページへのアクセス権を付与し、「**[!UICONTROL 続行]**」をクリックします
   - 一部のビジネスへのアクセス権を付与し、「**[!UICONTROL 続行]**」をクリックします
   - 1 つ以上の Instagram アカウントをオプトインし、**[!UICONTROL 続行]** をクリックします
   - 選択内容を確認し、「**[!UICONTROL 保存]**」をクリックします

1. _[!UICONTROL メタ広告]_ 表示で、1 つ以上のアカウントを選択し、**[!UICONTROL 選択]** をクリックします。

_[!UICONTROL メタ広告アカウント]_ ビューには、`Account name`、`Added by`、`Date added` および `Status` が一覧表示されます。 リストにさらにアカウントを追加するには、「**[!UICONTROL アカウントを追加]**」を使用します。

## データ取り込み

GenStudio for Performance Marketingは、最初に、最新の 6 か月間の履歴データを読み込みます。 これにより、トレンドの分析、パフォーマンスの評価、十分な情報に基づいた意思決定を行うための関連するインサイトにすぐにアクセスできます。 アカウントのデータ量によっては、取り込みプロセスに 1～5 日かかる場合があります。

>[!BEGINSHADEBOX]

**データの取り込みと保持のポリシー**

GenStudio for Performance Marketingはチャネルデータを 13 か月間保持します。 この保持ポリシーには、最初の接続中に取り込まれた 6 か月のデータが含まれており、包括的な履歴データの分析とレポートを確実に行います。

>[!ENDSHADEBOX]
