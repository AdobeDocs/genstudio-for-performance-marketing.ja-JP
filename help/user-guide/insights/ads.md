---
title: 広告と広告プレースメントの概要
description: Adobe GenStudio for Performance Marketingの広告および広告プレースメントのパフォーマンスに関する顧客エンゲージメント、予算および支出の概要を参照してください。
level: Intermediate
feature: Ad Performance, Text Attributes, Reporting and Insights
exl-id: e3827b1a-53d0-465c-8125-15b0e298ef3a
source-git-commit: 8a5d15df7a347c4ee7767610fc9bb23fc7b71db4
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 0%

---

# 広告と広告プレースメントの概要

[!DNL Insights] _[!UICONTROL 広告]_ ビューには、接続されたチャネル広告アカウントの広告のリストが表示されます。 _広告_ は、マーケティングキャンペーンの一部として特定のオーディエンスに配信することを目的とした、視覚的でインタラクティブなコンテンツを含むプロモーションアセットです。 Facebook の場合、広告はメタ広告名です。

{{connect-insights}}

_[!UICONTROL 広告]_ テーブルは、[!UICONTROL  広告名 ] を使用して整理されます。 テーブルの右側の上にある設定（歯車）アイコンをクリックして、表示可能列を切り替えます。 テーブルの左側の上にフィルター（ファネル）アイコンをクリックすると、**[!UICONTROL フィルター]** メニューが開き、複数のリストから選択できます。 すべてのフィルターを削除するには、テーブルの上にある「**[!UICONTROL すべてクリア]**」を選択します。

