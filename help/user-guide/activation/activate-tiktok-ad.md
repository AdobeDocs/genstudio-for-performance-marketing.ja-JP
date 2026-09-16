---
title: TikTok広告のアクティベート
description: TikTokのインフィード動画広告エクスペリエンスをアクティベートする方法について説明します。
feature: Ad Activation
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: d87258a7-722c-4afd-b632-adddc447c7aa
    internal-label: Ad activation
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
source-wordcount: '294'
ht-degree: 1%
---
# TikTok広告のアクティブ化

Adobe GenStudio for Performance Marketingは、TikTok広告エクスペリエンスのアクティベーションをサポートします。

**サポートされている形式**：インフィード ビデオ広告。

GenStudio for Performance Marketingで[TikTok エクスペリエンスを作成](/help/user-guide/create/tiktok-experiences.md)し、アクティベーション用に選択できます。

TikTok広告のアクティベーションは、他の有料広告チャネルへのアクティベーションに必要な[同じ一般的な手順](create-activation.md)に従います。 このページでは、TikTok固有の前提条件と設定フィールドについて説明します。 GenStudio for Performance MarketingでTikTok エクスペリエンスをアクティベートしたら、TikTok Ads Managerを使用して最終チェックを実行し、広告を起動します。

GenStudioのシステムマネージャーやエディターは、

## 前提条件

* Operatorまたは管理者アクセス権を持つTikTok Ads アカウント。
* GenStudio システムマネージャーまたはエディターによって接続された、使用が有効な少なくとも1つのTikTok広告アカウント。
* ターゲット TikTok キャンペーンは、TikTok Ads Managerに既に存在している必要があります。 GenStudio for Performance Marketingではなく、TikTok Ads Managerが、広告グループの予算、入札、最適化、ターゲティングを定義します。

## TikTok アカウントを連携する

エクスペリエンスをアクティベートする前に、GenStudioのシステムマネージャーがTikTok Ads アカウントをGenStudio for Performance Marketingに接続する必要があります。

1. **[!UICONTROL Settings]** > **[!UICONTROL TikTok]** > **[!UICONTROL Connect]**&#x200B;に移動します。
1. 開いたウィンドウでTikTok Ads Manager アカウントにログインし、OAuth ログインを完了します。 お客様のアカウントには、広告アカウントへのオペレーターまたは管理者のアクセス権が必要です。

接続が完了したら、少なくとも1つのTikTok広告アカウントが使用可能になっていることを確認します。

## TikTok設定フィールド

承認済みアセットとプライマリテキストは[!DNL Content]でレビューと承認が完了しているため、アクティブ化中はロックされ、編集できません。 次の項目を編集できます。

* **テキストフィールド**:Call-to-action、宛先URL、トラッキング ID （プラットフォームの広告名として使用）
* **プラットフォーム設定フィールド**:TikTok Ads アカウント、Campaign、広告グループ
