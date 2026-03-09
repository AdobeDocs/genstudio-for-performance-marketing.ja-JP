---
title: Meta Ads への接続
description: Meta Ads アカウントを接続して、Adobe GenStudio for Performance Marketingで広告とメディアをアクティブ化およびモニタリングします。
level: Intermediate
role: Admin, Developer
recommendations: noDisplay
feature: Reporting and Insights
exl-id: 78110edf-947b-4e05-a3f1-de4b1eabda44
TQID: https://experienceleague.adobe.com/egZtqgG24xRPuMu7QAnuo25ZgUr-q7hGL9-k1x-PCQ0
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7id: c95c94c1-727b-457a-9184-a4dda4c95ab2id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: e0aa398c-6185-4e77-8cf7-2561c578c181id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2: id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 750
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
- 接続を試みる前に、Meta Business Manager で Instagram アカウントページの関連付けを確認してください
- 接続しているすべてのアセットへの管理者アクセスの確認

>[!ENDSHADEBOX]

## Meta Ads アカウントを接続する

1. **[!UICONTROL 詳細]**/**[!UICONTROL 設定]** をクリックします。

1. 「_Data Connectors_」セクションで、_Meta Ads **[!UICONTROL カードの]**接続_ をクリックします。

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

## 接続のベストプラクティス

エラーを防ぐには、接続を設定する際に次のベストプラクティスを考慮します。

- [ ] 初期接続のための最小限のアセット選択（単一ページのみ）で開始
- [ ] ページアクセスが機能することを確認した後にのみ Instagram アカウントを追加します
- [ ] Instagram アカウントがMeta Business Manager で選択した Facebook ページに正しく関連付けられていることを確認します
- [ ] 段階的アプローチを使用：最初に基本的な接続を確立してから、アセットを展開する
- [ 接続 ] 試みる前にすべてのアセットの管理者権限を確認するには

## Meta Ads 統合の切断とトラブルシューティング

GenStudio for Performance Marketing インスタンスがMeta Ads アカウントに正しく接続されていない場合があります。 問題の原因となる可能性のある一般的な設定を次に示します。

- Instagram アカウントは、関連する Facebook ページを選択せずに選択されます
- 最初の接続を実行したユーザーの権限を失効させました

このような場合は、Meta広告アカウントをGenStudio for Performance Marketing インスタンスに再接続するのが最適です。 まず、ユーザーはMeta Business Manager から直接アプリ統合を削除し、権限をリセットするための新しい方法を作成する必要があります。 これには、Meta Business Manager への管理者アクセス権が必要です。

次の手順では、キャッシュされた権限をクリアし、統合フローをリセットします。

1. Facebook web サイトにアクセスして ](https://business.facebook.com)0}Meta Business Manager} にアクセスします。[
1. アカウントでログインします。 アカウントには、Business Manager への管理者アクセス権が必要です。
1. 左下にある「**[!UICONTROL 設定]**」歯車アイコンをクリックして、ビジネスPortfolio設定に移動します。
1. 左側のメニューで、「**[!UICONTROL 統合]**」をクリックします。
1. **[!UICONTROL 接続されているアプリ]** を選択します。 接続されたアプリのリストにAdobe GenStudioが表示されます。
   ![Meta Business Manager 接続アプリケーション ](./meta-connected-apps.png "Meta Business Manager 接続アプリケーション ウィンドウ ")
1. アプリ名をクリックします。
1. 「**[!UICONTROL 削除]**」をクリックします。
1. プロンプトが表示されたら、削除を確認します。

Meta Ad Accounts、Instagram プロファイル、Facebook ページに再接続できるようになりました。

## Instagram アカウントの接続の問題

接続の設定中に、関連する Facebook ページを接続せずに Instagram アカウントを選択すると、問題が発生する可能性があります。 次のようなエラーが発生する場合があります。

- 「{Page_Name} に接続できませんでした」または一般的な接続エラー。
- ビジネスフローの Facebook ログイン中の接続タイムアウト。
- 複数のアセットが選択されている場合のサイレントエラー。
- Instagram、ページ、広告アカウントを同時に選択すると、接続が失敗します。

### 解決手順：

1. [Meta Business Manager](https://business.facebook.com) /統合/接続されたアプリに移動します。
1. 既存の「Adobe GenStudio」統合がある場合は、それを削除します。 「**削除**」をクリックします。
1. GenStudioに戻り、接続プロセスを再試行します。
1. 最初の接続時にターゲットの Facebook ページのみを選択します。
1. 最初の接続試行中に Instagram アカウントを選択しないでください。
1. 他のアセットを追加する前に、接続が成功したことを確認します。
1. ページ接続が安定したら、Instagram アカウントを個別に追加します。