![ 広告フィルターとテーブル ](/help/assets/insights-ads-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## 広告の詳細

広告を選択し、各広告に関連付けられたパフォーマンス指標、テキスト属性、プレースメントを表示します。 _[!UICONTROL 広告の詳細ページ]_ には、広告の `click-through rate`、`cost per action`、`spend` の指標（広告に費やした予算の割合）が含まれます。 広告にはフィードやバナーなど、複数のプレースメントを含めることができるので、広告プレースメントごとに同じ指標の分類を表示できます。 **[!UICONTROL 広告プレースメントによるパフォーマンス]** の下の左右の矢印を使用して、プレースメント指標を順番に切り替えます。

![ 指標と広告プレースメントを含む広告の詳細 ](/help/assets/insights-ad-details.png){zoomable="yes"}

### テキスト属性

広告プレビューの下に、広告に関連付けられた [!UICONTROL  テキスト属性 ] のリストがあります。 アセットと広告が承認されて [!DNL Content] に保存されると、GenStudio for Performance Marketingは固有の機能に基づいてタグを生成します。 システムメタデータについて詳しくは、[ メディアの詳細 ](/help/user-guide/content/asset-details.md#system-metadata) を参照してください。

### 広告プレースメント

メタ広告を含むキャンペーンを作成した時点で、キャンペーン [ 目的 ](channels.md#objectives) に基づいて広告を実行する場所を選択している可能性があります。 広告プレースメントは、広告のオーディエンスのリーチを広げます。

GenStudio for Performance Marketingは、アセットフィード、リンク広告、1 つの画像やビデオなど、広告形式をサポートしています。 以下に、プラットフォーム別の広告形式のリストを示します。

| Instagram | Facebook/Meta | Messenger | オーディエンスネットワーク |
| ------------ | ---------------- | ------------ | ---------------- |
| 検索 <br> ホーム <br> 検索グリッドの検索 Home<br>Feed<br>Reels<br>Profile feed<br>Search<br>Shop<br>Stories | Business Explore<br>Feed<br>In-stream video<br>Marketplace<br>Reels<br>Reels overlay<br>Right column<br> 検索結果 <br> ストーリー <br> ビデオフィード <br>Facebook リールの広告 | Inbox<br>Stories | ネイティブ、バナー、インタースティシャル <br> リワードのビデオ |

#### サポートされていないプレースメント

GenStudio for Performance Marketingは、次の広告プレースメントをサポートしていません。

- 協調
- カタログ/Advantage+ カタログ
- インスタンスの経験
- カルーセル

## 広告パフォーマンス

インサイト指標は、キャンペーンの成功に貢献する広告と、最も効果的な広告プレースメントを評価するのに役立ちます。

次の表に、[!UICONTROL  広告 ] テーブルビューでの主要なデジタルマーケティング指標の定義とインサイトを示します。 各指標には、広告名に関する簡単な定義、指標の計算方法、広告の重要性と広告への影響を理解するのに役立つ 1 つ以上のインサイトが含まれます。

| 指標 | 定義 | インサイト |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL 広告名]** | 接続されたチャネルアカウントの広告のリスト。 キャンペーンを選択して広告をフィルタリングします。 | いずれかの主要指標をクリックして、広告リストを並べ替えます。 |
| **[!UICONTROL キャンペーン]** | キャンペーンは、特定の目的を達成するために設計された一連の広告です。 | 広告テーブルをキャンペーンでフィルターすると、キャンペーンのすべての広告の概要指標が、[!UICONTROL  チャネル ] ビューのキャンペーンの概要行とは異なる場合があります。 この不一致は、Meta などのチャネルソースとGenStudioで使用される要約計算が若干異なる場合に発生する可能性があります。 |
| **[!UICONTROL プレースメント]** | 広告 [ プレースメント ](#ad-placements) の数、キャンペーンで広告が表示された場所。 | プレースメントを使用すると、オーディエンスのリーチが向上します。<p>プレースメントとメディアがゼロの広告は、[ サポートされていない広告タイプ ](#unsupported-placements) を示している場合があります。</p> |
| **[!UICONTROL メディア]** | 広告または広告で使用されるアセットの数。 | 広告テーブルのカウントは、広告の詳細ビューのカウントとは異なる場合があります。 この不一致は、Meta などのチャネルソースとGenStudioで使用される要約計算が若干異なる場合に発生する可能性があります。 |
| **[!UICONTROL インプレッション]** | インタラクションや表示に関係なく、広告の配置または広告がチャネルに読み込まれるたびにカウントされます。 | インプレッション数が多い場合は、幅広い可視性を示すことがありますが、真のパフォーマンスインサイトを得るには、他のエンゲージメント指標と関連させて検討してください。 |
| **[!UICONTROL クリック数]** | 広告プレースメントで、ユーザーがリンクやコールトゥアクションボタンなどのクリック可能な要素を操作した回数。 | クリック数が多い場合は、コンテンツに対する強い関心とエンゲージメントを示し、効果的で適切なオーディエンスに届く可能性があります。 |
| **[!UICONTROL CTR ]**<br>_クリックスルー率_ | キャンペーン内の広告のクリックにつながったインプレッション数の割合（%）。<br>**計算**:`clicks` を `impressions` で割ったもの | クリックスルー率が高い場合は、コンテンツの関連性が高く、メッセージの発信とデザインにオーディエンスに対する動機となり、オーディエンスの関心を効果的にターゲティングしていることを示します。 |
| **[!UICONTROL CPM ]**<br>_1,000 人当たりのコスト_ | 広告インプレッション 1000 件ごとのコスト。<br>**計算**：合計金額 `spent` リーチで割り、さらに 1,000 を掛けます | 特に、クリックスルー率が高い場合は、値を小さくすると、コスト効率の高い表示を示す可能性があります。 |
| **[!UICONTROL アクションあたり ]**<br>_CPA コスト_ | 購入や購読など、特定の顧客アクションを達成するために費やした平均コスト。<br>**計算**：合計金額 `spent` 顧客処理の完了数で割った値 | 貴重な顧客アクションにつながる広告の支出を監視するために使用します。 |
| **[!UICONTROL CPC ]**<br>_クリックあたりのコスト_ | 広告プレースメント内の各クリックに関連する平均コスト。<br>**計算**：合計金額 `spent` を `clicks` で割った値 | 平均コストが低いと、特にコンバージョンの増加と比較した場合、コスト効率の高い広告費用が発生する可能性があります。 |
| **[!UICONTROL 費用]** | この広告を掲載するために特定の期間にキャンペーン予算から費やした金額。 | 短期間に支出額が多いと、急激な使用が示唆され、リソースの早期枯渇につながる可能性があります。 主要パフォーマンス指標に対する支出額を追跡し、全体的な ROI を監視するのに役立ちます。 |

## 配置パフォーマンス

_[!UICONTROL 広告の詳細ページ]_ ビューの上位 3 つの指標には、選択した広告の全体的なパフォーマンスが反映されます。 ただし、「プレースメント別のパフォーマンス _のセクションには、各広告プレースメントの詳細な指標が表示されます_。 左右の矢印を使用して、異なる広告プレースメント間を移動します。

次の表に、広告プレースメントのパフォーマンス指標の定義を示します。

| 指標 | 定義 | インサイト |
| ---------------------- | ----------------------------- | ----------- |
| **[!UICONTROL CTR ]**<br>_クリックスルー率_ | クリックにつながった単一の広告プレースメントのインプレッションの割合（%）。<p>**計算**:`clicks` を `impressions` で割った値<p>この指標は、オーディエンスを引き付ける際の広告の配置の有効性を判断するのに役立ちます。 | CTR が高い場合は、広告プレースメントがオーディエンスにとって関連性が高く、魅力的であり、より多くのインタラクションにつながることを示します。 |
| **[!UICONTROL アクションあたり ]**<br>_CPA コスト_ | 購入や購読など、目的の顧客アクションを達成するために 1 つの広告プレースメントに費やされる平均コスト。<p>**計算**：合計金額 `spent` 顧客処理の完了数で割った値<p>この指標は、価値のあるアクションを推進する際の広告プレースメントのコスト効率を評価するのに役立ちます。 | CPA が低いほど、低コストでオーディエンスのインタラクションを目的のアクションに変換する際に、広告の配置が効果的であることを示唆します。 |
| **[!UICONTROL CPC ]**<br>_クリックあたりのコスト_ | 1 つの広告プレースメントでの各クリックに関連する平均コスト。<p>**計算**：合計金額 `spent` を `clicks` で割った値<p>この指標は、クリックを生成する際の広告配置のコスト効率を評価するのに役立ちます。 | CPC が低いほど、広告プレースメントが低コストでクリックを生成していることを示し、投資回収率を最大限に高めるのに役立ちます。 |
| **[!UICONTROL 費用]** | 1 つの広告プレースメントに費やされた金額。広告全体に費やされた合計金額の一部を表します。 この指標は、各広告プレースメントの予算配分と支出効率を追跡するのに役立ちます。 | 費用を監視すると、様々なプレースメントをまたいでリソースが効果的に使用されていることを確認できます。 |
