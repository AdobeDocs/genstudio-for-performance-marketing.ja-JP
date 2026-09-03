---
title: テキスト機能
description: GenStudio for Performance Marketingで使用される属性カテゴリのテキスト機能について説明します。
feature: Reporting and Insights, Text Attributes, Generative AI
exl-id: 7b81b0ae-0c62-468f-965c-fd8070644fb3
TQID: https://experienceleague.adobe.com/Oec5q249StCtuG-2-n1dYmJoEDRPaqLF2QANpwClQ3A
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: c95c94c1-727b-457a-9184-a4dda4c95ab2id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
subfeature_v2: id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: d095671a-1355-40aa-8b5f-06c33c68080bid: e0eb8757-182f-49f3-94a4-1587d16f5094id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eb30f47f-d87a-400f-8f78-63ce7979ff56id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3id: fc314d1d-7cb9-4a38-8dbd-8f9b6478f40d
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 1300
ht-degree: 1%

---

# テキスト機能

テキスト機能には、単語、文章、絵文字、セマンティクス、感情、トーンの分類など、[!DNL Insights]での分析に使用される特定のテキスト要素のカウントが含まれます。 テキストは読みやすさのスコアを受け取る場合もあります。

GenStudio for Performance Marketingは、AdobeのAIおよびマシンラーニング機能を使用してテキストを学習し、関連するテキストのトーンとマーケティングのストーリーに基づいて[!UICONTROL  メディア属性]を適用します。 このプロセスでは、入力テキストに英数字が含まれていることを確認し、余白と印刷不可能な文字を削除し、テキストを許可される最大1500語に切り捨てます。 検出された属性タグを適用する前に、AIは一般的なトーンを予測します。

## 声の調子

トーンは、言語を通じて示される一般的なキャラクター、態度、雰囲気を表します。 単語や句読点、文構造、スタイルをシンプルに選択するだけで、メッセージのトーンを変えることができます。 たとえば、次の緊急メッセージをトーンの3つの基本レベルで考えてみましょう。

| トーン | 説明 | 例 |
| -------------- | ----------------------------------- | --------------------------------------------------------- |
| フォーマル | 洗練されたプロフェッショナルな言語。 | `Take advantage of this distinctive and exceptional opportunity!` |
| 対話型 | フレンドリーでカジュアルな言語。 | `Don't miss out on this great opportunity!` |
| 直接 | わかりやすく、要点を伝えます。 | `Don't miss the chance!` |

トーンに関するその他の副次的な値は、メッセージのキャラクターと態度をより細かく区別します。 前述の緊急メッセージの例に従い、生成AIは、この気まぐれな例で&#x200B;_詩的な_ トーンを検出する場合があります。`Embrace the moment, without delay, for this occasion won't always stay.`

次の表に、GenStudio for Performance Marketing AIで認識される階調値を示します。

| トーン | 説明 | 例 |
| -------------- | ------------------------------------------------ | --------------------------------------------------------- |
| アサーティブ | 表現に自信と力強さを持つ。 | `You need to act now to secure this deal!` |
| 直接 | わかりやすく、要点を伝えます。 | `Don't miss the chance!` |
| 共感的 | 理解と感性を示す。 | `We understand your needs, and this is perfect for you.` |
| 熱心な | 強く熱心な喜び、興味、承認を示している | `This is an amazing opportunity you can't miss!` |
| ユーモラス/ウィッティ | 明敏で賢い | `Why wait? Grab this deal before it's gone!` |
| インスピレーション | 励ましと高揚。 | `Believe in yourself and seize this opportunity!` |
| 詩的 | 芸術的で表現力豊か。 | `Embrace the dawn of a new opportunity.` |
| 定量 | ビューを作成することができます。 | `99% of users loved this offer, and you will too.` |
| 感覚 | 五感を引き付ける。 | `Feel the excitement with this incredible offer!` |
| Storytelling | メッセージを伝えるストーリーのナレーション。 | `Once upon a time, there was an offer you couldn't refuse.` |

## 感情的なアピール

マーケターは、人間の感情の力を活用して、オーディエンスとブランドとの間に強力なつながりを築きます。 幸福、恐れ、興奮、ノスタルジーなどの感覚を利用することで、マーケターはより深いレベルで共感を呼ぶメッセージを作成し、エンゲージメントを促進し、消費者の行動に影響を与えることができます。 感情的なアピールは、より親近感のある記憶に残るコンテンツを配信し、最終的にブランドロイヤルティを育み、望ましい行動を促すのに役立ちます。

説得の戦術、マーケティングの感情、ストーリーのスタイルは、連携して顧客セグメントをターゲットにします。

