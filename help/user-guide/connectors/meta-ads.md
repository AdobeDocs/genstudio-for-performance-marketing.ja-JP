---
title: Meta Adsに接続
description: Meta Ads アカウントを接続して、Adobe GenStudio for Performance Marketingで広告とメディアをアクティベートおよびモニタリングします。
level: Intermediate
role: Admin, Developer
recommendations: noDisplay
feature: Reporting and Insights
exl-id: 78110edf-947b-4e05-a3f1-de4b1eabda44
TQID: https://experienceleague.adobe.com/egZtqgG24xRPuMu7QAnuo25ZgUr-q7hGL9-k1x-PCQ0
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: e0aa398c-6185-4e77-8cf7-2561c578c181
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: afce03c5167b728fe04e4722a1e4f39868d523df
workflow-type: tm+mt
source-wordcount: 875
ht-degree: 0%

---

# Meta Adsに接続

このページでは、Meta Ads プロファイルアカウントをGenStudio for Performance Marketingに接続して管理し、キャンペーンの管理、コンテンツの書き出し、アクティブなキャンペーンの広告データへのアクセスを行う方法について説明します。

>[!BEGINSHADEBOX]

**前提条件**:

- すべてのMeta サービスにアクセスできるFacebook/Meta ログイン
- Meta Business Portfolioおよび広告アカウントに対する&#x200B;_フルコントロール_ （以下を含む）:
   - キャンペーンの管理
   - パフォーマンスを見る
   - Creative Hub モックアップの管理
   - 高度な分析
- ブラウザーでポップアップブロッカーを無効にする
- 接続を試す前に、Meta Business ManagerでInstagram アカウントページの関連付けを確認します
- 接続されているすべてのアセットへの管理者アクセスを確認

>[!ENDSHADEBOX]

## Meta Ads アカウントへの接続

1. **[!UICONTROL 詳細]** > **[!UICONTROL 設定]**&#x200B;をクリックします。

1. _Data connectors_ セクションで、_Meta Ads_ カードの&#x200B;**[!UICONTROL Connect]**&#x200B;をクリックします。

1. Facebook アカウントにログインします。

   ポップアップブロッカーを削除してから、**[!UICONTROL 更新]**&#x200B;を使用して再試行する必要があります。

1. Facebookの認証手順に従って、アカウント情報を確認し、**[!UICONTROL 別名で続行…]**&#x200B;をクリックします

1. _[!UICONTROL Facebook Login for Business]_ （MetaからAdobeへのロゴ）で、次の手順に従ってGenStudio for Performance Marketingへのアクセス権を付与します。

   - 1つ以上のMeta Business プロファイルを選択し、**[!UICONTROL 続行]**&#x200B;をクリックします
   - 1つ以上のMeta ページを選択し、**[!UICONTROL 続行]**&#x200B;をクリックします
   - 1つ以上のInstagram アカウントを選択し、**[!UICONTROL 続行]**&#x200B;をクリックします
   - 選択内容を確認し、**[!UICONTROL 保存]**&#x200B;をクリックします

     ![選択項目のレビュー](/help/assets/meta/meta-review-selections.png "選択項目のレビュー"){width="400" zoomable="yes"}

1. アカウントが接続されているという確認を受け取ったら、**[!UICONTROL アカウントを取得]**&#x200B;をクリックします。

   このステップにより、GenStudio for Performance Marketingはすべての広告、メタデータ、指標にアクセスできるようになり、パフォーマンスが最適になります。

1. _[!UICONTROL Meta Ads]_&#x200B;で、[!DNL Insights]に含める1つ以上のアカウントを選択し、**[!UICONTROL 選択]**&#x200B;をクリックします。

