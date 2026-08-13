---
title: ビデオ機能
description: GenStudio for Performance Marketingで使用される属性カテゴリのビデオ機能について説明します。
level: Intermediate
feature: Reporting and Insights, Video Attributes, Generative AI
exl-id: 0dfdd735-b365-4a15-a6fd-e981697442cb
TQID: https://experienceleague.adobe.com/s-8h3ODnNuRyebiDTLZGQORJzPnPOcPzQjIhWBmpk-c
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: c95c94c1-727b-457a-9184-a4dda4c95ab2id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
subfeature_v2: id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 683
ht-degree: 17%

---

# ビデオ機能

ビデオの特徴は、ビデオ内の明確で有益な要素、サウンド、またはパターンを表し、[!DNL Insights]を使用して分析します。 これらの機能は、ビデオコンテンツの分類と理解に役立ち、より正確で詳細なインサイトを実現します。 オーディオムード、音楽ジャンル、オブジェクトなどの様々な属性を特定することで、AIは動画の包括的な分析を提供し、より優れた意思決定と戦略の策定に役立てることができます。

## オーディオ検出

GenStudio for Performance Marketingの音声検出では、ビデオのオーディオトラックを分析して、様々な属性を識別します。 この検出プロセスは、存在するオーディオの種類を特定し、特定のジャンルまたは音楽のカテゴリーをタグ付けし、音声からキーワードを抽出することによって、オーディオの全体的なムードを決定する。 これらのオーディオ要素を理解することで、AIは動画のコンテンツとコンテキストに関するより深いインサイトを提供し、全体的な分析と分類プロセスを強化します。

## ビデオ機能を検索

**ビデオをプレビューし、オーディオのサンプルを聴くには**:

1. _[!DNL Insights]_で、**[!UICONTROL 属性]**ビューを選択します。

1. **[!UICONTROL ビデオ]**&#x200B;を選択して、テーブル表示を変更します。

1. **[!UICONTROL 属性カテゴリ]** リストから機能を選択します。 オーディオの例の場合は、**音楽ジャンル**&#x200B;を選択します。

1. 属性を選択すると、そのカテゴリを共有するビデオの詳細ビューが表示されます。

   例えば、`Music genre` カテゴリには、属性として`electronic`が含まれている場合があります。

1. _属性の詳細_ ページには、この属性を持つすべてのビデオが一覧表示されます。 リスト内の任意のビデオの上にマウスポインターを置くと、ビデオのプレビューが開始されます。

1. 「**ミュート解除**」（ビデオプレビューの左下隅）ボタンを切り替え、ビデオプレビューのオーディオを聴きます。

次の表に、GenStudio for Performance Marketing AIで認識されるビデオ機能カテゴリを示します。 メディアコンテンツの検出済み属性リストが完全ではありません。 豊富な機能セットを含むメディアは、AIが特定する3つの主要な機能に制限される場合があります。

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| カテゴリ | 説明 | 例 |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| オーディオムード | オーディオトラックの全体的な感情的なトーンまたは雰囲気（`calm`、`upbeat`、または`tense`など）を決定します。 | `Energetic`, `Happy`, `Emotional Ambient/atmospheric`, `Relaxing`, `Dramatic`, `Expressive/characterful`, `Intense`, `Slow`, `Neutral` |
| オーディオタイプ | `music`や`speech`など、1つ以上の音声コンテンツタイプが存在するビデオにタグ付けします。 | `Music`, `Speech`, `Silence`, `Special effects`, `Ambience` |
| カテゴリ | ビデオを1つ以上の幅広いコンテンツカテゴリに分類します。 | `Entertainment`, `Sports`, `Music`, `Gaming`, `Howto tutorials`, `Fashion and style`, `Film and animation`, `Science and technology`, `Autos and vehicles`, `Pets and animals`, `People and blogs`, `News and politics`, `Social causes and activism`, `Travel and events`, `Education`, `Sales and offers` |
| 音楽カテゴリ | 音楽がビデオに存在する場合の音楽ジャンルの幅広い分類。 ジャンルは、`contemporary`や`traditional`のスタイルなど、一般的な種類の音楽を特定するのに役立ちます。 | `Contemporary/pop music`, `Traditional/folk-based music`, `Instrumental/orchestral music`, `Rock music`, `Acoustic/unplugged music`, `Specialised/occasional music`, `Experimental/unique music` |
| 音楽ジャンル | ビデオに音楽が存在する場合の音楽スタイルの特定の分類。これにより、`electronic`や`jazz`など、音楽をより詳細に識別できます。 | `electronic`, `hip-hop`, `dance`, `novelty`, `rock`, `world`, `reggae`, `pop`, `film`, `jazz`, `background`, `latin` |
| オブジェクト | ビデオに表示される1つ以上の項目、エンティティ、および要素を識別します。 | 値が多すぎます。ただし、例として、`backpack`、`book`、`hawk`、`glasses`、`fish`、`pencil`、`mountain bike`、`soap`などがあります。 |
| オリエンテーション | 幅と高さに対するビデオの整列。 高さより広い（横）、幅より高い（縦）、幅と高さが等しい（正方形）かどうかを検出します。 | `landscape`, `portrait`, `square` |
| ユーザー | 少なくとも1人の人物が存在する場合、1つ以上の属性は、その人物またはビデオに存在する人物を表す場合があります。 | `person`, `woman`, `man`, `girl`, `boy`, `social group`, `kid`, `crowd`, `people` |
| シーン | ビデオ内の設定や環境を識別し、ビデオの作成場所や表示される場所の種類に関するコンテキストを提供します。 | 値が多すぎます。ただし、例として、`lake`、`underwater`、`highway`、`hill`、`log cabin`、`island`、`beach`、`lounge`などがあります。 |
| スタイル | After EffectsやLightroomで使用されるビデオ要素など、ビデオ要素に適用される視覚的処理を検出します。 | `design`, `illustration`, `logo`, `square`, `cartoon`, `art`, `matte`, `neon` |
| タグ | 特定の分類に該当しないその他のビデオ特性を検出します。 タグは、ビデオに関する追加のコンテキストとメタデータを提供します。 | 値が多すぎます。ただし、例として、`construction`、`gothic`、`healing`、`military`、`selfie`、`football`、`typing`、`dancer`、`dancing`などがあります。 |
