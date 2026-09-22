---
title: Activate の概要
description: Adobe CX Enterprise およびサードパーティアプリケーションを使用してコンテンツをアクティブ化する方法について説明します。
level: Beginner
feature: Ad Activation
exl-id: 365fe253-d189-467e-a723-f54cd74ff60b
TQID: https://experienceleague.adobe.com/-Nal0YqjTzKw4g2SM3IuMf0a13e87CWdTqBZPd0dBkU
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
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: ht
source-wordcount: '413'
ht-degree: 100%
---
# Adobe GenStudio for Performance Marketing のアクティブ化

GenStudio for Performance Marketing [!DNL Activate] は、Meta や LinkedIn などの有料広告チャネルに向けて広告エクスペリエンスを準備および配信するための場所です。_アクティベーション_&#x200B;では、承認済みの広告エクスペリエンスとそのアセットを取り込み、特定のチャネルに必要な設定を適用して、非アクティブでオフのステータスでそのチャネルに直接配信します。そこから、広告を公開する前に、チャネル独自の広告マネージャーで最終レビューを行うことができます。

[!DNL Activate] は、エクスペリエンスをチャネルに直接配信するので、ファイルの書き出しや、チャネル独自の広告管理マネージャーへの手動アップロードを行う必要はありません。

有料広告チャネルに対して広告エクスペリエンスをアクティブ化する前に、GenStudio システムマネージャーまたはエディターでこのチャネルの広告アカウントを接続する必要があります。

## アクティブ化の機能

[!DNL Activate] を使用して、ターゲットの有料広告チャネルの広告エクスペリエンスを準備します。単一のアクティベーションテーブルで、複数の有料広告チャネルをまたいで[エクスペリエンスを一括でアクティブ化します](create-activation.md)。次に、[アクティベーションを管理](manage-activations.md)して、アクティブ化したすべてのエクスペリエンスのステータスと詳細を確認します。

>[!VIDEO](https://video.tv.adobe.com/v/3503538?learn=on)

### 承認済みのエクスペリエンスを Content からアクティブ化

[!DNL Content] から 1 つ以上の承認済みで公開済みのエクスペリエンスを選択するか、[!DNL Activate] ランディングページから開始します。[!DNL Activate] の以前のバージョンとは異なり、単一のアクティベーションテーブルに、複数の有料広告チャネルのエクスペリエンスを、広告の形式とチャネル別に整理して一度に含めることができます。

>[!NOTE]
>
>[!DNL Content] では、Meta や LinkedIn などの宛先を&#x200B;**チャネル**&#x200B;と呼びます。[!DNL Activate] では、同じ宛先を&#x200B;**プラットフォーム**&#x200B;と呼びます（例：**[!UICONTROL プラットフォーム設定]**）。2 つの用語は、同じものを指しています。

### 広告とプラットフォーム設定の詳細の指定

アクティベーションテーブルの各行は、1 つの広告を表します。承認済みのクリエイティブアセット、見出し、本文は、既にレビューと承認が完了しているのでロックされています。コールトゥアクションテキストおよび宛先 URL と、広告アカウント、キャンペーン、広告セットなどのプラットフォーム設定の詳細など、残りのフィールドを編集できます。一度に 1 行のフィールドを編集するか、複数の行を選択して共有フィールドを一括編集します。

### エクスペリエンスのレビューと広告チャネルへの公開

すべての行に[!UICONTROL アクティブ化準備完了]が表示されていることを確認します。[!DNL Activate] では、欠落しているフィールドや無効なフィールド、互換性のないコールトゥアクション、重複するトラッキング ID が[!UICONTROL 注意が必要]としてフラグが付けられます。すべての行の準備が整ったら、「**[!UICONTROL プラットフォームに送信]**」をクリックして、テーブル内のすべての広告を公開します。[!DNL Activate] は、各広告のステータスをほぼリアルタイムで報告し、正常に公開された広告には、宛先プラットフォームのネイティブ広告管理マネージャーの広告へのディープリンクが含まれます。失敗した広告はエラーメッセージを返し、再試行できます。
