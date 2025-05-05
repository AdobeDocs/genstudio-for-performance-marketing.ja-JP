---
title: ビデオ機能
description: GenStudio for Performance Marketingで使用される属性カテゴリのビデオ機能について説明します。
level: Intermediate
feature: Reporting and Insights, Video Attributes, Generative AI
exl-id: 0dfdd735-b365-4a15-a6fd-e981697442cb
source-git-commit: c742fb33a04b36da35036a4554a475141fce8b01
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 1%

---

# ビデオ機能

ビデオの特徴は、[!DNL Insights] で分析するために、ビデオ内の個別のわかりやすい要素、サウンドまたはパターンを表します。 これらの機能は、ビデオコンテンツの分類と理解に役立ち、より正確で詳細なインサイトを得ることができます。 AI は、オーディオムード、音楽ジャンル、オブジェクトなどのさまざまな属性を特定することで、ビデオの包括的な分析を提供し、より良い意思決定と戦略の策定に役立ちます。

## オーディオ検出

GenStudio for Performance Marketingのオーディオ検出では、ビデオのオーディオトラックを分析して様々な属性を特定します。 この検出プロセスは、存在する音声の種類を特定し、特定のジャンルまたは音楽のカテゴリをタグ付けし、音声からキーワードを抽出することで、音声の全体的なムードを決定します。 これらのオーディオ要素を理解することで、AI はビデオのコンテンツとコンテキストに関するより深いインサイトを提供し、分析と分類プロセス全体を強化できます。

## ビデオ機能を検索

**ビデオをプレビューしてオーディオのサンプルを再生するには**:

1. _[!DNL Insights]_&#x200B;で、**[!UICONTROL 属性]**&#x200B;ビューを選択します。

1. **[!UICONTROL ビデオ]** を選択して、テーブルの表示を変更します。

1. **[!UICONTROL 属性カテゴリ]** リストからフィーチャーを選択します。 音声の例の場合は、「音楽ジャンル **を選択し** す。

1. そのカテゴリを共有するビデオの詳細ビューの属性を選択します。

   例えば、`Music genre` カテゴリは、属性として `electronic` を持つ場合があります。

1. _属性の詳細_ ページには、この属性を持つすべてのビデオが一覧表示されます。 リスト内の任意のビデオの上にマウスポインターを置くと、ビデオのプレビューが開始されます。

1. （ビデオプレビューの左下隅にある） **ミュート解除** ボタンを切り替えて、ビデオプレビューのオーディオを聴きます。

次の表に、GenStudio for Performance Marketing AI で認識されるビデオ機能カテゴリを示します。 メディアコンテンツについて検出された属性リストは、すべてを網羅しているわけではありません。 豊富な機能セットを含むメディアは、AI によって特定された 3 つの最も支配的な機能に制限される場合があります。

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| カテゴリ | 説明 | 例 |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| オーディオムード | `calm`、`upbeat`、`tense` など、オーディオトラックの全体的な感情的なトーンまたは雰囲気を決定します。 | `Energetic`、`Happy`、`Emotional Ambient/atmospheric`、`Relaxing`、`Dramatic`、`Expressive/characterful`、`Intense`、`Slow`、`Neutral` |
| 音声タイプ | 1 つ以上のオーディオコンテンツタイプ（`music` や `speech` など）が存在するビデオをタグ付けします。 | `Music`、`Speech`、`Silence`、`Special effects`、`Ambience` |
| カテゴリ | ビデオを 1 つ以上の広範なコンテンツカテゴリに分類します。 | `Entertainment`, `Sports`, `Music`, `Gaming`, `Howto tutorials`, `Fashion and style`, `Film and animation`, `Science and technology`, `Autos and vehicles`, `Pets and animals`, `People and blogs`, `News and politics`, `Social causes and activism`, `Travel and events`, `Education`, `Sales and offers` |
| 音楽カテゴリ | 音楽がビデオに含まれる場合の、音楽のジャンルの大分類。 ジャンルは、音楽の一般的なタイプ、例えば `contemporary` や `traditional` のスタイルを識別するのに役立ちます。 | `Contemporary/pop music`、`Traditional/folk-based music`、`Instrumental/orchestral music`、`Rock music`、`Acoustic/unplugged music`、`Specialised/occasional music`、`Experimental/unique music` |
| 音楽ジャンル | ビデオ内に音楽が存在する場合の音楽スタイルの特定の分類。これにより、`electronic` や `jazz` など、音楽のより詳細な識別が可能になります。 | `electronic`, `hip-hop`, `dance`, `novelty`, `rock`, `world`, `reggae`, `pop`, `film`, `jazz`, `background`, `latin` |
| オブジェクト | ビデオに表示される 1 つ以上の項目、エンティティ、要素を識別します。 | 値が多すぎますが、例えば、`backpack`、`book`、`hawk`、`glasses`、`fish`、`pencil`、`mountain bike`、`soap` などがあります |
| オリエンテーション | 幅と高さに対するビデオの配置。 高さより幅が広い（横）、高さより高い（縦）、幅と高さが等しい（正方形）のいずれかを検出します。 | `landscape`、`portrait`、`square` |
| ユーザー | 少なくとも 1 人のユーザーが存在する場合、1 つ以上の属性がそのユーザーまたはビデオに存在するユーザーを説明できます。 | `person`、`woman`、`man`、`girl`、`boy`、`social group`、`kid`、`crowd`、`people` |
| シーン | ビデオ内の設定または環境を識別し、ビデオが作成された場所や表示される場所のタイプに関するコンテキストを提供します。 | 値が多すぎますが、例えば、`lake`、`underwater`、`highway`、`hill`、`log cabin`、`island`、`beach`、`lounge` などがあります |
| スタイル | After EffectsやLightroomで使用されるものなど、ビデオ要素に適用される視覚的処理を検出します。 | `design`, `illustration`, `logo`, `square`, `cartoon`, `art`, `matte`, `neon` |
| タグ | 特定の分類に該当しないその他のビデオ特性を検出します。 タグは、ビデオに関する追加のコンテキストとメタデータを提供します。 | 値が多すぎますが、例えば、`construction`、`gothic`、`healing`、`military`、`selfie`、`football`、`typing`、`dancer`、`dancing` などがあります |
