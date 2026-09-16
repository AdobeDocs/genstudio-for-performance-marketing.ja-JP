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
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 5%
---
# Adobe GenStudio for Performance Marketing のアクティブ化

GenStudio for Performance Marketing [!DNL Activate]では、MetaやLinkedInなどの有料広告チャネルに広告エクスペリエンスを準備して配信できます。 _アクティベーション_&#x200B;は、承認済みの広告エクスペリエンスとそのアセットを取り込み、特定のチャネルに必要な設定を適用し、非アクティブでオフのステータスでそのチャネルに直接配信します。 そこから、広告が公開される前に、チャネルの独自の広告マネージャーで最終レビューをおこなうことができます。

[!DNL Activate]は、エクスペリエンスをチャネルに直接配信するので、ファイルをエクスポートしたり、チャネルの独自の広告マネージャーに手動でアップロードしたりする必要はありません。

広告エクスペリエンスをそのチャネルにアクティベートするには、GenStudioのシステムマネージャーまたはエディターが各有料広告チャネルの広告アカウントを接続する必要があります。

## Activate の機能

[!DNL Activate]を使用して、ターゲットの有料広告チャネルの広告エクスペリエンスを準備します。 単一のアクティベーションテーブルで[複数の有料広告チャネルをまたいで](create-activation.md) エクスペリエンスを一括でアクティベートします。 次に、[ アクティベーションを管理](manage-activations.md)して、アクティベートされたすべてのエクスペリエンスのステータスと詳細を確認します。

>[!VIDEO](https://video.tv.adobe.com/v/3503538?learn=on)

### コンテンツから承認済みエクスペリエンスを活用

[!DNL Content]から1つ以上の承認済み、公開済みエクスペリエンスを選択するか、[!DNL Activate]のランディングページから開始します。 以前のバージョンの[!DNL Activate]とは異なり、単一のアクティベーションテーブルには、複数の有料広告チャネルのエクスペリエンスを、広告の形式とチャネル別に整理して一度に含めることができます。

>[!NOTE]
>
>[!DNL Content]は、**チャネル**&#x200B;のMetaやLinkedInなどの宛先を呼び出します。 [!DNL Activate]は、同じ宛先を&#x200B;**プラットフォーム**&#x200B;と呼び出します（例：**[!UICONTROL プラットフォーム設定]**）。 2つの用語は同じことを指している。

### 広告とプラットフォームの設定の詳細

アクティベーションテーブルの各行は、1つの広告を表します。 承認済みのクリエイティブアセット、見出し、本文は、レビューと承認が済んでいるためロックされています。 Call-to-actionのテキスト、リンク先URL、広告アカウント、キャンペーン、広告セットなどのプラットフォーム設定の詳細など、残りのフィールドを編集できます。 一度に1行のフィールドを編集するか、複数の行を選択して共有フィールドを一括編集します。

### エクスペリエンスのレビューと広告チャネルへの公開

すべての行に[!UICONTROL  アクティベートの準備完了]が表示されていることを確認します。 [!DNL Activate]は、フィールドが見つからないか無効であり、互換性のないCTAが含まれており、トラッキング IDが[!UICONTROL 要注意]として重複していることを示しています。 すべての行の準備ができたら、**[!UICONTROL プラットフォームに送信]**&#x200B;をクリックして、テーブル内のすべての広告を公開します。 [!DNL Activate]は、各広告のステータスをほぼリアルタイムでレポートし、正常に公開された広告には、宛先プラットフォームのネイティブ広告マネージャーの広告へのディープリンクが含まれます。 失敗した広告はエラーメッセージを返し、再試行できます。
