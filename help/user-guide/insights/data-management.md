---
title: データ管理
description: GenStudio for Performance Marketingでのデータの取得と保存  [!DNL Insights]  ついて説明します。
feature: Reporting and Insights
level: Experienced
role: Admin, Developer
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
TQID: https://experienceleague.adobe.com/HM2e0Yq2uwTpKtK-z8gHs0hDFrsJS6koQBqoNoKJK0Y
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: e0aa398c-6185-4e77-8cf7-2561c578c181
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: d3cdead0-685a-4489-9250-4bb709942f66
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 249
ht-degree: 0%

---

# データ管理

GenStudio for Performance Marketingでは、Adobe Experience Platform（AEP）を使用して、[!DNL Insights] を強化する指標とメタデータのデータ取り込みとストレージを行います。 AEPでは _スキーマ_ を使用して、データ構造とデータ収集の保存および管理のための _データセット_ を定義します。

## データ接続

GenStudio for Performance Marketingでは、Customer Journey Analytics（CJA）を使用して、1 つ以上のAEP データセットへの接続を作成することで、複数のデータソースを集計します。 CJAでは、これらのデータ接続を使用して、[!DNL Insights] で指標を分析するためのデータビューを作成します。

>[!BEGINSHADEBOX]

**データ接続に関する重要な情報**

[Adobe システム管理者 &#x200B;](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager) の場合は、GenStudio for Performance MarketingをサポートするAEP サンドボックス管理コンポーネントおよびデータレイクコンポーネントへのアクセスを許可する使用権限がある可能性があります。

>[!WARNING]
>
>AEPで実稼動サンドボックスをリセットすると、すべてのデータ接続が削除され、[!DNL Insights] が機能しなくなります。

GenStudio for Performance Marketingを確実に動作させるために必要な、次のデータ接続については、注意して削除しないでください。

- プレフィックスが `GS Insights` のAEP データセット
- `GS Insights` プレフィックスが付いたAEP スキーマ、クラス、フィールドグループ
- カスタムフィールドグループ `timestamp for metadata`
- AEP接続：`GS Insights` プレフィックスが付いたデータフロー
- AEP Connections:GS Insights アカウント

AEPでデータコンポーネントを削除する前に、_Customer Journey Analytics_ ガイドの [&#x200B; 影響の削除 &#x200B;](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion) を参照してください。

>[!ENDSHADEBOX]

## データ保持ポリシー

GenStudio for Performance Marketingはチャネルデータを 13 か月間保持します。 この保持ポリシーには、最初の接続中に取り込まれた 6 か月のデータが含まれており、包括的な履歴データの分析とレポートを確実に行います。

[&#x200B; 有料メディアアカウントの接続 &#x200B;](/help/user-guide/connectors/connect-channel.md) を参照してください。
