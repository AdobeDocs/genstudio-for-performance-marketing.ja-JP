---
title: ステートフル生成によるコンテンツの生成と調整
description: '[!DNL GenStudio for Performance Marketing]のボイスプリントとビジュアルキューを使用して、ブランドに即したコンテンツを生成し、順番に調整する方法を説明します。'
feature: Create Prompt, Generative AI, Content Generation
role: User
level: Beginner
source-git-commit: 22db02c07a9f33cb1c70df9286ad6eb143dafd38
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%
---
# ステートフル生成によるコンテンツの生成と調整

[!DNL GenStudio for Performance Marketing]はStateful Generationを使用して、ブランドに即したコンテンツを作成し、毎回新しいプロンプトで始めるのではなく、会話を順番に作成して改善します。 調整を行うと、以前の指示と保持しているバリエーションが生成に記憶され、要求した変更のみが適用されます。

Stateful Generationは、生成に3種類のコンテキストを追加します。ボイスプリントは、ブランドボイスにコピーを保持し、画像またはビデオにグラウンドコピーを視覚的に表示します。web ページのURLは、選択したページから参照コンテキストを追加します。

## コンテンツの生成と調整

1. [!DNL GenStudio for Performance Marketing]で、チャネルと形式の生成を開始します。 各チャネルの生成を開始するには、[[!DNL Create] 概要](/help/user-guide/create/overview.md)を参照してください。
1. _オプション_：独自のクリエイティブでコピーをグラウンド化するには、**[!UICONTROL コンテンツから選択]**&#x200B;を選択し、次に[視覚的なキュー](#ground-content-in-an-image-or-video)として使用する画像またはビデオを選択します。
1. 「**[!UICONTROL 生成]**」を選択します。 [!DNL GenStudio for Performance Marketing]はバリエーションのセットを作成し、サポートされているチャネルに[ ブランドボイス ](#keep-copy-in-your-brand-voice)を自動的に適用します。
1. プロンプトドロワーで結果を調整します。 必要な変更（`shorten the headline`、`make variant 2 punchier`、または`change the headline`など）を入力します。 生成は、その変更のみを適用し、以前の指示を保持します。
1. 調整を続ける間にバリエーションを保持するには、プロンプト ドロワーに`keep variant 2`などの指示を入力します。
1. コンテンツの準備ができたら、書き出すか、レビュー用に送信します。

## 画像またはビデオ内のコンテンツのグラウンド

ビジュアルキューを利用することで、添付した画像や動画を世代が読み取り、そのクリエイティブを反映したコピーを作成できます。 **[!UICONTROL Creative オプション]**&#x200B;の切り替えスイッチは、視覚的なキューを制御し、デフォルトではオンになっています。

ビジュアルキューを使用するには、**[!UICONTROL コンテンツから選択]**&#x200B;を選択し、生成する前に画像またはビデオを選択します。 視覚的なキューを使用せずに生成するには、**[!UICONTROL Creative オプション]**&#x200B;をオフにします。

>[!NOTE]
>ビジュアルキューは、マルチフレームディスプレイ広告やカルーセル広告では使用できません。

## ブランドボイスにコピーを反映

ボイスプリントは、ブランドで学んだ音声を生成されたコピーに適用し、余分なプロンプトを入力することなくブランドに即した音声を生成します。 LinkedInやMetaなど、[ インサイト ](/help/user-guide/insights/overview.md)を持つチャネルでは、デフォルトでオンになっています。

## Web ページをコンテキストとして使用

生成をweb ページに向け、そのコンテンツをコンテキストとして使用できます。 プロンプト ドロワーで、`Use this URL to generate an ad for this channel: https://www.example.com`などのURLを含む命令を入力します。

>[!NOTE]
>プロンプトにURLを入力します。 _パラメーター_&#x200B;を通じて追加しないでください。

## 関連する機能

- [ バリエーションの管理](/help/user-guide/create/manage-variants.md)：生成されたバリエーションをキャンバス上で直接編集および調整します。
- [効果的なプロンプトを作成](/help/user-guide/effective-prompts.md)：より効果的な結果を生み出すプロンプトを作成します。
