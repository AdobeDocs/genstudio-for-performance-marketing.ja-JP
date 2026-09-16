---
title: Meta広告のアクティベート
description: Meta広告エクスペリエンスをアクティベートする方法について説明します。
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
TQID: https://experienceleague.adobe.com/hDR0ngNiGnCXCCOgNhVG8gX4kHGrNvfybPbuMLwYk7U
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
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
source-wordcount: '382'
ht-degree: 0%
---
# Meta広告のアクティベート

Adobe GenStudio for Performance Marketingは、InstagramやFacebookに対するMeta広告エクスペリエンスの活用をサポートしています。

**サポートされている形式**：画像、ビデオ、カルーセル。

[GenStudio for Performance MarketingでMeta エクスペリエンス &#x200B;](/help/user-guide/create/create-meta-ad.md)を作成し、アクティベーション用に選択します。

Meta広告のアクティベーションは、他の有料広告チャネルへのアクティベーションに必要な[同じ一般的な手順](create-activation.md)に従います。 このページでは、Meta固有の前提条件と設定フィールドについて説明します。 GenStudio for Performance MarketingでMeta エクスペリエンスをアクティベートしたら、[Meta Ads Manager](https://adsmanager.facebook.com/)を使用してエクスペリエンスを確認し、広告を起動します。

ほかのチャネルとは異なり、Metaの広告では、1つの広告に複数の縦横比を含めることができます。 エクスペリエンスに複数の縦横比がある場合、[!DNL Activate]は、縦横比ごとに1行ではなく、1行のみを生成します。

GenStudioのシステムマネージャーやエディターは、

## 前提条件

コネクテッドMeta広告アカウントに、Meta広告プラットフォームの以下のコンポーネントで広告を管理するための完全な権限が付与されていることを確認します。

* Meta広告アカウント
* Facebook ページ
* Meta キャンペーン
* Meta広告セット
* Instagram プロフィール（オプション）

ターゲットのMeta キャンペーンと広告セットは、既にMeta Ads Managerに存在する必要があります。 GenStudio for Performance Marketingは現在、キャンペーンや広告セットを作成していません。

## Meta アカウントの連携

エクスペリエンスをアクティベートする前に、GenStudioのシステムマネージャーがMeta アカウントをGenStudio for Performance Marketingに接続する必要があります。 この接続により、GenStudio for Performance MarketingとMeta間でデータを流すことができ、アクティベーションプロセスが可能になります。 [Meta Adsへの接続](/help/user-guide/connectors/meta-ads.md)を参照してください。

Instagram アカウントを選択するには、Meta Business Managerで[使用するInstagram アカウントが、オンボーディング中に選択した同じ広告アカウント &#x200B;](/help/user-guide/connectors/meta-ads.md#connect-an-instagram-account)に接続されていることを確認します。 この接続が見つからない場合、アクティベーション中に&#x200B;**[!UICONTROL Instagram プロファイル]** ドロップダウンメニューにInstagram アカウントが表示されない可能性があります。

同期が完了したら、追加されたアカウントを表示できます。 大量のデータは同期に時間がかかります。

## Meta設定フィールド

承認済みのアセット、見出し、本文のコピーはロックされ、既に[!DNL Content]でレビューと承認が行われているため、アクティブ化中は編集できません。 次の項目を編集できます。

* **テキストフィールド**：説明、Call-to-action、宛先URL、URL パラメーター、トラッキング ID （Meta広告名として使用）
* **プラットフォーム設定フィールド**：広告アカウント、Facebook ページ、Instagram プロファイル、Meta キャンペーン、Meta広告セット
