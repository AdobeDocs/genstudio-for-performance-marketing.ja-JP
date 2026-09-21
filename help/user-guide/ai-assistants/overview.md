---
title: AI アシスタント
description: AI アシスタントを[!DNL GenStudio for Performance Marketing]に接続して、インサイトを取得し、ドラフトを作成し、承認済みの広告を公開する方法について説明します。
role: User
source-git-commit: 6fb7ddb7549ea6bcd66b6139fbde9ebe12ddaa22
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 1%
---

# AI アシスタントの概要

[!DNL GenStudio for Performance Marketing]は、モデル コンテキスト プロトコル （MCP）を通じて、サポートされているAI アシスタントに接続します。 接続されると、自然言語の会話を通じて、広告のパフォーマンスを照会し、クリエイティブを組み立て、承認された広告を公開することができます。

## サポートされているAI アシスタント

サポートされているAI アシスタントのパスを通じて接続できます。

| AI アシスタント | 接続パス |
|---|---|
| Adobe CX Enterprise Coworker | 組織で管理されているネイティブ接続 |
| クロード | リモート MCP コネクタ |
| ChatGPT web版 | 開発者モードのリモート MCP コネクタ |
| Codex | コマンドラインから設定されたリモート MCP接続 |
| 執筆者 | リモート MCP カスタムコネクタ |
| Microsoft Copilot | Microsoft ガイダンスで設定されたリモート MCP接続 |

設定ガイダンスについては、[AI アシスタントへの接続](connect-ai-assistants.md)を参照してください。

## 機能

AI アシスタントにつながれば、次の3つの業務に取り組むことができます。

- **インサイト：**&#x200B;見出しのKPIを取得し、最もパフォーマンスの高い広告と最もパフォーマンスの低い広告を見つけ出し、広告が特定の方法でパフォーマンスを示す理由を理解し、パフォーマンスデータにもとづいたレコメンデーションを受け取ります。
- **作成：** テンプレートを参照し、テンプレートまたはレコメンデーションから編集可能なドラフトを作成し、レビューと承認のためにドラフトを共有します。
- **アクティブ化：**&#x200B;承認済みのエクスペリエンスを検索し、その公開ターゲットを解決して、接続されたチャネルに公開します。

サポートされるチャネルは機能によって異なります。 Insightsでは、ほとんどのレポートでMeta、LinkedIn、Innovidをカバーしています。 カスタムのコンバージョン指標では、MetaとLinkedInをカバーしています。

Meta、LinkedIn、Display、TikTok、YouTubeのカバーを作成できます。 Meta、LinkedIn、Google Campaign Manager 360のカバーをアクティベートします。 各ツールのチャネルサポートについては、[AI アシスタントツールのリファレンス ](tools-reference.md)を参照してください。

## アクセスと権限

AI アシスタント機能は、一般に、[!DNL GenStudio for Performance Marketing]に対して有効になっている顧客が利用できます。 商品にアクセスできるアクティブなAdobe アカウントが必要です。

接続はAdobe IDを使用し、既存の製品権限を尊重します。 アカウントが既に表示できる組織、有料メディアアカウント、キャンペーン、データのみにアクセスできます。

各接続は、1つのAdobe Identity Management System （IMS）組織に対してスコープが設定されます。 切り替える必要がある場合は、別の組織を再接続して選択します。

## 関連する機能

- **[AI アシスタントを接続](connect-ai-assistants.md)**：サポートされているAI アシスタントをアカウントに接続します。
- **[AI アシスタントを使用](use-ai-assistants.md)**：有料メディアの分析とレコメンデーションのプロンプト例を確認します。
- **[AI アシスタント ツール リファレンス](tools-reference.md)**：使用可能なインサイト、作成、アクティブ化、およびフィードバック ツールを確認します。
