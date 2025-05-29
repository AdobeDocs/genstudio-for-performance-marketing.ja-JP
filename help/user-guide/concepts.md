---
title: Adobe GenStudio for Performance Marketing概念
description: Adobe GenStudio for Performance Marketingの概念と用語について説明します。
feature: Generative AI
role: User
exl-id: 7dd00b4c-f429-499b-851d-3606c82c09dc
source-git-commit: 1ff6a3ecf0a0773c3a6f13d6993042b0620c6dd2
workflow-type: tm+mt
source-wordcount: '699'
ht-degree: 0%

---

# 概念

GenStudio for Performance Marketingは、Adobeのコンテンツサプライチェーンを具体化してマーケティングキャンペーンを合理化するスタンドアロンのエンタープライズ製品です。 パーソナライズされ、ブランドで承認されたコンテンツを大規模に構築し、有効性を監視し、常に変化する市場に迅速に適応することは困難です。 GenStudio for Performance Marketingでは、ジェネレーティブ AI をエンタープライズマーケティングチームのパフォーマンスの乗数として活用する、1 つのアプリケーションでCreative CloudとExperience Cloudを統合します。

GenStudio for Performance Marketingを使用すると、次のことができます。

* 有料メディア、メール、ディスプレイ広告など、最優先のデジタルチャネルに対して自然言語プロンプトを使用して、オンブランドコンテンツを作成します

* 関係者との共同作業による、生成されたコンテンツのレビューと承認
* 生成および承認されたコンテンツを保存して、今後のマーケティングキャンペーン用にアクセスできる
* アセットのパフォーマンスを分析し、最もパフォーマンスの高いコンテンツの主な属性を特定することで、コンテンツの有効性を評価する

## ジェネレーティブ AI テクノロジー

GenStudio for Performance Marketingは、生成 AI の力を活用して、コンテンツ作成プロセスを加速し、高品質なコンテンツ生成を確実に行います。 クリエイティブアセットの反復的なライフサイクルにより、ターゲットオーディエンスの共感を得られる、より正確でブランドに合わせたコンテンツが得られます。

強力なブランドガイドライン機能を通じて、組織のブランディング、顧客のペルソナ、製品の説明を取り込むことから始めます。 これらのガイドラインの準備とアップロード方法については、[ ガイドラインの概要 ](../user-guide/guidelines/overview.md) を参照してください。

{{in-academy}}

### 大規模な言語モデル

GenStudio for Performance Marketingは、Adobeのジェネレーティブ AI プラットフォームを活用しています。このプラットフォームは、基盤となる AI および機械学習（ML）サービスを提供します。 このプラットフォームは、大規模な言語モデル（LLM）の使用を簡素化し、Adobeの GenAI 機能が魅力的なエクスペリエンスを作成できるようにします。

GenStudio for Performance Marketingでは、Azure OpenAI.<!-- Claude, and Gemini models. --> を通じて GPT シリーズのサードパーティ LLM を使用します。

## [!DNL Generative Actions]

_[!DNL Generative Actions]_&#x200B;は、[Adobe GenStudio for Performance Marketingの製品説明 ](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html) で定義されているように、GenStudio for Performance Marketing内での生成 AI 機能の使用を定量化するユニットです。

<!-- Add example about usage mode?
Where users check how many generative actions they have left
How they re-up their genactions
If genactions roll over month to month or not -->

### 料率

[GenStudio for Performance Marketingの製品説明 ](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html) に記載されている通り、[!DNL Generative Actions] のデフォルトの割り当てが受け取ります。

>[!NOTE]
>
>使用率は場合によって異なります。 計画は変更される場合があります。 更新後の評価について詳しくは、[Adobe GenStudio for Performance Marketingの製品説明 ](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html) を参照してください。

次の関数は、指定された割合で [!DNL Generative Actions] を使用します。

