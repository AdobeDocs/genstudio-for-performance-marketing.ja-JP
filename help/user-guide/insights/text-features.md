---
title: テキスト機能
description: GenStudio for Performance Marketingで使用される属性カテゴリのテキスト機能について説明します。
feature: Reporting and Insights, Text Attributes, Generative AI
exl-id: 7b81b0ae-0c62-468f-965c-fd8070644fb3
source-git-commit: 3ccc6313a7c559f1c0846c144d23b783da0aecfa
workflow-type: tm+mt
source-wordcount: '1290'
ht-degree: 1%

---

# テキスト機能

テキスト機能には、単語、文、絵文字などの特定のテキスト要素のカウントや、[!DNL Insights] での分析に使用されるセマンティクス、感情、トーンの分類が含まれます。 テキストは、読みやすさのスコアが得られる場合もあります。

GenStudio for Performance Marketingは、Adobeの AI と機械学習機能を使用して、テキストを調べ、関連するテキストのトーンとマーケティングの物語に基づいて [!UICONTROL &#x200B; メディア属性 &#x200B;] を適用します。 このプロセスでは、入力テキストが英数字を含んでいるか、余分な空白や印刷不可能な文字が削除されているか、テキストが許容される最大 1500 語に切り捨てられているかが検証されます。 検出された属性タグを適用する前に、AI が一般的なトーンを予測します。

## 声トーン

トーンは、言語を通じて示される一般的な性格、態度、または雰囲気を表します。 単語や句読点、文の構造、スタイルを簡単に選択して、メッセージのトーンを変更できます。 例えば、トーンの 3 つの基本的なレベルを使用して、次の緊急メッセージについて考えてみましょう。

| トーン | 説明 | 例 |
| -------------- | ----------------------------------- | --------------------------------------------------------- |
| 正式 | 洗練されたプロフェッショナルな言葉。 | `Take advantage of this distinctive and exceptional opportunity!` |
| 会話 | フレンドリーで非公式な言語。 | `Don't miss out on this great opportunity!` |
| ダイレクト | 単刀直入で要領を得ている。 | `Don't miss the chance!` |

トーンのその他の第 2 の値は、メッセージの性格と態度をより細かく区別します。 緊急メッセージの以前の例に合わせて、GenAI は、次の気まぐれな例では _詩的_ トーンを検出する可能性があります。`Embrace the moment, without delay, for this occasion won't always stay.`

次の表に、GenStudio for Performance Marketing AI で認識される色調値を示します。

| トーン | 説明 | 例 |
| -------------- | ------------------------------------------------ | --------------------------------------------------------- |
| 断定的 | 自信を持って力強い表現。 | `You need to act now to secure this deal!` |
| ダイレクト | 単刀直入で要領を得ている。 | `Don't miss the chance!` |
| 共感的な | 理解と感受性を示す。 | `We understand your needs, and this is perfect for you.` |
| 熱心な | 激しく熱心な楽しみ、興味、または承認を示す。 | `This is an amazing opportunity you can't miss!` |
| ユーモラス/ウィット | 心が軽くて賢い。 | `Why wait? Grab this deal before it's gone!` |
| 感動的 | 励まし、励ます。 | `Believe in yourself and seize this opportunity!` |
| 詩的 | 芸術的で表現力豊か。 | `Embrace the dawn of a new opportunity.` |
| 定量的 | 数値データによる。 | `99% of users loved this offer, and you will too.` |
| 感覚 | 感覚を引き付ける。 | `Feel the excitement with this incredible offer!` |
| ストーリーテリング | メッセージを伝えるためにストーリーをナレーションする。 | `Once upon a time, there was an offer you couldn't refuse.` |

## 情緒的魅力

マーケターは、人間の感情の力を活用して、オーディエンスとブランドの間に強いつながりを作り出します。 幸せ、恐怖、興奮、ノスタルジアなどの感覚を活用することで、マーケターはより深いレベルで共鳴するメッセージを作成し、エンゲージメントを促進し、消費者の行動に影響を与えることができます。 感情的な魅力は、より関連性が高く思い出に残るコンテンツを提供するのに役立ち、最終的にブランドロイヤルティを促進し、望ましい行動を促します。

説得の戦術、マーケティング上の感情、物語のスタイルが組み合わさって、顧客セグメントがターゲットになります。

- **物語のスタイル** 真正性、お祝い、コミュニティなど）は、ターゲットオーディエンスの共感を得られる価値とアイデンティティを伝え、より説得力があり、関連性の高いメッセージを作成するのに役立ちます。
- 希少性、社会的証拠、相反性などの **説得** 戦術は、消費者の感情や好みに訴えることで消費者の行動に影響を与えるように設計されています。
- **マーケティングの感情** は、ブランドとのエンゲージメントやコネクションを高める感情を刺激することを目的としています。

GenStudio for Performance MarketingAI は、テキストを分析して感情的な手掛かり、トーン、物語のスタイルを特定することにより、これらの特徴を検出して区別します。 AI は、自然言語処理（NLP）と機械学習アルゴリズムを使用して、パターンを識別し、事前定義された感情的および説得力のある属性に基づいてテキストを分類します。

### 物語のスタイル

ナレーション（アピール要因）属性は、ターゲットオーディエンスの共感を得られる値、目的または ID を伝えるメディアを識別するのに役立ちます。 次の表に、GenStudio for Performance Marketing AI で認識される物語スタイルを示します。

| アピール要因 | 説明 | 例 |
| ----------------- | --------------------------------------------------------------------- | ------------------------------------------ |
| 信頼性 | 本物で本物で、透明性と誠実さを強調しています。 | `A behind-the-scenes look at how our products are made.` |
| お祝い | 特別な機会や成果を喜びとお祭りでマークする。 | `Join us in celebrating our 10th anniversary with special offers!` |
| コミュニティ | グループ間の帰属意識と一体感を醸成する。 | `Our brand is built on the strength of our community.` |
| 利便性 | 使いやすさと時間節約のメリットを強調。 | `Get what you need with just one click.` |
| 権限の付与 | 個人がコントロールを取り、意思決定できるよう奨励し、それを可能にします。 | `Empower yourself with our latest tools and resources.` |
| 探索 | 新しいエクスペリエンスに関連する発見や冒険を招待します。 | `Discover new horizons with our travel packages.` |
| 未来の | イノベーションと前向きなアイデアに焦点を当てます。 | `Experience the future of technology today.` |
| 誇大広告 | 製品やイベントに関する興奮や期待を生み出す。 | `Don't miss out on the most anticipated event of the year!` |
| 甘い | 空想、欲望、または喜びに訴える。 | `Treat yourself to the finest gourmet chocolates.` |
| 安心の心 | 安心を与え、安心感を与える。 | `Rest easy knowing your data is safe with us.` |
| パーソナライズ機能 | 個々の環境設定に合わせてエクスペリエンスや製品を調整する。 | `Get a custom-fit solution just for you.` |
| 威信 | 高いステータスと排他性との関連付け。 | `Join the elite with our premium membership.` |
| 時間の無駄 | 永続的な品質と古典的な魅力を強調。 | `Our designs are timeless and never go out of style.` |
| 汎用性 | 適応性と多用途を強調表示する。 | `Our product fits seamlessly into any lifestyle.` |
| 幸福 | 健康、幸福、そして全体的な健康を促進する。 | `Enhance your well-being with our holistic approach.` |

### 説得の戦術

消費者の行動に影響を与え、望ましい行動を促すために、説得テクニックが使用されます。 具体的な心理トリガーや顧客セグメントをターゲットに、マーケティングメッセージの効果を高める施策です。 次の表に、GenStudio for Performance Marketing AI が認識する説得の手法を示します。

| 戦術 | 説明 | 例 |
| --------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| 擬人化 | 人間の特性の製品またはブランドへの帰属。 | `Our friendly chatbot is here to help you.` |
| 比較 | 選択に影響を与えるオプション間の違いを強調表示する。 | `See how we compare to the competition.` |
| 具体性 | メッセージをより具体的なものにするための具体的な詳細情報を提供する。 | `Save 20% on your next purchase.` |
| 推奨 | 信頼できる情報源や影響力者からの承認を特徴としています。 | `Recommended by top industry experts.` |
| ドアに足を踏み入れる | 小さなリクエストから始めて、大きなリクエストに同意する可能性を高めます。 | `Try our free trial today.` |
| リアクタンスの克服 | 反対意見を認め、反論に対処することで抵抗を減らす。 | `We understand your concerns, and here's how we address them.` |
| 相反性 | 再来訪を促す価値あるものを提供すること。 | `Get a free gift with your purchase.` |
| 欠乏 | 限られた可用性を強調することで、危機感を生み出します。 | `Only a few items left in stock!` |
| ソーシャル ID | グループに属しているという消費者の感覚を活用。 | `Join our community of innovators.` |
| 社会的影響 | 社会や環境に対するプラスの影響を重視する。 | `Your purchase helps plant a tree.` |
| ソーシャルの校正 | 証言やユーザー作成コンテンツを使用して信頼を構築する | `See why thousands of users love our product.` |

### マーケティング感情

感情は、オーディエンスから特定の感情や反応を呼び起こすためにマーケティングメッセージでターゲット設定され、ブランドへのエンゲージメントとつながりを高める可能性があります。 次の表に、GenStudio for Performance MarketingAI が認識する感情を示します。

| 情緒 | 説明 | 例 |
| ------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| 誤嚥 | より大きな何かを達成または達成したいという欲求を刺激する。 | `Imagine the possibilities with our premium service.` |
| 課題 | 障害を克服したり、新しいタスクを受け入れたりするように、オーディエンスを促します。 | `Are you ready to take the next step in your career?` |
| 好奇心 | 興味と詳細を学びたいという願望を引き起こします。 | `Discover the secrets behind our success.` |
| 排他性 | 選択グループの一部であるという感覚を生み出します。 | `Join our exclusive club for members-only benefits.` |
| 魅力的 | 魅力的またはエキサイティングなコンテンツでオーディエンスを魅了します。 | `Be amazed by our latest innovations.` |
| 満足 | 製品やサービスの利用による満足感と喜びを提供する。 | `Enjoy the ultimate comfort with our luxury bedding.` |
| 認識 | オーディエンスの成果やステータスを確認し、評価する。 | `Get the recognition you deserve with our award-winning service.` |
| 信頼 | ブランドの信頼性と信頼性を構築します。 | `Trust us to deliver quality and excellence every time.` |
| 緊急度 | 時間に依存する機会を強調して、迅速なアクションを促す。 | `Act now before this limited-time offer expires!` |

## 読みやすさのスコア

読みやすさのスコアリングは、テキストの読みやすさと理解しやすさを評価します。 これは、コンテンツがターゲットオーディエンスに適していることを確認するのに役立ちます。 スコアは、文の長さや単語の複雑さなど、様々な要因に基づいています。 次の表に、GenStudio for Performance Marketing AI で認識される読みやすさのレベルを示します。

| 読みやすさのレベル | 説明 | 例 |
| ------------------- | ------------------------------------------------------------------ | --------------------------------------------------------- |
| 5 年生 | 幼児に適した非常に単純な言語。 | `The cat sat on the mat.` |
| 6 年生 | 一般的な聴衆に適したシンプルで明確な言語。 | `You can find great deals on our website.` |
| 7 年生 | わかりやすい語彙と構造で、理解しやすい。 | `Our new product is simple to use and very effective.` |
| 8 年生と 9 年生 | ティーンエイジャーに適した明確で簡潔な言語。 | `This guide will help you understand the basics of our service.` |
| 10 年生から 12 年生 | より複雑な言語、年上のティーンエイジャーや大人に適しています。 | `The comprehensive manual provides detailed instructions for setup.` |
| 大学 | 高度な言語、よく教育を受けた聴衆に適しています。 | `The study explores the multifaceted implications of the new policy.` |
| 大卒 | 専門家や専門家に適した高度な言語。 | `The dissertation delves into the intricacies of quantum mechanics.` |

## カウント

ハッシュタグ数、単語数、文の数、ストップワードの比率などのカウント属性を理解し活用することで、コンテンツ戦略を大幅に強化できます。 これらの指標は、マーケティング活動の有効性とリーチに関する貴重なインサイトを提供します。 次の表に、GenStudio for Performance Marketing AI で認識されるカウントのカテゴリを示します。

| カテゴリ | 説明 | 例 |
| --------------------- | --------------------------------------------------------------------------- | --------------------- |
| 絵文字の数 | テキストに存在する絵文字の数です。 絵文字を使用すると、エンゲージメントを高め、感情を素早く伝えることができます。 | `😊`、`🚀`、`❤️` |
| HashTags Count | テキストで使用されるハッシュタグの数。 ハッシュタグは、コンテンツを分類し、ソーシャルメディアでの検出性を高めるのに役立ちます。 | `#Marketing`、`#Sale` |
| 文あたりの単語数 | テキスト内の文あたりの平均単語数。 多くの場合、短い文の方が読みやすく理解しやすいです。 | `10` |
| 単語数 | テキスト内の単語の合計数。 単語数が多いと、より詳細な情報が得られますが、読むためにより多くの労力が必要になる場合もあります。 | `1500 words` |
| ストップワードの比率 | テキスト内の意味のある単語に対するストップワードの比率。 ストップワード（「a」「an」「the」など）は、多くの場合、検索クエリや検索結果で無視されます。 ストップワードの割合が高いと、コンテンツのエンゲージメントが低下し、読みにくくなります。 | `0.375` |
| 文数 | テキスト内の文の合計数。 文が増えると、より詳細なコンテンツを示すことがありますが、過度に長いテキストは読者の興味を失う可能性があります。 | `75 sentences` |
