---
title: 有料メディアアカウントの接続
description: Adobe GenStudio for Performance Marketingで有料メディアアカウントを接続して、広告やメディアをアクティブ化およびモニタリングします。
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights, Delivery and Activation
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
source-git-commit: 631ad4931363a6acef902bf4626bd79aff683981
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# 有料メディアアカウントの接続

_有料メディアアカウント_ とは、企業が有料広告キャンペーンを管理および実行するサードパーティの広告プラットフォーム上のアカウントを指します。 これらのアカウントは、ソーシャルメディアプラットフォームやディスプレイネットワークなどの有料チャネルを通じて、製品、サービス、ブランドを宣伝するために使用されます。 有料メディアアカウントをGenStudio for Performance Marketingに接続すると、データ交換の効率化、[ インサイトでのキャンペーンのパフォーマンスの監視 ](/help/user-guide/insights/overview.md)、[ アクティブ化を使用した新規広告プレースメントの配信 ](/help/user-guide/activation/overview.md) を行うことができます。

## データ取り込み

GenStudio for Performance Marketingは、最初に、最新の 6 か月間の履歴データを読み込みます。 これにより、トレンドの分析、パフォーマンスの評価および十分な情報に基づいた意思決定を行うための適切なインサイトが得られます。 完全なデータ取り込みプロセスには、アカウントのデータ量に応じて 1～5 日かかる場合があります。

>[!BEGINSHADEBOX]

**データの取り込みと保持のポリシー**

GenStudio for Performance Marketingはチャネルデータを 13 か月間保持します。 この保持ポリシーには、最初の接続中に取り込まれた 6 か月のデータが含まれており、包括的な履歴データの分析とレポート作成を確実に行います。

>[!ENDSHADEBOX]


## 有料メディアアカウントへの接続

1. 省略記号 **[!UICONTROL ...をクリックします。その他]** 左下のナビゲーションにあります。

1. 歯車アイコンで **[!UICONTROL 設定]** を選択します。

1. _[!UICONTROL 設定]_ で、「_[!UICONTROL Data connectors]_」セクションからコネクタタイプを選択し、「**[!UICONTROL 接続]**」をクリックします。

   オプションで、接続されたアカウントが既に存在する場合は、「_接続されたアカウント_」をクリックして、アカウント名、詳細およびステータスのリストを表示できます。

1. コネクタタイプを選択します。 前提条件として選択したコネクタタイプの特定のガイダンスページを確認し、接続手順を完了します。

   - [Google Campaign Manager 360](google-cm360.md)
   - [LinkedIn](linkedin-ads.md)
   - [Meta広告](meta-ads.md)
