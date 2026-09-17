---
title: ChatGPT広告をアクティベートする
description: ChatGPT広告エクスペリエンスをアクティベートする方法について説明します。
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
source-wordcount: '272'
ht-degree: 0%
---
# ChatGPT広告をアクティベートする

Adobe GenStudio for Performance Marketingは、ChatGPT広告エクスペリエンスのアクティベーションをサポートします。

**サポートされている形式**: チャットカード。

GenStudio for Performance Marketingで[ChatGPT エクスペリエンス &#x200B;](/help/user-guide/create/create-chatgpt-ad.md)を作成し、アクティベーション用に選択できます。

ChatGPT広告のアクティベーションは、他の有料広告チャネルへのアクティベーションに必要な[一般的な手順](create-activation.md)に従います。 このページでは、ChatGPT固有の前提条件と設定フィールドについて説明します。 GenStudio for Performance MarketingでChatGPT エクスペリエンスをアクティベートしたら、OpenAI Ads Managerを使用して最終チェックを実行し、広告を起動します。

GenStudioのシステムマネージャーやエディターは、

## 前提条件

* OpenAI広告アカウントとそのアカウントのAPI キー。
* ターゲットのChatGPT キャンペーンと広告グループは、既にOpenAI Ads Managerに存在している必要があります。 GenStudio for Performance Marketingでは、新しいキャンペーンや広告グループは作成されません。

## ChatGPT アカウントを接続

エクスペリエンスをアクティベートする前に、GenStudioのシステムマネージャーがOpenAI Ads アカウントをGenStudio for Performance Marketingに接続する必要があります。

1. OpenAI Ads Managerで、**[!UICONTROL Settings]** > **[!UICONTROL API Keys]** > **[!UICONTROL Create New Key]**&#x200B;に移動します。
1. GenStudio for Performance Marketingで、**[!UICONTROL More]** > **[!UICONTROL Settings]** > **[!UICONTROL ChatGPT]** > **[!UICONTROL Connect]** > **[!UICONTROL Add Account]**&#x200B;に移動します。
1. OpenAI Ads アカウントの名前を入力し、API キーを貼り付け、**[!UICONTROL アカウントを追加]**&#x200B;をクリックします。

## ChatGPT設定フィールド

承認済みのアセット、見出し（タイトル）、本文コピーはロックされ、既に[!DNL Content]でレビューと承認が行われているため、アクティベーション中は編集できません。 次の項目を編集できます。

* **テキストフィールド**：ターゲット URL、トラッキング ID （プラットフォームの広告名として使用）
* **プラットフォーム設定フィールド**: OpenAI Ads アカウント、OpenAI キャンペーン、OpenAI広告グループ

ターゲット URLは、有効な`https://`形式（例：`https://www.example.com`）を使用する必要があります。
