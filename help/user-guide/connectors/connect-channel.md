---
title: 有料メディアアカウントを接続
description: Adobe GenStudio for Performance Marketingで有料メディアアカウントを接続して、広告やメディアをアクティブ化およびモニタリングします。
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights, Delivery and Activation
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
source-git-commit: 2f18b273684a9fe9b9b8903838ae09f5cd2b7842
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# 有料メディアアカウントを接続

_有料メディアアカウント_ とは、企業が有料広告キャンペーンを管理および実行するサードパーティの広告プラットフォーム上のアカウントを指します。 これらのアカウントは、ソーシャルメディアプラットフォームやディスプレイネットワークなどの有料チャネルを通じて、製品、サービス、ブランドを宣伝するために使用されます。 有料メディアアカウントをGenStudio for Performance Marketingに接続すると、データ交換の効率化、[ インサイト ](/help/user-guide/insights/overview.md) でのキャンペーンのパフォーマンスのモニタリング、[ アクティブ化 ](/help/user-guide/activation/overview.md) による新規広告プレースメントの配信を行うことができます。

**有料メディアアカウントに接続するには**:

1. 省略記号 **[!UICONTROL ...をクリックします。その他]** 左下のナビゲーションにあります。

1. 歯車アイコンで **[!UICONTROL 設定]** を選択します。

1. _[!UICONTROL 設定]_ で、「_[!UICONTROL Data connectors]_」セクションからコネクタタイプを選択し、「**[!UICONTROL 接続]**」をクリックします。

   オプションで、接続されているアカウントがある場合、「_接続されているアカウント_」をクリックして、アカウント名、詳細およびステータスのリストを表示できます。

1. 前提条件を確認し、接続手順を続行するために選択したコネクタタイプを以下に示します。

   - [Google Campaign Manager 360](google-cm360.md)
   - [メタ広告](meta-ads.md)

## 有料メディア接続

GenStudio for Performance Marketingは、好みのマーケティングプラットフォームと統合するために、様々なコネクタタイプをサポートしています。 各コネクタタイプには、特定の前提条件と、接続を正常に完了するために実行するセットアップ手順があります。

## データ取り込み

GenStudio for Performance Marketingは、最初に、最新の 6 か月間の履歴データを読み込みます。 これにより、トレンドの分析、パフォーマンスの評価、十分な情報に基づいた意思決定を行うための関連するインサイトにすぐにアクセスできます。 アカウントのデータ量によっては、取り込みプロセスに 1～5 日かかる場合があります。

>[!BEGINSHADEBOX]

**データの取り込みと保持のポリシー**

GenStudio for Performance Marketingはチャネルデータを 13 か月間保持します。 この保持ポリシーには、最初の接続中に取り込まれた 6 か月のデータが含まれており、包括的な履歴データの分析とレポートを確実に行います。

>[!ENDSHADEBOX]
