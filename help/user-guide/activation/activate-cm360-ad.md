---
title: Google Campaign Manager 360広告のアクティベート
description: Google Campaign Manager 360 エクスペリエンスをアクティベートする方法について説明します。
feature: Ad Activation
exl-id: e4ee4e04-8dd0-4e05-a0f7-0ddca2fbb6be
TQID: https://experienceleague.adobe.com/pQbT2OC7-jK33HhJWgTBBtJrmEvr48mGkl8v-fTkOLQ
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
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%
---
# Google Campaign Manager 360広告のアクティベート

Adobe GenStudio for Performance Marketingは、Google Campaign Manager 360への広告エクスペリエンスのアクティベーションをサポートしています。

**サポートされている形式**：静的ディスプレイ、ビデオディスプレイ、HTML5 Zip ディスプレイ。

Google Campaign Manager 360広告のアクティベーションは、他の有料広告チャネルへのアクティベーションに必要な[同じ一般的な手順](create-activation.md)に従います。 このページでは、Google Campaign Manager 360に固有の前提条件と設定フィールドについて説明します。 GenStudio for Performance Marketingでエクスペリエンスをアクティベートしたら、Google Campaign Manager 360を使用してエクスペリエンスを確認し、広告を起動します。

GenStudioのシステムマネージャーやエディターは、

## 前提条件

* ターゲット広告主へのアクセス権を持つGoogle Campaign Manager 360 アカウント。
* Campaign Manager 360への読み取りと書き込みをおこなうための広告主への管理者アクセス権。

キャンペーンマネージャー360は、異なる広告主内のキャンペーンおよび広告を整理し、各広告主はクリエイティブライブラリを含む。 ターゲット広告主は、既にCampaign Manager 360に存在している必要があります。GenStudio for Performance Marketingは、広告主のクリエイティブライブラリに広告エクスペリエンスを公開しますが、広告は作成しません。

## Google Campaign Manager 360 アカウントを連携する

クリエイティブライブラリでアセットを公開する前に、GenStudio システムマネージャーまたはエディターがGoogle Campaign Manager 360 アカウントをGenStudio for Performance Marketingに接続する必要があります。 Campaign Manager 360への読み取りと書き込みをおこなうには、広告主への管理者アクセス権が必要です。 [有料メディアアカウントの接続](/help/user-guide/connectors/connect-channel.md)を参照してください。

同期が完了したら、追加されたアカウントを表示できます。

## Google Campaign Manager 360の設定フィールド

承認されたアセットは[!DNL Content]でレビューと承認が完了しているため、アクティブ化中はロックされ、編集できません。 次の項目を編集できます。

* **テキストフィールド**: トラッキング ID （プラットフォームのクリエイティブ名として使用）
* **プラットフォーム設定フィールド**：広告主

アクティベーションが完了すると、クリエイティブエクスペリエンスはGoogle Campaign Manager 360の選択した広告主のクリエイティブライブラリに配信されます。
