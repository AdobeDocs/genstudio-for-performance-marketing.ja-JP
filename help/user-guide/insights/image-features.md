---
title: 画像の機能
description: GenStudio for Performance Marketingで使用される属性カテゴリの画像機能について説明します。
level: Intermediate
feature: Reporting and Insights, Image Attributes, Generative AI
exl-id: b7e3d202-4085-48a4-a6ba-c950dfd52233
TQID: https://experienceleague.adobe.com/dFi5aYBN8Mr3cYF9tHcAEh2ncDiQdCZiQIPrksmSmdw
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: c95c94c1-727b-457a-9184-a4dda4c95ab2id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
subfeature_v2: id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 1178
ht-degree: 11%

---

# 画像機能

画像の特徴は、画像内の明確で有益な要素またはパターンを表し、[!DNL Insights]を使用した分析に使用されます。 これらの機能は、ビジュアルコンテンツを分類および理解し、より正確で詳細なインサイトを実現するのに役立ちます。 AIは、スタイル、色、オブジェクトなどの様々な属性を識別することで、画像の包括的な分析を提供し、より優れた意思決定と戦略の策定を支援します。

## スタイル検出

_画像スタイル_&#x200B;を決定することは、他の画像特性を識別するための基盤となります。 AIは適切な分析手法を適用して関連する特徴を認識できるため、画像をより包括的に把握できます。 それぞれのスタイルには、画像の認識と分析方法に影響を与える、明確な視覚的特徴があります。

画像スタイルが`photograph`として識別された場合、AIは`camera settings`、`camera proximity`、`Photography genres`の追加特性を分析します。 これらの特性は写真に固有であり、画像の構成と品質に関するより深いインサイトを提供します。 Adobeの&#x200B;_写真_&#x200B;の[28種類の写真スタイル ](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html)を参照し、人気のある写真の種類と基本用語について学習します。

画像スタイルが`sketch`または`digital cartoon`として識別される場合、異なる特性セットが関連する可能性があります。 この階層的なアプローチにより、分析はコンテキストに即して正確であり、調査する特定のタイプの画像に合わせてカスタマイズされます。

## 検索画像の機能

**特定の属性カテゴリの画像を表示するには**:

1. _[!DNL Insights]_で、**[!UICONTROL 属性]**ビューを選択します。

1. **[!UICONTROL 画像]**&#x200B;を選択して、テーブルビューを変更します。

1. `Scenes`など、**[!UICONTROL 属性カテゴリ]** リストから画像機能を選択します。

1. 属性を選択すると、そのカテゴリを共有する画像の詳細ビューが表示されます。

   例えば、`Scenes` カテゴリには、属性として`restaurant`が含まれている場合があります。

1. _属性の詳細_ ページには、この属性を持つすべての画像が一覧表示されます。

