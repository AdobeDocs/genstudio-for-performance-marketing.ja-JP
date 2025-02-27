---
title: 画像機能
description: GenStudio for Performance Marketingで使用される属性カテゴリの画像機能について説明します。
feature: Insights, Attributes, Generative AI
source-git-commit: c15140ed3fe3d07e9112e9ad4781cb8fcf65045d
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 0%

---

# 画像機能

画像の特徴は、[!DNL Insights] での分析に使用される、画像内の個別のわかりやすい要素やパターンを表します。 これらの機能は、視覚的なコンテンツを分類して理解するのに役立ち、より正確で詳細なインサイトを可能にします。 スタイル、色、オブジェクトなどのさまざまな属性を識別することで、AI は画像の包括的な分析を提供し、より良い意思決定と戦略の策定に役立ちます。

## スタイルの検出

_画像スタイル_ を決定することは、他の画像特性を識別するための基盤となります。 AI が適切な解析手法を適用し、関連性の高い特徴を認識することで、画像をより包括的に理解することができます。 各スタイルには、画像の認識および分析方法に影響を与える明確な視覚的特性があります。

画像スタイルが `photograph` として識別された場合、AI は `camera settings`、`camera proximity` および `Photography genres` の追加の特性を分析します。 これらの特性は写真に固有のもので、画像の構成と品質に関するより深い洞察を提供します。 Adobeの [28 種類の写真スタイル ](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html) 写真について学ぶ _を参照し、人気のある写真の種類と基本的な用語について学びます_。

画像スタイルが `sketch` または `digital cartoon` として識別された場合、異なる特性セットが関係する可能性があります。 この階層的アプローチにより、分析のコンテキストが正確になり、調査する画像のタイプに合わせて調整されます。

## 画像機能を検索

**特定の属性カテゴリの画像を表示するには**:

1. _[!DNL Insights]_で、**[!UICONTROL 属性]**ビューを選択します。

1. 「**[!UICONTROL イメージ]**」を選択して、テーブル表示を変更します。

1. **[!UICONTROL 属性カテゴリ]** リストから、`Scenes` などの画像機能を選択します。

1. そのカテゴリを共有する画像の詳細ビューの属性を選択します。

   例えば、`Scenes` カテゴリは、属性として `restaurant` を持つ場合があります。

1. _属性の詳細_ ページには、この属性を持つすべての画像が一覧表示されます。

