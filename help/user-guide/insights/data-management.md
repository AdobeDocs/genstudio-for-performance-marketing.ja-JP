---
title: データ管理
description: GenStudio for Performance Marketingでのデータの取得と保存  [!DNL Insights]  ついて説明します。
feature: Reporting and Insights
level: Experienced
role: Admin
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
source-git-commit: 3448392bc3f1496dafdbed2995f40bdba9c91c31
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# データ管理

GenStudio for Performance Marketingでは、Adobe Experience Platform（AEP）を使用して、[!DNL Insights] を強化する指標とメタデータのデータ取り込みとストレージを行います。 AEPでは _スキーマ_ を使用して、データ構造とデータ収集の保存および管理のための _データセット_ を定義します。

## データ接続

GenStudio for Performance Marketingは、Customer Journey Analytics（CJA）を使用し、1 つ以上のAEP データセットへの接続を作成して、複数のデータソースを集計します。 CJA は、これらのデータ接続を使用して、[!DNL Insights] で指標を分析するためのデータビューを作成します。

>[!BEGINSHADEBOX]

**データ接続に関する重要な情報**

[Adobe システム管理者 ](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager) の場合は、GenStudio for Performance MarketingをサポートするAEP サンドボックス管理コンポーネントおよびデータレイクコンポーネントへのアクセスを許可する使用権限がある可能性があります。

>[!WARNING]
>
>AEPで実稼動サンドボックスをリセットすると、すべてのデータ接続が削除され、[!DNL Insights] が機能しなくなります。

GenStudio for Performance Marketingを確実に動作させるために必要な、次のデータ接続については、注意して削除しないでください。

- プレフィックスが `GS Insights` のAEP データセット
- `GS Insights` プレフィックスが付いたAEP スキーマ、クラス、フィールドグループ
- カスタムフィールドグループ `timestamp for metadata`
- AEP接続：`GS Insights` プレフィックスが付いたデータフロー
- AEP Connections:GS Insights アカウント

AEPでデータコンポーネントを削除する前に、_Customer Journey Analytics_ ガイドの [ 影響の削除 ](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion) を参照してください。

>[!ENDSHADEBOX]

## データ保持ポリシー

GenStudio for Performance Marketingはチャネルデータを 13 か月間保持します。 この保持ポリシーには、最初の接続中に取り込まれた 6 か月のデータが含まれており、包括的な履歴データの分析とレポートを確実に行います。

[ チャネル広告アカウントの接続 ](/help/user-guide/insights/connect-channel.md) を参照してください。
