---
title: メタ広告への接続
description: メタ広告アカウントを連携して、Adobe GenStudio for Performance Marketingで広告とメディアをアクティブ化およびモニタリングします。
level: Intermediate
role: Admin, Data Engineer
recommendations: noDisplay
feature: Reporting and Insights
source-git-commit: 2f18b273684a9fe9b9b8903838ae09f5cd2b7842
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# メタ広告への接続

メタ広告プロファイルアカウントをGenStudio for Performance Marketingに接続すると、キャンペーンの管理、コンテンツのエクスポート、アクティブなキャンペーンの広告データへのアクセスを行うことができます。

>[!BEGINSHADEBOX]

**前提条件**:

- すべてのメタサービスにアクセスできる Facebook/Meta ログイン

- メタビジネスPortfolioおよび広告アカウントに対する _フルコントロール_。以下が含まれます。

   - キャンペーンの管理
   - パフォーマンスの表示
   - Creative Hub モックアップの管理
   - 高度な分析

- ブラウザーでポップアップブロッカーを削除します

>[!ENDSHADEBOX]

**Meta 広告アカウントを接続するには**:

1. **[!UICONTROL 詳細]**/**[!UICONTROL 設定]** をクリックします。

1. 「_Data Connectors_」セクションで、**[!UICONTROL メタ広告]** カードの _接続_ をクリックします。

1. Facebook アカウントにログインします。

   ポップアップ ブロックを削除してから、[**[!UICONTROL 更新]**] を使用して再試行してください。

1. Facebook 認証の手順に従い、アカウント情報を確認して、「**[!UICONTROL 次のユーザーとして続行]**」をクリックします。

1. _[!UICONTROL ビジネス向けの Facebook ログイン]_ （Meta からAdobeへのシンボル）で、次の選択を順を追ってGenStudio for Performance Marketing アクセスを付与します。

   - 1 つ以上のメタビジネスプロファイルを選択し、「**[!UICONTROL 続行]**」をクリックします
   - 1 つ以上のメタページを選択し、「**[!UICONTROL 続行]**」をクリックします。
   - 1 つ以上の Instagram アカウントを選択し、**[!UICONTROL 続行]** をクリックします
   - 選択内容を確認し、「**[!UICONTROL 保存]**」をクリックします

     ![ 選択項目を確認 ](/help/assets/meta/meta-review-selections.png " 選択項目を確認 "){width="400" zoomable="yes"}

1. アカウントが接続されていることを確認したら、**[!UICONTROL 取得]** をクリックします。

   この手順により、最適なパフォーマンスを得るために、GenStudio for Performance Marketingがすべての広告、メタデータおよび指標にアクセスできるようにします。

1. _[!UICONTROL メタ広告]_ で、[!DNL Insights] に含める 1 つ以上のアカウントを選択し、**[!UICONTROL 選択]** をクリックします。

1. _Platform に接続_ 確認が表示されたら、「**[!UICONTROL アカウントを表示]**」をクリックします。

   _[!UICONTROL メタ広告アカウント]_ ビューには、`Account name`、`Added by`、`Date added` および `Status` が一覧表示されます。

   ![ メタアカウントリスト ](/help/assets/meta/meta-accounts-list.png " 接続されたメタアカウントのリスト "){zoomable="yes"}

リストにさらにアカウントを追加するには、「**[!UICONTROL アカウントを追加]**」を使用します。 同じメタビジネスプロファイルにリンクされたアカウントを追加する場合、承認フローが若干異なる場合があります。 接続プロセスでは、新しい Meta Ads アカウントのみを選択します。
