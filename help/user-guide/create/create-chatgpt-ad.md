---
title: ChatGPT広告エクスペリエンスの作成
description: Adobe GenStudio for Performance MarketingでChatGPTの有料メディアエクスペリエンスを作成、レビュー、公開、アクティベートする方法について説明します。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
source-git-commit: 0f5bc2b5416193c01cc4b2fc96d9cb575e209aa3
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 9%

---


# ChatGPT広告体験の作成

[!DNL GenStudio for Performance Marketing]の[[!DNL Create]](/help/user-guide/create/overview.md)を使用して、生成、ブランドとチャネルのチェック、承認、[!DNL Content]への公開、およびMetaやGoogle Campaign Manager 360などのチャネルに使用されているのと同じ[!DNL Activate] フローでのアクティベーションを通じて、ガイドラインとアセットから&#x200B;**ChatGPT広告**&#x200B;を有料メディアエクスペリエンスとして構築します。

開始する前に、必要に応じて[&#x200B; ガイドライン &#x200B;](/help/user-guide/guidelines/add-guidelines.md)を追加し、[効果的なプロンプト &#x200B;](/help/user-guide/effective-prompts.md)を確認して、見出しプロンプトで強力なバリエーションを生成します。

## 前提条件

[!DNL GenStudio for Performance Marketing]でChatGPT広告を作成またはアクティブ化する前に、これらの前提条件に従って設定する必要があります。

### アクセスと役割

* [!DNL GenStudio for Performance Marketing]に&#x200B;**編集者**&#x200B;以上の役割があります。 [&#x200B; ユーザーの役割と権限 &#x200B;](/help/user-guide/user-roles.md) を参照してください。
* **OpenAI広告アカウント**&#x200B;とそのアカウントの&#x200B;**API キー**&#x200B;があります。
* **ChatGPT Ads** アカウントが[!DNL GenStudio for Performance Marketing]に接続されています。

OpenAI Ads ManagerでAPI キーを作成するには：

1. OpenAI Ads Managerで、**[!UICONTROL Settings]** > **[!UICONTROL API Keys]** > **[!UICONTROL Create New Key]**&#x200B;に移動します。

[!DNL GenStudio for Performance Marketing]でChatGPT Ads アカウントを接続するには：

1. 左下の領域で、**[!UICONTROL 詳細]** > **[!UICONTROL 設定]** > **[!UICONTROL ChatGPT]** > **[!UICONTROL 接続]** > **[!UICONTROL アカウントを追加]**&#x200B;をクリックします。
1. OpenAI広告アカウントの名前を入力し、API キーを貼り付けて、**[!UICONTROL アカウントを追加]**&#x200B;をクリックします。

フローが正常に完了すると、広告アカウントが接続されます。

### 設定の作成

* アプリがブランドに即したコピーを生成できるように、**[!DNL Brands]**、**[!DNL Products]**&#x200B;および&#x200B;**[!DNL Personas]**&#x200B;が設定されています。 [&#x200B; ガイドラインの概要](/help/user-guide/guidelines/overview.md)を参照してください。
* 使用する画像は、[[!DNL Content]](/help/user-guide/content/overview.md)で利用できます。

## ChatGPT広告の生成

[!DNL Create] ワークスペースでChatGPT広告を有料メディアエクスペリエンスとして作成します。

### ChatGPT エクスペリエンスを開始

ChatGPT作成を開くには：

1. **[!UICONTROL 作成]** / **[!UICONTROL ChatGPT]**&#x200B;に移動します。 ChatGPTのテンプレートは選択しません。1つの広告レイアウトが使用されます。
   作成ワークフロー![&#128279;](./create-chatgpt-clp.png){width="60%"}のChatGPT タイル
1. _キャンバス_&#x200B;で、**[!DNL Brand]**、**[!DNL Product]**、**[!DNL Persona]**&#x200B;および&#x200B;**言語**&#x200B;を選択します。
1. [!DNL Content]から画像を選択します。
1. ChatGPTの見出しコピーのプロンプトを入力します。
1. 「**[!UICONTROL 生成]**」をクリックします。

[!DNL GenStudio for Performance Marketing] **は4つの** クリエイティブのバリエーションを生成します。

実行できる操作：

* トーン、長さ、強調を調整するには、**[!UICONTROL 再生成]** または **[!UICONTROL リファイン]** を使用します。
* _キャンバス_&#x200B;で直接テキストを編集します。
* **[!UICONTROL スワップ]**&#x200B;を使用して、[!DNL Content]から代替画像を選択します。

生成されたエクスペリエンスを編集する方法の詳細については、[&#x200B; バリエーションの管理](/help/user-guide/create/manage-variants.md)を参照してください。

### ブランドチェックとチャネルチェックの実行

エクスペリエンスを保存またはレビュー用に送信する前に、ブランドおよびチャネルのルールに照らし合わせてコピーとレイアウトを検証します。

コンテンツチェックを実行するには：

1. **[!UICONTROL コンテンツチェック]** （ブランドチェックとチャネルチェック）をクリックします。
1. [_コンテンツチェック_ パネル &#x200B;](/help/user-guide/guidelines/brand-validation.md#content-check-panel)で検証結果を確認します。
1. バリエーションを編集したり、必要に応じて再生成することで、コピーの長さや画面テキストの高密度さなどのフラグが立った問題を解決できます。

[&#x200B; ブランド検証](/help/user-guide/guidelines/brand-validation.md)を参照してください。

## [!DNL GenStudio for Performance Marketing]にChatGPT広告を保存

保存すると、ChatGPT広告エクスペリエンスが[!DNL Content]に移動され、レビュー、再利用、アクティベートできるようになります。

次の 2 つの状態があります。

* **ドラフトエクスペリエンス** – 進行中で承認されていません。
* **公開されたエクスペリエンス** — [!DNL Content]で承認され、アクティブ化に利用できます。

### レビュー用に送信

1. エクスペリエンスのヘッダーから、「**[!UICONTROL レビューを依頼]**」をクリックします。
1. 承認者（ブランド、法務、パフォーマンスの関係者など）を選択します。
1. オプション：**[!UICONTROL 設定]**&#x200B;でメモを追加します。
1. **[!UICONTROL レビュー用に送信]** をクリックします。

承認者は、ChatGPT エクスペリエンス、ブランドおよびチャネルのチェック結果を表示したり、**[!UICONTROL 承認]**&#x200B;または変更を依頼したりできます。

[&#x200B; レビューと承認を依頼](/help/user-guide/approvals/request-review.md)および[&#x200B; レビューと承認](/help/user-guide/approvals/overview.md)を参照してください。

### コンテンツに公開

すべての必要な承認が完了したら、次の手順で[!DNL Content]に公開します。

1. **[!UICONTROL コンテンツに公開]** をクリックします。
1. メタデータの確認（例：キャンペーン名やアクティベーション名、地域、言語、ペルソナ、funnel ステージ、チャネル：ChatGPT **など）**
1. 「**[!UICONTROL 公開する]**」をクリックします。

ChatGPT広告は[!DNL Content]に表示され、チャネルやキャンペーンなどのフィルターで検索でき、[!DNL Activate]で選択する準備が整っています。

[承認済みコンテンツを公開](/help/user-guide/approvals/publish-content.md)および[[!DNL Content] 概要](/help/user-guide/content/overview.md)を参照してください。

## ChatGPT広告をアクティベートする

ChatGPT アクティベーションでは、MetaおよびGoogle Campaign Manager 360と同じ[[!DNL Activate]](/help/user-guide/activation/overview.md) モジュールが使用されます。 共有アクティベーションワークフローについては、[&#x200B; アクティベーションの作成](/help/user-guide/activation/create-activation.md)を参照してください。

### ChatGPT アクティベーションを開始

[!DNL Content]または[!DNL Activate]から開始できます。

**[!DNL Content]**&#x200B;から

* 1つ以上の&#x200B;**公開** ChatGPT エクスペリエンスを選択します。

**[!DNL Activate]**&#x200B;から

* **ChatGPT** カードを開き、**[!UICONTROL +新規]**&#x200B;をクリックします。

各エクスペリエンスは&#x200B;**one**&#x200B;個のChatGPT広告にマッピングされます。

### エクスペリエンス設定の指定

選択した各エクスペリエンスに対して、次の内容を確認します。

* **タイトル**
* **本文**
* **ターゲット URL** – 有効な`https://`形式（例：`https://www.example.com`）を使用する必要があります。

### プラットフォーム設定の指定

ChatGPT Ads Managerの詳細を選択します。

* **OpenAI Ads アカウント**
* **ChatGPT Campaign** — OpenAI Ads Managerに既に存在する必要があります。
* **ChatGPT広告グループ** — OpenAI Ads Managerに既に存在する必要があります。
* **ChatGPT広告名** — ChatGPT広告ごとに1つの異なる名前。

### レビューと公開

1. クリエイティブおよびプラットフォームの詳細をすべて確認します。
1. 「**[!UICONTROL 公開する]**」をクリックします。

[!DNL GenStudio for Performance Marketing]さんが&#x200B;**非アクティブ**&#x200B;状態でChatGPT Ads Managerに広告をプッシュするので、メディアチームは最終的なローンチのタイミングと予算を他の有料チャネルと同じように制御できます。 [概要をアクティブ化](/help/user-guide/activation/overview.md)を参照してください。

### 公開後に何が起こるか

* 進行中の&#x200B;**公開中**&#x200B;のモーダルが表示され、自動的に閉じます。
* 最新のアクティベーションを一覧表示する&#x200B;**ChatGPT アクティベーション** テーブルにリダイレクトされます。 処理完了中にステータスに「**[!UICONTROL 保留中]**」が表示される。
* 公開完了時に移動することができます。

処理が完了すると：

* 確認ポップアップに&#x200B;**成功**&#x200B;または&#x200B;**失敗**&#x200B;が表示されます。
* ポップアップをクリックするか、アクティベーションテーブルでChatGPT アクティベーションを開くと、**Details** ページが表示されます。
* アクティベーション **[!UICONTROL 失敗]**&#x200B;した場合、テーブルには、ステータスとChatGPTからのエラーメッセージが表示されます。

OpenAI Ads Managerでは、メディアチームは最終チェックを実施し、準備ができたら広告や広告グループを公開することができます。
