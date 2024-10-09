---
title: 属性の概要
description: Adobe GenStudio for Performance Marketingで特定の属性のパフォーマンスを評価する方法について説明します。
feature: Insights, Assets
source-git-commit: ce08231cb723bec3d80a732837b72a435d3b552d
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# 属性の概要

[!DNL Insights]_[!UICONTROL 属性]_ ビューには、選択したチャネルアカウントの広告キャンペーンで使用される属性のリストが表示されます。

_[!UICONTROL Attributes]_ テーブルは、[!UICONTROL Attribute] という名前を使用して整理されます。 「**[!UICONTROL 画像]**」ボタンと「**[!UICONTROL ビデオ]**」ボタンを使用して、リストタイプを切り替えることができます。 テーブルの右側の上にある設定（歯車）アイコンをクリックして、表示可能列を切り替えます。

テーブルの左側の上にあるフィルター（ファネル）アイコンをクリックすると、**[!UICONTROL フィルター]** メニューが開き、[!UICONTROL  アカウント ] および [!UICONTROL  属性カテゴリ ] から選択して、テーブルの属性をフィルタリングできます。 次の例は、`Lighting Condition` カテゴリの属性のリストを示しています。

![ 属性フィルターとテーブル ](/help/assets/insights-attributes-filter.png){zoomable="yes"}

## 属性の詳細

属性は、色、構成、視覚要素、その他のプロパティなど、固有の詳細によってアセットを識別するのに役立ちます。

属性の詳細表示では、選択した属性を使用しているエクスペリエンスを確認できます。 詳細には、属性パフォーマンスの合計と、各エクスペリエンスに関連するパフォーマンス指標の分類が含まれます。