- 真正性、祝祭、コミュニティなどの&#x200B;**ナラティブ スタイル**&#x200B;は、ターゲット オーディエンスに響く価値観とアイデンティティを伝え、より魅力的で関連性の高いメッセージを作成するのに役立ちます。
- 希少性、社会的証明、相互主義などの&#x200B;**説得の戦術**&#x200B;は、消費者の感情や好みに訴えかけることで、消費者の行動に影響を与えるように設計されています。
- **マーケティング感情**&#x200B;は、ブランドとのエンゲージメントと関連性を高める感情を刺激することを目的としています。

GenStudio for Performance Marketing AIは、テキストを分析して、感情的な合図、トーン、ナラティブスタイルを検出し、これらの特性を区別します。 AIは自然言語処理（NLP）とマシンラーニング（機械学習）のアルゴリズムを利用してパターンを特定し、事前に定義された感情的かつ説得力のある属性にもとづいてテキストを分類します。

### 物語のスタイル

物語や訴求要因は、ターゲットオーディエンスの心に響く価値、目的、アイデンティティを伝えるメディアを特定するのに役立ちます。 次の表に、GenStudio for Performance Marketing AIで認識されるナラティブスタイルを示します。

| 訴求力 | 説明 | 例 |
| ----------------- | --------------------------------------------------------------------- | ------------------------------------------ |
| 真正性 | 透明性と誠実さを重視した、誠実かつ真のサービスを提供。 | `A behind-the-scenes look at how our products are made.` |
| お祝い | 喜びや祝祭で特別な機会や成果をマークする。 | `Join us in celebrating our 10th anniversary with special offers!` |
| コミュニティ | グループ間の帰属意識と一体感の醸成。 | `Our brand is built on the strength of our community.` |
| 利便性 | 使いやすさと時間の節約というメリットを重視。 | `Get what you need with just one click.` |
| 能力開発 | 個人が主導権を握り、意思決定をするように奨励し、能力を高める。 | `Empower yourself with our latest tools and resources.` |
| 探索 | 発見と冒険を促し、新しい体験を促す。 | `Discover new horizons with our travel packages.` |
| 未来的 | イノベーションと先進的なアイデアの強調： | `Experience the future of technology today.` |
| 宣伝 | 製品やイベントに関する興奮や期待の生成。 | `Don't miss out on the most anticipated event of the year!` |
| 補償 | 空想、欲望、または喜びに訴える。 | `Treat yourself to the finest gourmet chocolates.` |
| 安心感 | 安心感と安心感を提供する。 | `Rest easy knowing your data is safe with us.` |
| パーソナライズ機能 | 個々の顧客の好みに合わせた体験や製品の提供。 | `Get a custom-fit solution just for you.` |
| Prestige | 高い地位と限定性を伴う。 | `Join the elite with our premium membership.` |
| タイムレス | 永続的な品質と古典的な魅力を強調。 | `Our designs are timeless and never go out of style.` |
| 汎用性 | 適応性と複数の用途の強調： | `Our product fits seamlessly into any lifestyle.` |
| ウェルビーイング | 健康、幸福、そして全体的な健康を促進する。 | `Enhance your well-being with our holistic approach.` |

### 説得戦術

説得テクニックは、消費者の行動に影響を与え、望ましい行動を促すために使用されます。 この戦略は、マーケティングメッセージの効果を高めるために、特定の心理的トリガーと顧客セグメントをターゲットにします。 次の表に、GenStudio for Performance Marketing AIが認識する説得の戦術を示します。

| 戦術 | 説明 | 例 |
| --------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| 擬人化 | 人間の特徴を製品やブランドに帰する。 | `Our friendly chatbot is here to help you.` |
| 比較 | 選択肢に影響を与えるためには、オプションの違いを強調する必要があります。 | `See how we compare to the competition.` |
| 具体性 | メッセージをより具体的にするための詳細を提供する。 | `Save 20% on your next purchase.` |
| 支持 | 信頼できるソースやインフルエンサーからの承認を利用します。 | `Recommended by top industry experts.` |
| ドアの中の足 | 小さなリクエストから始めて、大きなリクエストに合意する可能性を高める。 | `Try our free trial today.` |
| リアクタンスの克服 | 反対意見を認め対処することで抵抗を減らす。 | `We understand your concerns, and here's how we address them.` |
| 相互性 | 何か価値あるものを提供することで、お客様にリターンをお届けします。 | `Get a free gift with your purchase.` |
| Scarcity | 限られた在庫を強調し、切迫感を高める。 | `Only a few items left in stock!` |
| ソーシャルアイデンティティ | 消費者のグループ帰属意識を活用。 | `Join our community of innovators.` |
| 社会的影響 | 社会や環境へのプラスの影響を強調する。 | `Your purchase helps plant a tree.` |
| ソーシャルプルーフ | 顧客の声やユーザー生成コンテンツを使用して、信頼を構築する。 | `See why thousands of users love our product.` |

