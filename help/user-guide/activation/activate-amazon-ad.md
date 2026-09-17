---
title: Amazon Adsをアクティベート
description: Amazon広告のエクスペリエンスをアクティベートする方法について説明します。
feature: Ad Activation
exl-id: 539cb43c-a9d8-4473-8a7d-e81967111741
TQID: https://experienceleague.adobe.com/4L4JHcYLSsoQ50QbCW7Mof52h5jpz3z8n0UL8CaqLA8
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
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%
---
# Amazon Adsをアクティベート

Adobe GenStudio for Performance Marketingは、Amazon Adsへの広告体験のアクティベーションをサポートしています。

**サポートされている形式**：静的表示。

Amazon広告エクスペリエンスのアクティベーションは、他の有料広告チャネルへのアクティベーションに必要な[同じ一般的な手順](create-activation.md)に従います。 このページでは、Amazon Ads固有の前提条件と設定フィールドについて説明します。 GenStudio for Performance Marketingでエクスペリエンスをアクティベートしたら、Amazon Adsを使用してエクスペリエンスをレビューし、広告を起動します。

GenStudioのシステムマネージャーやエディターは、

## 前提条件

* ターゲットのAmazon Ads アカウントへのアクセス。
* Amazon Adsへの読み取りおよび書き込みをおこなうための管理者アクセス権を持ちます。

Amazon Adsは、様々なアカウント内のキャンペーンや広告を整理し、各アカウントにはクリエイティブライブラリが含まれます。 ターゲットアカウントは既にAmazon Adsに存在している必要があります。GenStudio for Performance Marketingは、そのアカウントのクリエイティブライブラリに広告エクスペリエンスを公開しますが、アカウントは作成しません。

## Amazon Ads アカウントへの接続

クリエイティブライブラリでアセットを公開する前に、GenStudioのシステムマネージャーがAmazon Ads アカウントをGenStudio for Performance Marketingに接続する必要があります。 Amazon Adsの読み取りおよび書き込みを行うには、そのアカウントへの管理者アクセス権が必要です。 [有料メディアアカウントの接続](/help/user-guide/connectors/connect-channel.md)を参照してください。

同期が完了したら、追加されたアカウントを表示できます。

## Amazon広告の設定フィールド

承認されたアセットは[!DNL Content]でレビューと承認が完了しているため、アクティブ化中はロックされ、編集できません。 次の項目を編集できます。

* **テキストフィールド**: トラッキング ID （プラットフォームのクリエイティブ名として使用）
* **プラットフォーム設定フィールド**: アカウント

アクティベーションが完了すると、クリエイティブエクスペリエンスはAmazon Adsの選択したアカウントのクリエイティブライブラリに配信されます。
