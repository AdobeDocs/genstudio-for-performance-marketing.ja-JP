---
title: データ管理
description: GenStudio for Performance Marketingでの [!DNL Insights] のデータの取り込みと保存について説明します。
feature: Reporting and Insights
level: Experienced
role: Admin, Developer
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
TQID: https://experienceleague.adobe.com/HM2e0Yq2uwTpKtK-z8gHs0hDFrsJS6koQBqoNoKJK0Y
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: c95c94c1-727b-457a-9184-a4dda4c95ab2id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: e0aa398c-6185-4e77-8cf7-2561c578c181
subfeature_v2: id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: d3cdead0-685a-4489-9250-4bb709942f66id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 249
ht-degree: 2%

---

# データ管理

GenStudio for Performance Marketingは、Adobe Experience Platform （AEP）を使用して、[!DNL Insights]を強化する指標とメタデータのデータ取り込みと保存を行います。 AEPでは、_スキーマ_&#x200B;を使用してデータ構造を定義し、_データセット_&#x200B;を使用してデータコレクションを保存および管理します。

## 柔軟な接続

GenStudio for Performance Marketingでは、Customer Journey Analytics（CJA）を使用して、1つ以上のAEP データセットへの接続を作成することで、複数のデータソースを集約します。 CJAでは、これらのデータ接続を使用して、[!DNL Insights]の指標を分析するためのデータビューを作成します。

>[!BEGINSHADEBOX]

**データ接続に関する重要な情報**

[Adobe system administrator](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager)の場合、GenStudio for Performance MarketingをサポートするAEP サンドボックス管理およびデータレイクコンポーネントへのアクセスを許可する使用権限が付与されている可能性があります。

>[!WARNING]
>
>AEPで実稼動サンドボックスをリセットすると、すべてのデータ接続が削除され、[!DNL Insights]が動作しなくなります。

GenStudio for Performance Marketingが確実に動作するために必要な次のデータ接続は削除しないでください。

- 接頭辞`GS Insights`が付いたAEP データセット
- AEP スキーマ、クラス、およびフィールドグループの先頭に`GS Insights`を付ける
- カスタムフィールドグループ `timestamp for metadata`
- AEP Connections: データフローの先頭に`GS Insights`を付ける
- AEP Connections: GS Insights アカウント

AEPのデータコンポーネントを削除する前に、_Customer Journey Analytics_ ガイドの[ インプリケーションの削除](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion)を参照してください。

>[!ENDSHADEBOX]

## データ保持ポリシー

GenStudio for Performance Marketingは、チャネルデータを13か月保持します。 この保持ポリシーには、最初の接続中に取り込まれた6か月間のデータが含まれ、包括的な履歴データ分析とレポートが保証されます。

[有料メディアアカウントの接続](/help/user-guide/connectors/connect-channel.md)を参照してください。
