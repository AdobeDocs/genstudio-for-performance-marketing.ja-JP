---
title: The Trade Deskへの広告の有効化
description: The Trade Deskへの静的ディスプレイ広告エクスペリエンスのアクティベーション方法について説明します。
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
source-wordcount: '461'
ht-degree: 0%
---
# The Trade Deskへの広告の有効化

Adobe GenStudio for Performance Marketingは、The Trade Deskへの広告体験の活性化をサポートしています。

**サポートされている形式**：静的表示（単一アセットのみ）。

The Trade Deskへの広告のアクティベーションは、他の有料広告チャネルへのアクティベーションに必要な[一般的な手順](create-activation.md)に従いますが、1つの違いがあります。 Trade Deskはセルフサービスの広告プラットフォームではなく、マネージドエンタープライズサービスであるため、アカウントアクセスは他のチャネルとは異なります。 このページでは、これらの違いに加えて、The Trade Deskに固有の前提条件と設定フィールドについて説明します。

GenStudioのシステムマネージャーやエディターは、

## 前提条件

* The Trade Deskのアカウントを作成します。 GenStudio for Performance Marketingに接続する前に、The Trade Deskで直接設定します。
* The Trade Desk アカウントチームが有効にしたAPI アクセス。 The Trade Deskの場合、アカウントチームは、他の有料広告チャネルで使用されるOAuth サインインではなく、API トークンを使用して、お客様の代わりに本アクセスを有効にします。
* The Trade DeskがGenStudio for Performance Marketingとの連携のために有効化した、正しい広告主、座席、権限。
* クリエイティブをターゲット広告主アカウントに公開する権限を持つ、The Trade Desk アカウントチームからのAPI トークンまたは資格情報。
* The Trade Deskに既に存在する宛先キャンペーン。 GenStudio for Performance Marketingは、その既存のキャンペーンに広告をアクティベートします。

## The Trade Desk アカウントに接続する

エクスペリエンスをアクティベートする前に、The Trade Deskのアカウントチームと協力してAPI アクセスを有効にしてから、GenStudioのシステムマネージャーがアカウントをGenStudio for Performance Marketingに接続します。

1. The Trade Deskのアカウントチームにお問い合わせいただき、GenStudio for Performance MarketingからThe Trade Deskのアカウントにクリエイターを公開するためのアクセス権をリクエストしてください。 アクティベーションに使用する広告主ID、シート、パートナーの詳細を確認します。
1. The Trade Desk アカウントチームからAPI トークンまたは資格情報を取得し、トークンがターゲット広告主アカウントのクリエイティブ公開権限をサポートしていることを確認します。
1. GenStudio for Performance Marketingで、**[!UICONTROL Settings]** > **[!UICONTROL Channels]**&#x200B;に移動し、**[!UICONTROL The Trade Desk]** タイルの&#x200B;**[!UICONTROL Connect]**&#x200B;をクリックします。 アカウント名、広告主ID、API トークンまたは資格情報を入力し、接続を保存します。

接続が失敗した場合は、The Trade Desk アカウントチームにAPI アクセスが有効になっており、トークンに正しい広告主と座席権限があることを確認してください。

## Trade Deskの設定フィールドには

承認されたアセットは[!DNL Content]でレビューと承認が完了しているため、アクティブ化中はロックされ、編集できません。 次の項目を編集できます。

* **テキストフィールド**: トラッキング ID （プラットフォームのクリエイティブ名として使用）
* **プラットフォーム設定フィールド**：アカウント、キャンペーン

現時点では、The Trade Deskへのアクティベーションは、シングルアセットの静的ディスプレイ広告のみをサポートしています。
