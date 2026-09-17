---
title: LinkedIn広告を有効にする
description: LinkedInの広告エクスペリエンスをアクティベートする方法について説明します。
feature: Ad Activation
exl-id: edc95319-36c3-4cbf-a5c0-865b49482b50
TQID: https://experienceleague.adobe.com/1mcxWePqYd8tYp3e1D2UTSeBHSvPj4WrqeSyiUCxD8c
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%
---
# LinkedIn広告を有効にする

Adobe GenStudio for Performance Marketingでは、[LinkedIn Campaign Manager](https://business.linkedin.com/marketing-solutions)へのLinkedIn広告エクスペリエンスのアクティブ化をサポートしています。

**サポートされている形式**：単一の画像、単一のビデオ。

GenStudio for Performance Marketingで[LinkedIn エクスペリエンスを作成](/help/user-guide/create/create-linkedin.md)し、アクティベーション用に選択できます。

LinkedIn広告のアクティベーションは、他の有料広告チャネルへのアクティベーションに必要な[同じ一般的な手順](create-activation.md)に従います。 このページでは、LinkedIn固有の前提条件と設定フィールドについて説明します。 GenStudio for Performance MarketingでLinkedIn エクスペリエンスをアクティベートしたら、LinkedIn Campaign Managerを使用してエクスペリエンスを確認し、広告を起動します。

GenStudioのシステムマネージャーやエディターは、

## 前提条件

* キャンペーンと広告を管理するための完全な権限を持つLinkedIn Campaign Manager アカウント。 このアカウントには既存のキャンペーンが含まれている必要があります。
* LinkedIn広告アカウントは、LinkedIn ページに広告を作成し、コンテンツを投稿するための完全な権限を持っています。

ターゲット LinkedIn キャンペーンと広告セットは、LinkedIn Campaign Managerに既に存在している必要があります。 GenStudio for Performance Marketingでは、キャンペーンや広告セットは作成されません。

>[!NOTE]
>
>LinkedInはキャンペーン階層の名前を変更しました：LinkedIn Campaign Managerが以前&#x200B;**キャンペーングループ**&#x200B;と呼んでいたものを&#x200B;**キャンペーン**&#x200B;と呼び、以前は&#x200B;**キャンペーン**&#x200B;と呼んでいたものを&#x200B;**広告セット**&#x200B;と呼んでいます。 [!DNL Activate]の&#x200B;**[!UICONTROL LinkedIn キャンペーン]**&#x200B;および&#x200B;**[!UICONTROL LinkedIn広告セット]**&#x200B;設定フィールドでは、この現在の用語が使用されています。

GenStudio for Performance Marketingでは現在、1つの画像と1つの動画のLinkedIn広告がサポートされており、1つの投稿につき1つの画像または動画のみを配信します。 エクスペリエンスに複数の縦横比が含まれる場合、[!DNL Activate]はアクティベーションテーブルの比率ごとに個別の行を生成し、各行を独自の広告として実行できるようにします。不要な行はすべて削除します。

## LinkedIn アカウントを接続

エクスペリエンスを活用するには、GenStudioのシステムマネージャーまたはエディターが、LinkedIn広告アカウントとGenStudio for Performance Marketingを連携させる必要があります。 正常に接続するには、広告アカウントとLinkedIn プロファイルページの両方に完全な管理者アクセス権が必要です。 広告アカウントを接続する必要があるのは、**[!UICONTROL 設定]**&#x200B;の1回のみです。 その後、そのインスタンスにアクセスできる人なら誰でも利用できます。

この接続により、GenStudio for Performance MarketingとLinkedIn間でデータを転送し、アクティベーションプロセスを実現できます。

同期が完了したら、追加されたアカウントを表示できます。 大量のデータは同期に時間がかかります。

## LinkedIn設定フィールド

承認されたアセット、見出し、および概要テキストはロックされ、既に[!DNL Content]でレビューと承認を行っているため、アクティベーション中に編集することはできません。 次の項目を編集できます。

* **テキストフィールド**：説明、Call-to-action、宛先URL、URL パラメーター、トラッキング ID （プラットフォームの広告名として使用）
* **プラットフォーム設定フィールド**:LinkedIn広告アカウント、LinkedIn キャンペーン、LinkedIn広告セット
