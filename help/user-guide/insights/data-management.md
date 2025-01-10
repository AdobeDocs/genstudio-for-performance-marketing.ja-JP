---
title: データ管理
description: GenStudio for Performance Marketingでのインサイトのデータ取得と保存について説明します。
feature: Insights
level: Experienced
role: Admin
last-substantial-update: 2025-1-7
source-git-commit: 5dbe645f2ccf033f515da22ffdcce86edcb9fb24
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# データ管理

GenStudio for Performance Marketingでは、Adobe Experience Platform（AEP）を使用して、[!DNL Insights] を強化する指標やメタデータのデータ取得とストレージを行います。 AEP では _スキーマ_ を使用してデータ構造を定義し、データコレクションを保存および管理する _データセット_ を定義します。

## データ接続

GenStudio for Performance Marketingでは、Customer Journey Analytics（CJA）を使用し、1 つ以上の AEP データセットへの接続を作成して、複数のデータソースを集計します。 CJA は、これらのデータ接続を使用して、[!DNL Insights] で指標を分析するためのデータビューを作成します。

>[!BEGINSHADEBOX]

**データ接続に関する重要な情報**

[Adobeシステム管理者 ](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager) の場合は、GenStudio for Performance Marketingをサポートする AEP サンドボックス管理コンポーネントおよびデータレイクコンポーネントへのアクセスを許可する使用権限がある可能性があります。

>[!WARNING]
>
>AEP で実稼動サンドボックスをリセットすると、すべてのデータ接続が削除され、[!DNL Insights] が機能しなくなります。

GenStudio for Performance Marketingを確実に動作させるために必要な、次のデータ接続については、注意して削除しないでください。

- プレフィックスが `GS Insights` の AEP データセット
- プレフィックスに `GS Insights` が付いた AEP スキーマ、クラスおよびフィールドグループ
- カスタムフィールドグループ `timestamp for metadata`
- AEP 接続：`GS Insights` プレフィックスが付いたデータフロー
- AEP Connections:GS Insights アカウント

AEP でデータコンポーネントを削除する前に、_Customer Journey Analytics_ ガイドの [ 影響を削除 ](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion) を参照してください。

>[!ENDSHADEBOX]

## データ保持ポリシー

GenStudio for Performance Marketingはチャネルデータを 13 か月間保持します。 この保持ポリシーには、最初の接続中に取り込まれた 6 か月のデータが含まれており、包括的な履歴データの分析とレポートを確実に行います。

[ チャネル広告アカウントの接続 ](/help/user-guide/insights/connect-channel.md) を参照してください。