次の表に、GenStudio for Performance Marketing AIで認識される画像の機能カテゴリを示します。 メディアコンテンツの検出済み属性リストが完全ではありません。 豊富な機能セットを含むメディアは、AIが特定する3つの主要な機能に制限される場合があります。

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| カテゴリ | 説明 | 例 |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 注意分布 | 視聴者の注意のレベルは、画像全体に広がり、画像の異なる領域にどの程度の焦点を当てることができるかを示します。 分布が高い場合は、単一の領域が視聴者の焦点を支配していないことを意味し、低い場合は、1つまたは2つの焦点が視聴者の注意を引くことを意味します。 | `high`, `medium`, `low`<p>左側の`low`配布と右側の`high`配布の例：<p>![低いボールと高いボールのプレー](/help/assets/category/image-attn-lowhigh.png "低いボールと高いボールのプレー"){width="200" zoomable="yes"} |
| カメラアングル | カメラが被写体をキャプチャする視点。これは、視聴者のイメージの認識と解釈に影響を与えます。 画像スタイルが`photograph`の場合、この特性が識別されます。 | `Low angle`, `High angle`, `Eye level`, `Neutral angle`, `Overhead view`, `Bird's eye view`<p>例：`Overhead view`<p>![ オーバーヘッド表示](/help/assets/category/image-camera-angle.png " オーバーヘッドからのショートパンツのペア "){width="200" zoomable="yes"} |
| カメラ設定 | 最終的な画像の外観と画質に影響を与える、カメラのコントロールの特定の調整と設定。 画像スタイルが`photograph`の場合、この特性が識別されます。 | `Fast shutter speed`, `Long exposure`, `Bokeh blur`, `Motion blur`, `Tilt-shift blur`, `Flash`, `Wide-angle`, `Black and white`, `Double-exposure`, `Macro`, `Normal mode`<p>`Fast shutter speed`設定の例：<p>![高速シャッタースピード ](/help/assets/category/image-camera-setting.png "波に乗る"){width="200" zoomable="yes"} |
| カラーとトーン | 画像内のカラーと色調の品質。 異なる画像レイヤーの40色の事前定義されたセットから最大3色を識別します。<p>**[!UICONTROL 描画色]** – 画像の前面レイヤーの色<br>**[!UICONTROL 背景色&#x200B;]**– 画像の背面レイヤーの色 | カラー値：`Red`, `Dark Red`, `Green`, `Bright Green`, `Dark Green`, `Light Green`, `Mud Green`, `Blue`, `Dark Blue`, `Light Blue`, `Royal Blue`, `Black`, `White`, `Off White`, `Gray`, `Dark Gray`, `Silver`, `Cream`, `Magenta`, `Cyan`, `Yellow`, `Khaki`, `Brown`, `Violet`, `Pink`, `Dark Pink`, `Maroon`, `Tan`, `Purple`, `Lavender`, `Turquoise`, `Plum`, `Gold`, `Emerald`, `Orange`, `Beige`, `Lilac`, `Olive``Mustard``Dark Brown` |
| 色温度 | 画像のカラーの一般的な暖かみまたは寒色度を表します。 | トーンまたは温度の値：`warm`、`cool`、`neutral`<br>![色および寒色系のトーン ](/help/assets/category/image-color-temp.png "寒色系の背景と複数の色付きのオブジェクトを含む色温度"){width="200" zoomable="yes"} |
| コンテンツ密度 | 画像内の視覚要素とディテールの濃度。視覚空間にどれだけの情報が詰め込まれているかを示します。<p>視聴者の焦点が画像のさまざまな領域にどのように広がっているかを測定するアテンション分布とは異なり、コンテンツ密度は、存在する視覚情報の量に焦点を当てます。 コンテンツ密度が高いほど、より多くの要素が存在することを意味します。 | `high`, `medium`, `low`<p>左側の`low`密度、右側の`high`密度の例：<p>![低密度と高密度のボールプレイ ](/help/assets/category/image-attn-lowhigh.png "低密度と高密度の差"){width="200" zoomable="yes"} |
| 画像スタイル | 写真やスケッチなど、画像の視覚的処理。 AIが画像のスタイルを決定すると、他の特性が特定される場合があります。 例えば、画像が写真の場合は、カメラ設定、カメラの近接、および照明条件が適用されます。 | `Photograph`, `Photograph with text overlay`, `Sketch`, `Painting`, `Digital cartoon`, `Infographics`, `Graphic design`, `Collage`, `Software screenshot`<p>`digital cartoon`画像スタイルの例![漫画の画像スタイル ](/help/assets/category/image-style.png "猫の画像スタイルの漫画"){width="200" zoomable="yes"} |
| 照明条件 | イメージ内の光の質と特性を記述し、そのムード、トーン、および可視性に影響を与えます。 | `Golden hour`, `Blue hour`, `Midday`, `Overcast`, `Night`, `Daylighting`, `Incandescent`, `Fluorescent`, `Colorful`, `Studio`<p>`daylighting`条件の例：<p>![日照条件で歩道を歩く人と犬](/help/assets/category/image-lighting.png "日照条件"){width="200" zoomable="yes"} |
| オブジェクト | 画像を構成する1つ以上の項目、エンティティ、および要素を識別します。 | 値が多すぎます。ただし、例として、`backpack`、`book`、`hawk`、`glasses`、`fish`、`pencil`、`mountain bike`、`soap`などがあります。<p>`toucan`および`bird` オブジェクトの例：<p>![鳥、ツアーズオブジェクト ](/help/assets/category/image-objects-bird.png " ツアーズオブジェクトのグラフィックデザイン "){width="200" zoomable="yes"} |
| オリエンテーション | 画像の幅と高さに対する画像の配置。 高さより広い（横）、幅より高い（縦）、幅と高さが等しい（正方形）かどうかを検出します。 | `landscape`, `portrait`, `square`<p>`square`方向の例：<p>![正方形のスケッチ ](/help/assets/category/image-orientation-square.png "正方形の方向の花のスケッチ "){width="200" zoomable="yes"} |
| ユーザー | 少なくとも1人が存在する場合、1つ以上の属性が画像内の人物または人物を表す場合があります。 | `person`, `woman`, `man`, `girl`, `boy`, `social group`, `kid`, `crowd`, `people`<p>ユーザー`woman`および`person`のカテゴリの例：<p>![ カメラを持つ人物](/help/assets/category/image-people.png " カメラを管理する人物"){width="200" zoomable="yes"} |
| 写真のジャンル | `Abstract`や`Landscape`などの画像のキャプチャに使用される被写体とテクニックを検出します（横方向とは異なります）。 | `Architecture`, `Astro`, `Landscape`, `Pet`, `Interior`, `Wildlife`, `Night`, `Cityscape`, `Seascape`, `Underwater`, `Storm`, `Adventure sports`, `Fashion`, `Portrait`, `Sports`, `Food`, `Street`, `Event`, `Lifestyle`, `Commercial`, `Group`, `Abstract`, `Minimalist`, `Composite`, `Surreal` <p>[写真の種類](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html)を参照してください。<p>例：`Adventure sports`<p>![ カヌーで立っている人](/help/assets/category/image-photography-genres.png " カヌーで立っているオールを持っている人"){width="200" zoomable="yes"} |
| シーン | 画像内の設定や環境を識別し、画像がキャプチャされた場所や表示された場所のタイプに関するコンテキストを提供します。 | 値が多すぎます。ただし、例として、`lake`、`underwater`、`highway`、`hill`、`log cabin`、`island`、`beach`、`lounge`などがあります。<p>例`snow`、`sky`、`winter`、`mountain`のシーンがヘルメットに反映されています。<p>![冬の雪のシーン ](/help/assets/category/image-scenes.png "冬、雪、空、山のシーンの反射"){width="200" zoomable="yes"} |
| 被写体の距離 | カメラと画像の被写体の間の距離。 | `close up`, `mid shot`, `long shot`<p>`Long shot`の例<p>![山頂をロングショット ](/help/assets/category/image-subject-distance.png "遠くの山頂の男性"){width="200" zoomable="yes"} |
| スタイル | LightroomやPhotoshopで使用される画像要素など、画像要素に適用される視覚処理を検出します。 | `design`, `illustration`, `logo`, `square`, `cartoon`, `art`, `circle`, `circular`<p>`circular` スタイルの例：<p>![ サンゴ礁の円形ゲートウェイ ](/help/assets/category/image-styles-circular.png " サンゴ礁の円形ポータル "){width="200" zoomable="yes"} |
| タグ | 特定の分類に該当しない他の画像特性を検出します。 タグは、画像に関する追加のコンテキストとメタデータを提供します。 例えば、AIは画像内の`helmet`および`motorobike` オブジェクトを検出し、`riding`をタグとして含めることができます。 | 値が多すぎます。ただし、例として、`construction`、`gothic`、`healing`、`military`、`selfie`、`football`、`typing`、`dancer`、`dancing`などがあります。<p>`dancer`および`dancing` タグの例：<p>![ ダンサーとダンスのタグ ](/help/assets/category/image-tags.png " ダンサー"){width="200" zoomable="yes"} |
