---
title: Meta Ads への接続
description: Meta Ads アカウントを接続して、Adobe GenStudio for Performance Marketingで広告とメディアをアクティブ化およびモニタリングします。
level: Intermediate
role: Admin, Data Engineer
recommendations: noDisplay
feature: Reporting and Insights
exl-id: 78110edf-947b-4e05-a3f1-de4b1eabda44
source-git-commit: fb5fe4885340639f8179c8de6944ac21bfe009ec
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Meta Ads への接続

このページでは、Meta Ads プロファイルアカウントをGenStudio for Performance Marketingに接続して管理し、キャンペーンの管理、コンテンツのエクスポート、アクティブなキャンペーンの広告データへのアクセスを行う方法について説明します。

>[!BEGINSHADEBOX]

**前提条件**:

- すべてのMeta サービスにアクセスできる Facebook/Meta ログイン

- 以下を含むMeta Business Portfolioおよび広告アカウントに対する _フルコントロール_

   - キャンペーンの管理
   - パフォーマンスの表示
   - Creative Hub モックアップの管理
   - 高度な分析

- ブラウザーでポップアップブロッカーを無効にする

>[!ENDSHADEBOX]

## Meta広告アカウントを接続

1. **[!UICONTROL 詳細]**/**[!UICONTROL 設定]** をクリックします。

1. 「_Data Connectors_」セクションで、**[!UICONTROL Meta Ads]** カードの _接続_ をクリックします。

1. Facebook アカウントにログインします。

   ポップアップ ブロックを削除してから、[**[!UICONTROL 更新]**] を使用して再試行してください。

1. Facebook 認証の手順に従い、アカウント情報を確認して、「**[!UICONTROL 次のユーザーとして続行]**」をクリックします。

1. _[!UICONTROL ビジネス向けの Facebook ログイン]_ （MetaからAdobeへのシンボル）で、以下の選択項目を順を追ってGenStudio for Performance Marketing アクセスを付与します。

   - 1 つ以上のMeta ビジネスプロファイルを選択し、「**[!UICONTROL 続行]**」をクリックします
   - 1 つ以上のMetaページを選択し、「**[!UICONTROL 続行]**」をクリックします
   - 1 つ以上の Instagram アカウントを選択し、**[!UICONTROL 続行]** をクリックします
   - 選択内容を確認し、「**[!UICONTROL 保存]**」をクリックします

     ![ 選択項目を確認 ](/help/assets/meta/meta-review-selections.png " 選択項目を確認 "){width="400" zoomable="yes"}

1. アカウントが接続されていることを確認したら、**[!UICONTROL 取得]** をクリックします。

   この手順により、最適なパフォーマンスを得るために、GenStudio for Performance Marketingがすべての広告、メタデータおよび指標にアクセスできるようにします。

1. _[!UICONTROL Meta広告]_ で、[!DNL Insights] に含める 1 つ以上のアカウントを選択し、**[!UICONTROL 選択]** をクリックします。

1. _Platform に接続_ 確認が表示されたら、「**[!UICONTROL アカウントを表示]**」をクリックします。

   _[!UICONTROL Meta Ads アカウント]_ ビューには、`Account name`、`Added by`、`Date added` および `Status` がリストされます。

   ![Meta アカウントのリスト ](/help/assets/meta/meta-accounts-list.png " 接続されているMeta アカウントのリスト "){zoomable="yes"}

リストにさらにアカウントを追加するには、「**[!UICONTROL アカウントを追加]**」を使用します。 同じMeta ビジネスプロファイルにリンクされたアカウントを追加する場合、認証フローが若干異なることがあります。 接続プロセスでは、新しいMeta Ads アカウントのみを選択します。

## Meta Ads 統合の切断とトラブルシューティング

GenStudio for Performance Marketing インスタンスがMeta Ads アカウントに正しく接続されていない場合があります。 問題の原因となる可能性のある一般的な設定を次に示します。

- Instagram アカウントは、関連する Facebook ページを選択せずに選択されます
- 最初の接続を実行したユーザーの権限を失効させました

このような場合は、Meta広告アカウントをGenStudio for Performance Marketing インスタンスに再接続するのが最適です。 まず、ユーザーはMeta Business Manager から直接アプリ統合を削除し、権限をリセットするための新しい方法を作成する必要があります。 これには、Meta Business Manager への管理者アクセス権が必要です。

次の手順では、キャッシュされた権限をクリアし、統合フローをリセットします。

1. Facebook web サイトにアクセスして [0}Meta Business Manager} にアクセスします。](https://business.facebook.com)
1. アカウントでログインします。 アカウントには、Business Manager への管理者アクセス権が必要です。
1. 左下にある「**[!UICONTROL 設定]**」歯車アイコンをクリックして、ビジネスPortfolio設定に移動します。
1. 左側のメニューで、「**[!UICONTROL 統合]**」をクリックします。
1. **[!UICONTROL 接続されているアプリ]** を選択します。 接続されたアプリのリストにAdobe GenStudioが表示されます。
   ![Meta Business Manager 接続アプリケーション ](./meta-connected-apps.png "Meta Business Manager 接続アプリケーション ウィンドウ ")
1. アプリ名をクリックします。
1. 「**[!UICONTROL 削除]**」をクリックします。
1. プロンプトが表示されたら、削除を確認します。

Meta広告アカウント、Instagram プロファイル、Facebook ページに再接続できるようになりました。
