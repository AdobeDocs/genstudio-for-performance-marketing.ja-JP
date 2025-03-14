---
title: テキスト機能
description: GenStudio for Performance Marketingで使用される属性カテゴリのテキスト機能について説明します。
feature: Insights, Attributes, Generative AI
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 7b81b0ae-0c62-468f-965c-fd8070644fb3
source-git-commit: 808ffdb7f55f7ff938e9346b8513fab46f86df7c
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 1%

---

# テキスト機能

テキスト機能には、単語、文、絵文字などの特定のテキスト要素のカウントや、[!DNL Insights] での分析に使用されるセマンティクス、感情、トーンの分類が含まれます。 テキストは、読みやすさのスコアが得られる場合もあります。

GenStudio for Performance Marketingは、Adobeの AI と機械学習機能を使用して、テキストを調べ、関連するテキストのトーンとマーケティングの物語に基づいて [!UICONTROL  メディア属性 ] を適用します。 このプロセスでは、入力テキストが英数字を含んでいるか、余分な空白や印刷不可能な文字が削除されているか、テキストが許容される最大 1500 語に切り捨てられているかが検証されます。 検出された属性タグを適用する前に、AI が一般的なトーンを予測します。

## 声トーン

トーンは、言語を通じて示される一般的な性格、態度、または雰囲気を表します。 単語や句読点、文の構造、スタイルを簡単に選択して、メッセージのトーンを変更できます。 例えば、トーンの 3 つの基本的なレベルを使用して、次の緊急メッセージについて考えてみましょう。

- `Formal`

  ```
  Take advantage of this distinctive and exceptional opportunity!
  ```

- `Conversational`

  ```
  Don't miss out on this great opportunity!
  ```

- `Direct`

  ```
  Don't miss the chance!
  ```

AI はさらに、より繊細なトーンを検出します。 前述の例と同じ緊急ステートメントを使用して、次のバージョンでは気まぐれな `poetic` トーンを使用しています。

- `Poetic`

  ```
  Embrace the moment, without delay, for this occasion won't always stay.
  ```

トーンのその他のセカンダリ値には、`Enthusiastic`、`Assertive`、`Humorous/Witty`、`Inspirational`、`Empathetic`、`Sensory`、`Storytelling`、`Poetic`、`Quantitative`、`Personal` などがあります

## 物語

ナレーション属性は、ターゲットオーディエンスの共感を得られる値、目的または ID を伝えるメディアを識別するのに役立ちます。

| 物語 | 説明 | 例 |
| ----------------- | ----------- | ------- |
| `Authenticity` |             |         |
| `Celebration` |             |         |
| `Community` |             |         |
| `Convenience` |             |         |
| `Empowerment` |             |         |
| `Exploration` |             |         |
| `Futuristic` |             |         |
| `Hype` |             |         |
| `Indulgence` |             |         |
| `Peace of mind` |             |         |
| `Personalization` |             |         |
| `Prestige` |             |         |
| `Timelessness` |             |         |
| `Versatility` |             |         |
| `Well-being` |             |         |

## 読みやすさのスコア

読みやすさのスコアリングは、テキストの読みやすさと理解しやすさを評価します。 これは、コンテンツがターゲットオーディエンスに適していることを確認するのに役立ちます。 スコアは、文の長さや単語の複雑さなど、様々な要因に基づいています。

| スコア | 学校レベル | メモ |
| ----------- | ------------------ | ------------------------------------------------------------------------- |
| 100.00-90.00 | 5 年生 | とても読みやすい。 普通の 11 歳の生徒に分かりやすい。 |
| 90.0～80.0 | 6 年生 | 読みやすい。 消費者向けの会話英語。 |
| 80.0～70.0 | 7 年生 | かなり読みやすい。 |
| 70.0～60.0 | 8 年生と 9 年生 | 明白な英語。 13 歳から 15 歳の生徒が簡単に理解できます。 |
| 60.0～50.0 | 10 年生から 12 年生 | かなり読みにくい。 |
| 50.0～30.0 | 大学 | 読みにくいです。 |
| 30.0～0.0 | 大卒 | とても読みにくいです。 大学卒業生が最もよく理解されています。 |

## 単語数

未定

次の表に、GenStudio for Performance Marketing AI で認識される画像の機能カテゴリを示します。

| カテゴリ | 説明 | 例 |
| -------------------- | ------------- | --------------------- |
| 絵文字の数 |             |        |
| HashTags Count |             |        |
| キーワード |             |        |
| マーケティングの感情 | 感情は、オーディエンスから特定の感情や反応を呼び起こすためにマーケティングメッセージでターゲット設定され、ブランドへのエンゲージメントとつながりを高める可能性があります。 | `Aspiration`、`Challenge`、`Curiosity`、`Exclusivity`、`Fascination`、`Gratification`、`Recognition`、`Trust`、`Urgency` |
| 説得力のある戦略 | 消費者の行動に影響を与え、望ましい行動を促すために使用される技術。 具体的な心理トリガーや顧客セグメントをターゲットに、マーケティングメッセージの効果を高める施策です。 | `Social identity`、`Social proof`、`Endorsement`、`Concreteness`、`Foot in the door`、`Overcoming reactance`、`Reciprocity`、`Comparison`、`Social impact`、`Scarcity`、`Anthropomorphism` |
| 声トーン | 単語選択、句読点、文構造、スタイルを通じて、マーケティングメッセージで伝えられる一般的な性格、態度、雰囲気。 | `Enthusiastic`, `Assertive`, `Humorous/Witty`, `Inspirational`, `Empathetic`, `Sensory`, `Storytelling`, `Poetic`, `Quantitative`, `Personal` |