### マーケティング感情

マーケティングメッセージでは、オーディエンスの具体的な感情や反応を刺激し、エンゲージメントとブランドとのつながりを強化するのに役立ちます。 次の表に、GenStudio for Performance Marketing AIで認識される感情を示します。

| 感情 | 説明 | 例 |
| ------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| 願望 | より大きなものを達成したり、達成したりしたいという願望を刺激します。 | `Imagine the possibilities with our premium service.` |
| 課題 | 障害を克服したり、新しいタスクを受け入れたりするようにオーディエンスを促す。 | `Are you ready to take the next step in your career?` |
| 好奇心 | 興味を喚起し、もっと学びたいと思っています。 | `Discover the secrets behind our success.` |
| 排他性 | 選択されたグループの一員という意識を育む。 | `Join our exclusive club for members-only benefits.` |
| 魅了 | 魅力的なコンテンツでオーディエンスを魅了。 | `Be amazed by our latest innovations.` |
| 満足度 | 製品やサービスの利用に対する満足度や喜びを提供する。 | `Enjoy the ultimate comfort with our luxury bedding.` |
| 認識 | オーディエンスの成果や状況を把握し、評価する。 | `Get the recognition you deserve with our award-winning service.` |
| 信頼 | ブランドに対する信頼と信頼性を高める。 | `Trust us to deliver quality and excellence every time.` |
| 緊急性 | 時間的制約のある機会を強調し、即座に行動を促す。 | `Act now before this limited-time offer expires!` |

## 読みやすさスコアリング

読みやすさスコアリングは、テキストがどの程度簡単に読んで理解できるかを評価します。 コンテンツをターゲットオーディエンスに適したものにすることができます。 スコアは、文章の長さや単語の複雑さなど、さまざまな要因にもとづいて算出されます。 次の表に、GenStudio for Performance Marketing AIで認識される読みやすさのレベルを示します。

| 読みやすさレベル | 説明 | 例 |
| ------------------- | ------------------------------------------------------------------ | --------------------------------------------------------- |
| 5年生 | 非常に簡単な言語、幼児に適しています。 | `The cat sat on the mat.` |
| 6年生 | 一般的なオーディエンスに適した、シンプルで明確な言語。 | `You can find great deals on our website.` |
| 7年生 | わかりやすい単語と構造。 | `Our new product is simple to use and very effective.` |
| 8年生と9年生 | 10代の若者に適した、明確で簡潔な言語。 | `This guide will help you understand the basics of our service.` |
| 10～12年生 | より複雑な言語、年上のティーンエイジャーや大人に適しています。 | `The comprehensive manual provides detailed instructions for setup.` |
| College | 高度な言語、十分な教育を受けた視聴者に適しています。 | `The study explores the multifaceted implications of the new policy.` |
| 大学卒業生 | 専門家や専門家に適した高度な言語。 | `The dissertation delves into the intricacies of quantum mechanics.` |

## カウント

ハッシュタグ数、単語数、文数、単語数などのカウント属性を把握し、活用することで、コンテンツ戦略を大幅に強化することができます。 これらの指標は、マーケティング施策の効果とリーチに関する貴重なインサイトを提供します。 次の表に、GenStudio for Performance Marketing AIで認識されるカウントカテゴリを示します。

| カテゴリ | 説明 | 例 |
| --------------------- | --------------------------------------------------------------------------- | --------------------- |
| 絵文字カウント | テキスト内に存在する絵文字の数。 絵文字は、エンゲージメントを高め、感情を迅速に伝えることができます。 | `😊`, `🚀`, `❤️` |
| HashTags数 | テキストで使用されるハッシュタグの数。 ハッシュタグは、コンテンツを分類し、ソーシャルメディアでの見つけやすさを向上させるのに役立ちます。 | `#Marketing`, `#Sale` |
| 文章あたりの単語数 | テキスト内の1文あたりの平均単語数。 短い文章の方が読みやすく、理解しやすいことがよくあります。 | `10` |
| 文字数 | テキスト内の単語の合計数。 単語数を多くすると、より詳細な情報を提供できますが、読み上げるのにより多くの労力が必要になる場合もあります。 | `1500 words` |
| ストップワード比率 | テキスト内の意味のある単語に対するストップワードの比率。 ストップワード（「a」、「an」、「the」など）は、検索クエリや結果で無視されることがよくあります。 ストップワードの割合が高いと、コンテンツの魅力が低下し、読みづらくなる可能性があります。 | `0.375` |
| 文章カウント | テキスト内の文章の合計数。 文章が多いほど詳細なコンテンツを示すことができますが、長すぎるテキストは読者の興味を失う可能性があります。 | `75 sentences` |