| 関数 | 生成アクション率 |
| -----------------------  | ------------------ |
| メールを作成 | 世代ごとに 5 個 |
| 有料メディア広告の作成 | 世代ごとに 5 個 |
| ディスプレイ広告の作成 | 世代ごとに 5 個 |
| セクションを再生成 | 世代ごとに 1 つ |

<!-- | Generate on-brand images | 1 per prompt  |
| Translation              | 1 per prompt  |
| Video: ADLS              | 1 per prompt  |
| Video: TTS + Avatar      | 1 per prompt  | -->

次の場合に [!DNL Generative Actions] _は使用されません_。

* バリアント生成時の [ ブランド検証 ](/help/user-guide/guidelines/brand-validation.md) の使用
* [ アップロードされたガイドライン ](/help/user-guide/guidelines/add-guidelines.md) からの情報の抽出
* 手動 [ バリアントの再チェック ](/help/user-guide/guidelines/brand-validation.md#improve-brand-alignment)
* デジタルアセットには、属性（[[!DNL Insights]](/help/user-guide/insights/overview.md)）が自動的にタグ付けされます

>[!TIP]
>
>[!DNL Generative Actions] の使用権限を超える場合は、アカウント担当者からさらに直接購入できます。

## データガバナンス

AI を使用してコンテンツを生成する場合、出力が安全で、すべてのユーザーにとって包括的であることを確認することが不可欠です。 これには、有害な偏見、ヘイトスピーチ、攻撃的な内容、不敬の可能性があるコンテンツの評価が必要です。 Adobeでは、コンテンツの創出技術を多角的に検証し、倫理の総合的な見直しを行い、有害コンテンツの発生抑制に向けた効果的な緩和策を実施しています。

このアプローチは、社会的責任を強化し、評判リスクを最小限に抑え、[Adobeの信頼と安全および倫理ポリシー ](https://www.adobe.com/content/dam/cc/en/ai-ethics/pdfs/Adobe-AI-Ethics-Principles.pdf) を確実に遵守します。

GenStudio for Performance Marketingには、Adobeのデータガバナンスの標準とポリシーに従って、有害または偏って特定されたコンテンツが使用されるのを防ぐための緩和計画が組み込まれています。 このようなコンテンツが検出されると、「生成できません」というメッセージが表示されてアセットの生成がブロックされることに注意する必要があります。

このメッセージが表示されたら、プロンプトを編集して再試行します _または_ プロンプトの内容にGenStudio for Performance Marketingによるレビューのフラグを立てます。 レビュー用にフラグが設定されたコンテンツのプロンプトデータは、内部レビュー目的で収集されます。

## コンテンツのライフサイクル

複数のチャネルで、より速いペースで質の高いエクスペリエンスが求められています。 GenStudio for Performance Marketingを使用すると、コンテンツサプライチェーンを簡略化して、マーケター向けのわかりやすいワークフローを構築できます。 GenStudio for Performance Marketingでは、ライフサイクルの各段階でAdobe テクノロジーを活用します。

<table style="table-layout:auto">

<tr style="border: 0;">

    <td>

       <p><strong>ワークフローと計画</strong></p>

    </td>

    <td>

        <p>アイデアのブレインストーミング、ガイドラインの定義、コンテンツに関する戦略の構築を行い、オーディエンスを引き付けます。</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>作成と実稼動</strong></p>

    </td>

    <td>

        <p>計画に基づいてコンテンツを生成します。 リアルタイムでの共同作業、フィードバックの受信、編集、コンテンツの承認を行います。</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>コンテンツ管理</strong></p>

    </td>

    <td>

        <p>クリエイティブアセットの保存、共有、検索を、一元化されたリポジトリで行います。 パフォーマンスに基づいたコンテンツの再利用と再活性化。</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>配信とアクティブ化</strong></p>

    </td>

    <td>

        <p>複数のマーケティングチャネルにわたってコンテンツと公開をアクティブ化します。</P>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>レポートとインサイト</strong></p>

    </td>

    <td>

        <p>アセットパフォーマンスの最適化のために、データを収集しインサイトを導き出します。</p>

    </td>

</tr>

</table>
