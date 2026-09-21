---
title: AI アシスタントに接続する
description: サポートされているAI アシスタントを[!DNL GenStudio for Performance Marketing]に接続し、使用可能なツールへのアクセスを確認する方法を説明します。
role: User
source-git-commit: 6fb7ddb7549ea6bcd66b6139fbde9ebe12ddaa22
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%
---

# AI アシスタントに接続する

パフォーマンスデータのクエリ、ドラフトの作成、承認済み広告の公開を行う前に、サポートされているAI アシスタントを[!DNL GenStudio for Performance Marketing]に接続します。 接続オプションは、AI アシスタントと組織によって異なります。

## 前提条件

接続する前に、以下があることを確認します。

- [!DNL GenStudio for Performance Marketing]へのアクセス権を持つアクティブなAdobe アカウント。
- Claude、ChatGPT、またはMicrosoft Copilotを使用する場合にリモート MCP接続を可能にするサポートされているプラン。 MCP接続を手動で設定する方法については、AI アシスタントのドキュメントを参照してください。

## Adobe CX Enterprise Coworkerとの連携

[!DNL GenStudio for Performance Marketing]個のツールは、Adobe CX Enterprise Coworkerのネイティブ接続として管理されます。 組織が可用性を管理しているため、MCP サーバーの直接URLを入力しないでください。

新しい会話を開始し、[接続を確認します](#verify-the-connection)。 ツールが表示されない場合は、組織の管理者またはAdobe担当者にお問い合わせください。

## Connect Claude

Claudeには、Pro、Max、Team、またはEnterprise プランが必要です。 同じリモートコネクタは、Web上のClaudeとデスクトップアプリケーションで機能します。

1. Claudeで、左側のサイドバーで「**[!UICONTROL カスタマイズ]**」を選択します。
1. 「**[!UICONTROL コネクタ]**」を選択し、追加アイコンを選択します。
1. 「**[!UICONTROL カスタムコネクタを追加]**」を選択します。
1. MCP サーバーのURLとして`https://genstudio-services.adobe.io/mcp`を入力します。
1. Adobe IDでログインします。
1. [!DNL GenStudio for Performance Marketing]へのアクセス権を持つIMS組織を選択します。

&#x200B;> [!NOTE]
&#x200B;> グループ版またはエンタープライズ版のプランでは、組織の所有者が最初にコネクタを追加する必要がある場合があります。 コネクタが既に使用可能な場合は、代わりに&#x200B;**[!UICONTROL Connect]**&#x200B;を選択します。

## ChatGPTの接続

ChatGPTには、Plus、Pro、Business、Enterprise、Education アカウントが必要です。 カスタム MCP接続は、開発者モードを通じてweb上で利用できます。

1. Web ブラウザーで[ChatGPT](https://chatgpt.com)にログインします。
1. **[!UICONTROL 設定]**&#x200B;を開き、**[!UICONTROL 開発者モード]**&#x200B;を有効にします。
1. **[!UICONTROL 設定]**&#x200B;で、アプリまたはコネクタの領域を開きます。
1. `GenStudio`という名前のカスタム MCP接続を追加します。
1. MCP サーバーのURLとして`https://genstudio-services.adobe.io/mcp`を入力します。
1. 認証方法として&#x200B;**[!UICONTROL OAuth]**&#x200B;を保持します。
1. Adobe IDでログインします。
1. [!DNL GenStudio for Performance Marketing]へのアクセス権を持つIMS組織を選択します。

&#x200B;> [!NOTE]
> ChatGPTは、開発者とコネクタの設定の場所を変更できます。 これらのラベルがアカウントで異なる場合は、現在のOpenAIの手順に従って、リモート MCP コネクタを追加してください。

## Connect Codex

Codexでは、Codex コマンドラインインターフェイスと認証済みCodex アカウントが必要です。

1. すべてのプロジェクトの`~/.codex/config.toml`を開くか、1つのプロジェクトの`.codex/config.toml`を開きます。
1. 次の設定を追加します。

   ```toml
   [mcp_servers.genstudio]
   url = "https://genstudio-services.adobe.io/mcp"
   auth = "oauth"
   ```

1. `codex mcp login genstudio`を実行します。
1. 開いたブラウザーウィンドウで、Adobe IDでログインします。
1. [!DNL GenStudio for Performance Marketing]へのアクセス権を持つIMS組織を選択します。

## Connect Writer

WriterにはAI Studioへのアクセスが必要です。

1. Writerで、**[!UICONTROL AI Studio]**&#x200B;を開きます。
1. **[!UICONTROL コネクタとツール]**&#x200B;を選択します。
1. 「**[!UICONTROL カスタムコネクタを作成]**」を選択します。
1. コネクタタイプとして「**[!UICONTROL MCP Server]**」を選択します。
1. コネクタの名前と説明を入力します。
1. MCP サーバーのURLとして`https://genstudio-services.adobe.io/mcp`を入力します。
1. コネクタのチームアクセス権を設定します。
1. 認証方法として&#x200B;**[!UICONTROL OAuth 2.0 （ユーザーレベル）]**&#x200B;を選択します。
1. Adobe IDでログインします。
1. 「**[!UICONTROL 保存]**」を選択します。

[!DNL GenStudio for Performance Marketing]個のツールがAI Studio ツールライブラリに表示されます。 各Writer ユーザーは、個々のAdobe IDでログインします。

## Microsoft Copilotへの接続

Microsoftは、Copilotのカスタム MCP接続の設定フローを制御します。 現在の[Microsoft Copilot ドキュメント &#x200B;](https://learn.microsoft.com/en-us/copilot/)に従って、リモート MCP サーバーを追加し、サーバーのURLとして`https://genstudio-services.adobe.io/mcp`を使用します。

プロンプトが表示されたら、Adobe IDでログインし、[!DNL GenStudio for Performance Marketing]へのアクセス権を持つIMS組織を選択します。

## 接続を確認する

設定が完了したら、ツールが使用可能であることを確認します。

1. AI アシスタントで新しい会話を開始します。
1. アクセスできる[!DNL GenStudio for Performance Marketing] ツールをアシスタントに尋ねます。
1. 応答に、Insights、Create、Activateのツールが一覧表示されていることを確認します。
1. 接続された有料メディアチャネルのパフォーマンス概要を尋ねます。

アシスタントは、使用可能なパフォーマンスデータを返すか、リクエストと一致するデータがない理由を説明します。

&#x200B;> [!TIP]
&#x200B;> 認証が失敗した場合は、再接続して、正しいIMS組織を選択したことを確認します。 ツールが表示されない場合は、アカウントが[!DNL GenStudio for Performance Marketing]へのアクセス権を持っていることを確認してください。

## 関連する機能

- [AI アシスタントの概要](overview.md)
- [AI アシスタントの使用](use-ai-assistants.md)
- [AI アシスタントツールリファレンス](tools-reference.md)