1. _Platform connected_&#x200B;の確認を受け取ったら、「**[!UICONTROL アカウントを表示]**」をクリックします。

   _[!UICONTROL Meta広告アカウント]_ ビューには、`Account name`、`Added by`、`Date added`および`Status`が一覧表示されます。

   ![Meta アカウントリスト &#x200B;](/help/assets/meta/meta-accounts-list.png "接続されたMeta アカウントのリスト "){zoomable="yes"}

**[!UICONTROL アカウントの追加]**&#x200B;を使用して、リストにアカウントを追加します。 同じMeta Business プロファイルにリンクされているアカウントを追加すると、認証フローが少し異なる場合があります。 接続プロセスでは、新しいMeta Ads アカウントのみを選択します。

## Instagram アカウントを接続

>[!IMPORTANT]
>
>Meta広告をアクティベートする前に、Meta Business Managerで、使用するInstagram アカウントが、オンボーディング中に選択した広告アカウントと同じ広告アカウントに接続されていることを確認します。 この接続が見つからない場合、アクティベーション中にInstagram アカウントが[!DNL GenStudio for Performance Marketing] _Instagram アカウント_ ドロップダウンメニューに表示されない可能性があります。

**Meta Business ManagerでInstagram アカウントの接続を確認または更新するには**:

1. **[!UICONTROL 設定]**&#x200B;に移動します。
1. _アカウント_&#x200B;で、**[!UICONTROL Instagram アカウント]**&#x200B;を選択します。
1. 使用するInstagram アカウントを選択します。
1. 「**[!UICONTROL Connected assets]**」をクリックします。
1. _広告アカウント_&#x200B;で、オンボーディング中に使用した広告アカウントがリストされていることを確認します。
1. 一覧にない場合は、**[!UICONTROL アセットの接続]**&#x200B;をクリックし、正しい広告アカウントを追加します。

広告アカウントが接続されたら、[!DNL GenStudio for Performance Marketing]に戻り、アクティベーションフローを続行します。

## 接続のベストプラクティス

エラーを防ぐには、接続を設定する際に、次のベストプラクティスを考慮してください。

- [ ]最初の接続では、アセットの選択を最小限に抑える（1 ページのみ）
- [ ] ページアクセスが機能することを確認した後にのみInstagram アカウントを追加する
- [ ] Instagram アカウントが、Meta Business Managerで選択したFacebook ページに正しく関連付けられていることを確認します
- [ ]段階的なアプローチを使用する：まず基本的な接続を確立してから、アセットを拡張します
- [ ]接続を試みる前に、すべてのアセットの管理者権限を確認してください

## Meta Ads統合の切断とトラブルシューティング

GenStudio for Performance Marketing インスタンスがMeta Ads アカウントに正しく接続されていない場合があります。 問題の原因となる一般的な設定は次のとおりです。

- 関連するFacebook ページを選択せずにInstagram アカウントが選択される
- 最初の接続を実行したユーザーの権限を取り消しました

このような場合は、Meta Ad AccountをGenStudio for Performance Marketing インスタンスに再接続することをお勧めします。 まず、ユーザーはMeta Business Managerからアプリ統合を直接削除し、権限をリセットするためのクリーンスレートを作成する必要があります。 これには、Meta Business Managerへの管理者アクセス権が必要です。

次の手順では、キャッシュされた権限をクリアし、統合フローをリセットします。

1. Facebook Web サイトにアクセスして、[Meta Business Manager](https://business.facebook.com)にアクセスします。
1. アカウントでログインします。 アカウントには、Business Managerへの管理者アクセス権が必要です。
1. 左下の&#x200B;**[!UICONTROL Settings]**&#x200B;歯車アイコンをクリックして、Business Portfolioの設定に移動します。
1. 左側のメニューで、**[!UICONTROL 統合]**&#x200B;をクリックします。
1. **[!UICONTROL Connected Apps]**&#x200B;を選択します。 Adobe GenStudioが接続されたアプリのリストに表示されます。
   ![Meta Business Manager Connected Apps](./meta-connected-apps.png "Meta Business Manager Connected Apps ペイン ")
1. アプリ名をクリックします。
1. 「**[!UICONTROL 削除]**」をクリックします。
1. プロンプトが表示されたら、削除を確認します。

Meta広告アカウント、Instagram プロファイル、Facebook ページを再接続できるようになりました。

## Instagram アカウントの接続の問題

接続設定中に、関連するFacebook ページに接続せずにInstagram アカウントを選択すると、問題が発生する可能性があります。 これは次のようなエラーを引き起こす可能性があります：

- &quot;Could not connect to {Page_Name}&quot; or generic connection failure.
- Facebook Login for Business フロー中に接続タイムアウトが発生しました。
- 複数のアセットを選択すると、サイレントエラーが発生する。
- Instagram、ページ、広告アカウントを同時に選択すると、接続が失敗します。

### 解決ステップ：

1. [Meta Business Manager](https://business.facebook.com)/統合/Connected Appsに移動します。
1. 既存の「Adobe GenStudio」統合がある場合は、削除します。 「**削除**」をクリックします。
1. GenStudioに戻り、接続プロセスを再試行します。
1. 最初の接続時にターゲットのFacebook ページのみを選択します。
1. 最初の接続試行中にInstagram アカウントを選択しないでください。
1. 他のアセットを追加する前に、接続が正常であることを確認します。
1. ページ接続が安定したら、Instagram アカウントを個別に追加します。
