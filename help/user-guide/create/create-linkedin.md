---
title: LinkedIn エクスペリエンスの作成
description: Adobe GenStudio for Performance Marketingを使用して、ブランドに準拠した LinkedIn エクスペリエンスを作成する方法を説明します。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
badgeBeta: label="Beta" tooltip="この機能は現在Betaにあるので、一部の機能が制限されるか、変更される可能性があります。"
recommendations: noDisplay
exl-id: abe10fc8-d6d5-4cad-9273-400b622f22b7
source-git-commit: d5019f1cdceccb8ce2fdd86c54cf2d36673a90aa
workflow-type: tm+mt
source-wordcount: '914'
ht-degree: 0%

---

# LinkedIn エクスペリエンスの作成

このチュートリアルでは、GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) （左側のナビゲーションエリアにある絵筆のアイコン [&#128279;](/help/user-guide/create/meta-experiences.md) を使用して、ブランドガイドラインに準拠した LinkedIn エクスペリエンス）を生成する方法を説明します。

LinkedIn 広告の作成を開始する前に、GenStudio for Performance Marketingで [ ガイドラインの追加 ](/help/user-guide/guidelines/add-guidelines.md) を行い、[ プロンプトの作成 ](/help/user-guide/effective-prompts.md) の基本を学習することが重要です。

## テンプレートを選択

新しい LinkedIn エクスペリエンスを生成するには、コンテンツのフレームワークを提供するテンプレートが必要です。 LinkedIn のサポートされる縦横比について詳しくは、[ テンプレートのベストプラクティス ](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) を参照してください。

**LinkedIn テンプレートを選択するには**:

1. _[!DNL Create]_&#x200B;で&#x200B;**[!UICONTROL LinkedIn]**&#x200B;をクリックします。
1. _フィルター_ の横にある検索オプションを使用して、特定のテンプレートを検索します。
1. クリックしてテンプレートを選択し、**[!UICONTROL 使用]** をクリックします。

   これにより、コンテンツ作成の中心となるキャンバスが開きます。

## パラメーターを追加

プロンプトドロワーの _パラメーター_ に [ ガイドライン ](/help/user-guide/guidelines/overview.md) とアセットを追加すると、コンテンツ生成プロセスが強化されます。これは、LinkedIn エクスペリエンスを生成するための準備における重要な手順です。

**パラメーターとアセットを追加するには**:

1. _パラメーター_ アイコンをクリックして、プロンプトドロワーを展開します。
1. 「_パラメーター_」セクションで、ガイドライン（[!DNL Brands]、[!DNL Personas]、[!DNL Products]）を選択して、コンテンツの作成を通知します。

   ![ ペルソナを選択 ](/help/assets/persona-select.png){width="600" zoomable="yes"}

   これらのメニューから利用できるブランド、ペルソナ、製品がない場合は、[GenStudio for Performance Marketingにガイドラインを追加 ](/help/user-guide/guidelines/add-guidelines.md) します。

1. コンテンツの生成に影響を与えるために、エクスペリエンス *および* で使用するコンテンツを追加します。
   * **[!UICONTROL コンテンツから選択]** をクリックして、[!DNL Content] リポジトリからアセット（画像）を選択し、1 つ以上の画像をフィルタリングして選択します。

     ![ ビジュアルコンテンツを選択 ](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

     接続された [!DNL AEM Assets Content Hub] リポジトリのアセットを使用するには、_場所_ ドロップダウンメニューからリポジトリを選択します。 1 つ以上の画像のフィルタリングと選択

   * または、アセットを「**[!UICONTROL コンテンツから選択]** セクションにドラッグ&amp;ドロップして、1 つ以上の新しいアセットをアップロードします。
1. **[!UICONTROL 使用]** をクリックします。

パラメーターの追加が完了したら、「_パラメーター_」アイコンをもう一度クリックすると、プロンプトドロワーを折りたたむことができます。

## プロンプトを入力

ガイドラインを選択したら、自然言語を使用してプロンプトを作成し、新しい LinkedIn エクスペリエンスのコンテンツの生成を開始します。 詳細なプロンプトは、良質で有用な出力を受け取ることを保証します。

プロンプトの書き込みについて詳しくは、[ 効果的なプロンプトの書き込み ](/help/user-guide/effective-prompts.md) を参照してください。

**プロンプトを入力するには**:

1. _生成するエクスペリエンスを記述」_ プロンプトボックスにプロンプトを入力します。
1. 「**[!UICONTROL 生成]**」をクリックします。

デフォルトでは、4 つのバリエーション（追加したプロンプト、ガイドラインおよびコンテンツによってすべて強化される）が生成され、キャンバスに表示されます。

生成されたコンテンツは徐々に読み込まれます。LinkedIn エクスペリエンスの各セクションが生成されると、キャンバスに表示されます。 これらの変更をキャンバスに読み込む方法については、[LinkedIn エクスペリエンス ](/help/user-guide/create/linkedin-experiences.md#progressive-loading) を参照してください。

## 生成された LinkedIn 広告を変更

[!DNL Content] に承認または公開するためのバリアントを送信する前に、LinkedIn 広告を編集するか、生成された広告のセットからバリアントを削除できます。

**生成されたバリアントを修正するには**:

* **LinkedIn とドラフトの名前を [ 編集](/help/user-guide/create/manage-variants.md#change-draft-name)** するには、キャンバスの上部にある _名称未設定のドラフト_ タイトルをクリックして、新しいタイトルを入力します。
* **LinkedIn 広告を [ 手動で編集](/help/user-guide/create/manage-variants.md#manually-edit-text)** するには、任意の広告セクション（件名行、ヘッダー、本文コピーなど）をクリックし、必要に応じて編集します。
* **コールトゥアクションを変更または選択するには**、「call-to-action」ボタンをクリックし、使用可能なボタンテキストオプションから選択します。 _リンク_ に、call-to-actionテキストの URL を入力します。
* **バリアントのセクションを [ 再生成](/help/user-guide/create/manage-variants.md#re-generate-sections)** するには、編集可能なテキストフィールドをクリックして _[!UICONTROL 編集候補]_ オプションを使用するか、_[!UICONTROL Generate new text_ セクションに新しいプロンプトを入力して &#x200B;]&#x200B;**[!UICONTROL Generate]** をクリックします。
* **画像を [ 切り抜きまたは再配置](/help/user-guide/create/manage-variants.md#crop-assets)** するには、画像の上にマウスポインターを置き、表示される切り抜きアイコンをクリックし、画像のサイズと配置を調整します。
* **LinkedIn 広告を [ 削除](/help/user-guide/create/manage-variants.md#delete-variant)** するには、バリアントのオプションメニューをクリックし、**[!UICONTROL バリアントを削除]** をクリックします。

## 生成フィードバックを送信

生成出力の品質に関する [ フィードバックを送信 ](/help/user-guide/create/manage-variants.md#generation-feedback) するには、オプションアイコン（3 つのドット）をクリックし、**[!UICONTROL 良好な出力]** または **[!UICONTROL 不良な出力]** を選択します。

## コンテンツチェックの整合性の確認

生成されたバリアントを最適化し、ブランド ID、プラットフォームガイドラインおよびアクセシビリティ標準に厳密に準拠するには、[_コンテンツチェック_ パネル ](/help/user-guide/guidelines/brand-validation.md#content-check-panel) の機能を活用します。 このパネルには、包括的なコンテンツチェックの詳細が表示され、改善点が明らかになります。

**バリアントに対してコンテンツチェックを実行するには**:

1. 右側のアクションバーにある _コンテンツチェック_ パネルアイコンをクリックして、[_コンテンツチェック_ パネル ](/help/user-guide/guidelines/brand-validation.md#content-check-panel) を開きます。 *レビューが必要* チェックと *合格* チェックの概要を表示し、改善が必要なセクションとガイドラインを確認します。

   ![_コンテンツチェック_ パネル ](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [ バリアントを手動で改訂 ](#revise-generated-variants) し、バリアントが実行されたコンテンツチェックと密接に連携していることを確認します。

[ ブランド検証 ](/help/user-guide/guidelines/brand-validation.md) を参照してください。

## レビューと承認の取得

キャンバスの上部のメニューバーからアクセスできる承認パネルを使用して、レビューを取得、レビューコメントを追跡、関係者からの承認を取得します。

**レビューと承認を取得するには**:

1. [ ドラフトのメタ広告エクスペリエンスの承認 ](/help/user-guide/approvals/request-review.md) を依頼する [ 承認リクエストの開始 ](/help/user-guide/approvals/approve-content.md)。

   ![ レビューおよび承認用のドラフトの送信 ](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. レビュープロセス中に [ レビュー担当者を削除または追加 ](/help/user-guide/approvals/review-and-edit.md#manage-approvals) できます。
1. [ レビュー用にコンテンツにアクセス ](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) し、修正要求を表示します。
1. レビューのコメントごとにドラフトを編集し [ メタ広告エクスペリエンスを公開 ](#publish-and-export-experience) します。

詳しくは、[ レビューと承認 ](/help/user-guide/approvals/overview.md) を参照してください。

## エクスペリエンスの公開と書き出し

生成した LinkedIn 広告を現在および将来の使用で利用できるようにするには、広告を [!UICONTROL &#x200B; コンテンツ &#x200B;] に公開し、マーケティングキャンペーンで使用するために書き出します。

1. **新しいエクスペリエンスを公開するには** 上部のツールバーまたは承認フロー内の **[!UICONTROL 公開]** をクリックします。
1. **新しいエクスペリエンスを書き出すには**、上部のツールバーにある **[!UICONTROL 書き出し]** をクリックします。
   1. JPG、PNG、GIFのいずれかのフォーマットを選択し、「**[!UICONTROL エクスポート]**」をクリックします。

詳細は、[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) を参照してください。