![ 属性パフォーマンス指標 ](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketingは、特定の機能を検出し、適切な属性をアセットまたはエクスペリエンスにタグとして適用します。 これらのタグの例については、[ カテゴリ ](#categories) を参照してください。 エクスペリエンスに関連付けられているすべての属性を表示するには、テーブルの右側の上にある設定（歯車）アイコンをクリックして **[!UICONTROL 属性]** 列を選択します。

## カテゴリ

GenStudio for Performance Marketingでは、画像、ビデオおよびテキストの特定の機能を認識し、機能タグをアセットに適用します。 _カテゴリ_ は、特定の特性を共有する一連の機能です。 _image orientation_ の値の例は `landscape` です。

検出され、自動的に適用された属性は編集できません。

<!--
Select any of the following to open a detailed list of feature categories:

+++**Image features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Background Colors      | 14 colors |
| Camera Position        | - `low angle`, `high angle`, `dutch angle`<br>- `overhead view`, `eye level`,`bird's eye view` |
| Camera Proximity       | `close up`, `mid shot`, `long shot` |
| Camera Setting         | - `fast shutter speed`, `long exposure`, `double exposure`<br>- `normal mode`, `flash`, `macro`, `wide-angle`<br>- `black and white`, `surreal`<br>- `bokeh blur`, `motion blur`, `tilt-shift blur` |
| Foreground Colors      | 14 colors |
| Image Type             | `photograph`, `sketch`, `painting`, `digital cartoon`, `infographics`, `graphic design`, `collage`, `screenshot` |
| Lighting Condition     | golden hour, blue hour, midday, overcast, night, high-key, low-key, daylight, incandescent, fluorescent, colorful, studio |
| Objects                | The items, entities, and elements that are visible, such as `lighthouse`, `orchid`, or `tunnel`. |
| Orientation            | Examples: `landscape`, `portrait`, `square` |
| Overall Tone           | `warm`, `cool`, `neutral` |
| People Categories      | Examples: `person`, `social group`, `people`, `kid` |
| Photography Styles     | `aerial photography`, `aerial photography`, `architectural photography`, `astrophotography`, `black and white photography`, `business photography`, `cityscape photography`, `commercial photography`, `composite photography`, `creative photography`, `editorial photography`, `event photography`, `family photography`, `fashion photography`, `fine art photography`, `food photography`, `holiday photography`, `indoor photography`, `landscape photography`, `lifestyle photography`, `macro photography`, `minimalist photography`, `night photography`, `outdoor photography`, `pet photography`, `portrait photography`, `product photography`, `real estate photography`, `seascape photography`, `sports photography`, `still-life photography`, `street photography`, `travel photography`, `underwater photography`, `wildlife photography` |
| Scenes                 | Examples: `city`, `island`, `living room` |
| Tags                   | Examples: `gaming`, `law`, `yoga` |
| Visual Attention Spread| The level of viewer attention spread across an image: `high`, `low` |
| Visual Content Density | The amount of information or detail in an image: `high`, `low` |

+++

+++**Video features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Audio Genre  | |
| Audio Genre Category  | |
| Audio Mood  | |
| Audio Types| |
| Objects  | |
| Orientation  | |
| People Categories  | |
| Scenes  | |
| Styles  | |
| Tags   | |
| Video Category  | |
| Video Type  | |

+++

+++**Text features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Emojis Count  | |
| HashTags Count  | |
| Keywords  | |
| Marketing Emotions  | |
| Narratives  |  |
| Persuasion Strategies  |  |
| Readability  | |
| Sentences Count  | |
| Stop Words Ratio  | |
| Text Quotes Count  | |
| Tones  | |
| Words Count  | |
| Words Count Per Sentence  | |

+++

-->

## 属性指標

インサイト指標は、どの属性がより顧客エンゲージメントを高めるかを評価するのに役立ちます。

### 指標の詳細

次の表に、[!UICONTROL  属性 ] ビューでの主要なデジタルマーケティング指標の定義とインサイトを示します。 各指標には、アセットに関連する簡単な定義、指標の計算方法、広告キャンペーンに対する重要性と影響を理解するのに役立つ 1 つ以上のインサイトが含まれます。

| 指標 | 定義 | インサイト |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL 属性]** | 属性名。 | 任意の主要指標の列見出しをクリックして、テーブルを並べ替えます。 |
| **[!UICONTROL カテゴリ]** | 属性の固有の品質を表す [ カテゴリ ](#categories)。 |  |
| 画像の **[!UICONTROL 数]** | この属性を持つ画像の数。 |  |
| ビデオの **[!UICONTROL 数]** | この属性を持つビデオの数。 |  |
| **[!UICONTROL インプレッション]** | この属性を持つ画像またはビデオが、インタラクションや表示に関係なく、チャネルに読み込まれるたびに発生する回数。 | インプレッション数が多い場合は、幅広い可視性を示すことがありますが、真のパフォーマンスインサイトを得るには、他のエンゲージメント指標の使用を検討してください。 |
| **[!UICONTROL クリック数]** | ユーザーがこの属性を使用して画像またはビデオを操作した回数。 | クリック数が多い場合は、コンテンツに対する強い関心とエンゲージメントを示し、効果的で適切なオーディエンスに届く可能性があります。 |
| **[!UICONTROL CTR ]**<br>_クリックスルー率_ | この属性を持つ画像またはビデオのクリックにつながるインプレッション数の割合（%）。<br>**計算**:`clicks` を `impressions` で割ったもの | クリックスルー率が高い場合は、コンテンツの関連性が高く、メッセージの発信とデザインにオーディエンスに対する動機となり、オーディエンスの関心を効果的にターゲティングしていることを示します。 |
| **[!UICONTROL CPM ]**<br>_1 千あたりのコスト_ | この属性を持つ画像またはビデオの 1000 件ごとの広告インプレッションのコスト（$）。<br>**計算**：合計金額 `spent` リーチで割り、さらに 1,000 を掛けます | 特に、クリックスルー率が高い場合は、値を小さくすると、コスト効率の高い表示を示す可能性があります。 |
| **[!UICONTROL CPC ]**<br>_クリックあたりのコスト_ | この属性を持つ画像またはビデオの各クリックに関連する平均コスト （$）。<br>**計算**：合計金額 `spent` を `clicks` で割った値 | 平均コストが低いと、特にコンバージョンの増加と比較した場合、コスト効率の高い広告費用が発生する可能性があります。 |
| **[!UICONTROL 費用]** | 一定期間の属性に関連する予算からの支出額（$）。 | 短期間に支出額が多いと、急激な使用が示唆され、リソースの早期枯渇につながる可能性があります。 主要なパフォーマンス指標に対する支出額を追跡し、全体的な ROI を監視するのに役立ちます。 |