次の表に、GenStudio for Performance Marketing AI で認識される画像の機能カテゴリを示します。 アセットに対して検出された属性リストは完全なものではありません。 豊富な機能セットを含むAssetsは、AI によって特定された 3 つの最も支配的な機能に制限される場合があります。

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| カテゴリ | 説明 | 例 |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 注意分布 | ビューアの注意のレベルは、画像に広がり、画像の様々な領域がどのくらいフォーカスを受け取るかを示します。 高い値に設定すると、焦点を合わせる領域が 1 つもなくなり、低い値に設定すると、1 つまたは 2 つの焦点位置に視聴者の注意が引かれます。 | `high`、`medium`、`low`<p>左側に `low` 分布の例、右側に `high` 分布の例：<p>![ 低分布および高分布のボールプレイ ](/help/assets/category/image-attn-lowhigh.png " 低分布および高分布の違い "){width="200" zoomable="yes"} |
| カメラアングル | カメラが被写体を捉える遠近感は、見る人のイメージやイメージの見方を左右します。 画像スタイルが `photograph` の場合、この特性が識別されます。 | `Low angle`、`High angle`、`Eye level`、`Overhead view`、`Dutch angle`、`Bird's eye view`<p>`eye level` の例：<p>![ 眼の高さ ](/help/assets/category/image-camera-angle.png " 異なる角度から座っている人 "){width="200" zoomable="yes"} |
| カメラ設定 | 最終的なイメージの外観と画質に影響する、カメラのコントロールの特定の調整と設定。 画像スタイルが `photograph` の場合、この特性が識別されます。 | `Fast shutter speed`, `Long exposure`, `Bokeh blur`, `Motion blur`, `Tilt-shift blur`, `Flash`, `Wide-angle`, `Black and white`, `Surreal`, `Double-exposure`, `Macro`, `Normal mode`<p>`macro` 設定の例：<p>![ マクロクローズアップショット ](/help/assets/category/image-subject-distance.png " クローズアップフラワーとジュエルミツバチのマクロ設定 "){width="200" zoomable="yes"} |
| カラーとトーン | 画像内のカラーと色調の品質。 異なる画像レイヤーの 40 色の事前定義済みセットから最大 3 色を識別します。<p>**[!UICONTROL 前景色]** – 画像の前面レイヤーの色 <br>**[!UICONTROL  背景色 ]**– 画像の背面レイヤーの色 | カラー値：`Red`、`Dark Red`、`Green`、`Bright Green`、`Dark Green`、`Light Green`、`Mud Green`、`Blue`、`Dark Blue`、`Light Blue`、`Royal Blue`、`Black`、`White`、`Off White`、`Gray`、`Yellow`、`Dark Gray`、`Silver`、`Cream`、`Magenta`、`Cyan`、`Mustard`、`Khaki` `Brown` `Dark Brown` `Violet` `Pink` `Dark Pink` `Maroon` `Tan` `Purple` `Lavender` `Turquoise` `Plum` `Gold` `Emerald` `Orange` `Beige` `Lilac` `Olive` |
| 色温度 | 画像内の色の一般的な暖かさや涼しさを表します。 | トーンまたは温度の値：`warm`、`cool`、`neutral`<br>![ カラーおよびクールなトーン ](/help/assets/category/image-color-temp.png " クールな背景と複数のカラーオブジェクトを備えたカラー温度 "){width="200" zoomable="yes"} |
| コンテンツ密度 | 画像内の視覚要素と詳細の集中。視覚空間にどれだけの情報が詰められているかを示します。<p>画像の様々な領域に視聴者の焦点がどのように広がっているかを測定する注意分布とは異なり、コンテンツ密度は、存在する視覚情報の量に焦点を当てます。 コンテンツ密度が高いほど、存在する要素が多くなります。 | `high`、`medium`、`low`<p>左側の `low` 密度と右側の `high` 密度の例：<p>![ 低密度および高密度のボールプレイ ](/help/assets/category/image-attn-lowhigh.png " 低密度および高密度の違い "){width="200" zoomable="yes"} |
| 画像スタイル | 写真やスケッチなどの画像の視覚的処理。 AI が画像スタイルを判断すると、他の特性が識別される場合があります。 例えば、画像が写真の場合、カメラ設定、カメラの近接性、照明条件が適用される場合があります。 | `Photograph`, `Sketch`, `Painting`, `Digital cartoon`, `Infographics`, `Graphic design`, `Collage`, `Software screenshot`<p>`digital cartoon` 画スタイルの例 ![ 漫画イメージスタイル ](/help/assets/category/image-style.png " 猫のイメージスタイル漫画 "){width="200" zoomable="yes"} |
| 照明条件 | イメージ内の光の質と特性を表し、そのムード、トーン、可視性に影響を与えます。 | `Golden hour`, `Blue hour`, `Midday`, `Overcast`, `Night`, `High-key`, `Low-key`, `Daylighting`, `Incandescent`, `Fluorescent`, `Colorful`, `Studio`<p>条件 `daylighting` 例：<p>![ 昼光条件 ](/help/assets/category/image-lighting.png " 昼光条件における歩道の人と犬 "){width="200" zoomable="yes"} |
| オブジェクト | 画像を構成する 1 つ以上の項目、エンティティ、要素を識別します。 | 値が多すぎますが、例えば、`backpack`、`book`、`hawk`、`glasses`、`fish`、`pencil`、`mountain bike`、`soap` などがあります<p>`toucan` オブジェクトと `bird` オブジェクトの例：<p>![bird, toucan object](/help/assets/category/image-objects-bird.png "Toucan bird object のグラフィックデザイン "){width="200" zoomable="yes"} |
| オリエンテーション | 幅と高さに対する画像の配置。 高さより幅が広い（横）、高さより高い（縦）、幅と高さが等しい（正方形）のいずれかを検出します。 | `landscape`、`portrait`、`square`<p>`square` 向きの例：<p>![ 正方形スケッチ ](/help/assets/category/image-orientation-square.png " 正方形の向きの花のスケッチ "){width="200" zoomable="yes"} |
| ユーザー | 1 人以上の人物が存在する場合、1 つ以上の属性がその人物または画像内の人物を説明できます。 | `person`、`woman`、`man`、`girl`、`boy`、`social group`、`kid`、`crowd`、`people`<p>`woman` と `person` のカテゴリに含まれる人物の例：<p>![ カメラを持つ人 ](/help/assets/category/image-people.png " カメラを管理する人 "){width="200" zoomable="yes"} |
| 写真ジャンル | 画像のキャプチャに使用する被写体やテクニックを検出します（例：`abstract` または `landscape`）（横向きと同じではありません）。 | `Architecture`, `Astro`, `Landscape`, `Pet`, `Interior`, `Wildlife`, `Night`, `Cityscape`, `Seascape`, `Underwater`, `Storm`, `Adventure sports`, `Fashion`, `Portrait`, `Sports`, `Food`, `Street`, `Event`, `Lifestyle`, `Commercial`, `Group` `Abstract` `Minimalist` `Composite`,<p>詳しくは、[ 撮影の種類 ](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html) を参照してください。 |
| シーン | 画像内の設定または環境を識別し、画像がキャプチャされた場所や表示された場所のタイプに関するコンテキストを提供します。 | 値が多すぎますが、例えば、`lake`、`underwater`、`highway`、`hill`、`log cabin`、`island`、`beach`、`lounge` などがあります<p>`snow`、`sky`、`winter`、`mountain` のシーンがヘルメットに反射する例：<p>![ 冬の雪のシーン ](/help/assets/category/image-scenes.png " 冬、雪、空、山のシーンの反射 "){width="200" zoomable="yes"} |
| 被写体距離 | カメラと画像の被写体との間の距離。 | `close up`、`mid shot`、`long shot`<p>`closeup shot` の例：<p>![ クローズアップショット ](/help/assets/category/image-subject-distance.png " フラワーとミツバチをクローズアップ "){width="200" zoomable="yes"} |
| スタイル | LightroomやPhotoshopで使用される視覚的処理を画像要素に適用します。 | `design`, `illustration`, `logo`, `square`, `cartoon`, `art`, `circle`, `circular`<p>`circular` スタイルの例：<p>![ サンゴ礁における円形の入り口 ](/help/assets/category/image-styles-circular.png " サンゴ礁における円形の入り口 "){width="200" zoomable="yes"} |
| タグ | 特定の分類に該当しないその他の画像特性を検出します。 タグは、画像に関する追加のコンテキストとメタデータを提供します。 例えば、AI が画像内の `helmet` および `motorobike` オブジェクトを検出し、タグとして `riding` を含めることができます。 | 値が多すぎますが、例えば、`construction`、`gothic`、`healing`、`military`、`selfie`、`football`、`typing`、`dancer`、`dancing` などがあります<p>`dancer` タグと `dancing` タグの例：<p>![ 舞踊及び舞踊家用 ](/help/assets/category/image-tags.png " タグ "){width="200" zoomable="yes"} |
