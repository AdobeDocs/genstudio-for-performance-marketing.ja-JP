---
title: メタ広告エクスペリエンスの作成
description: Adobe GenStudio for Performance Marketingを使用して（Facebook や Instagram 用の）オンブランドのメタ広告エクスペリエンスを作成する方法を説明します。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 42111bbf-70cd-4fd2-a7a9-15abe072d720
source-git-commit: f49a2bd241f98dda23f6612f8c699ec49d222a12
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---

# メタ広告エクスペリエンスの作成

このチュートリアルでは、GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) （左側のナビゲーションエリアにある絵筆のアイコン [&#128279;](/help/user-guide/create/meta-experiences.md) を使用して、ブランド化された  メタ広告エクスペリエンス）を生成する方法を説明します。

Meta 広告エクスペリエンスの作成を開始する前に、GenStudio for Performance Marketingで [ ガイドラインを組み込む ](/help/user-guide/guidelines/add-guidelines.md) ことが重要です。また、[ プロンプトの作成 ](/help/user-guide/effective-prompts.md) の基本を理解しておく必要があります。

## テンプレートを選択

新しいメタ広告エクスペリエンスの生成を開始するには、使用可能なテンプレートを使用して、コンテンツのフレームワークを提供します。 サポートされるメタ広告の縦横比について詳しくは、[ テンプレートのベストプラクティス ](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) を参照してください。

**メタ広告テンプレートを選択するには**:

1. _[!DNL Create]_&#x200B;で、「**[!UICONTROL メタ広告]**」をクリックします。
1. _フィルター_ の横にある検索オプションを使用して、特定のメタ広告テンプレートを見つけます。
1. テンプレートをクリックして選択し、「**[!UICONTROL 使用]**」をクリックします。

   これにより、コンテンツ作成の中心となるキャンバスが開きます。

## パラメーターを追加

プロンプトドロワーの _パラメーター_ に [ ガイドライン ](/help/user-guide/guidelines/overview.md) とアセットを追加すると、コンテンツ生成プロセスが強化されます。これは、メタ広告を生成するための準備における重要な手順です。

事前定義済みのガイドライン（[!DNL Brands]、[!DNL Personas]、[!DNL Products]）を含むテンプレートを使用する場合、これらのガイドラインはバリアントに適用されます。 必要に応じて変更できます。

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

ガイドラインを選択したら、自然言語を使用してプロンプトを作成し、新しいメタ広告エクスペリエンスのコンテンツの生成を開始します。 詳細なプロンプトは、あいまいなプロンプトやあいまいなプロンプトよりも高品質の出力を生成します。

プロンプトの書き込みについて詳しくは、[ 効果的なプロンプトの書き込み ](/help/user-guide/effective-prompts.md) を参照してください。

**プロンプトを入力するには**:

1. _生成するエクスペリエンスを記述」_ プロンプトボックスにプロンプトを入力します。
1. 「**[!UICONTROL 生成]**」をクリックします。

デフォルトでは、4 つのバリエーション（追加したプロンプト、ガイドラインおよびコンテンツによってすべて強化される）が生成され、キャンバスに表示されます。

生成されたコンテンツは徐々に読み込まれます。メタエクスペリエンスの各セクションが生成されると、キャンバスに表示されます。 これらの変更がキャンバスにどのように読み込まれるかを学ぶには、[ メタエクスペリエンス ](/help/user-guide/create/meta-experiences.md#progressive-loading) を参照してください。

## メタ広告チャネルを選択

メタ広告を生成する際は、Facebook 広告または Instagram 広告から選択できます。

右側のメニューバー（Facebook および Instagram アイコン **で「メタ広告」チャネルオプションを** Facebook **」と「Instagram**」の間で切り替えて、各チャネルのバリアントを表示および管理します。

[ メタ広告の改訂 ](#revise-generated-variants) 時に、Facebook 広告と Instagram 広告のアスペクト比を変更できます。

## 生成されたバリアントを修正

承認または公開用に送信する内容を選択する前に [!DNL Content] メタ広告を編集したり、生成された広告のセットからバリアントを削除したりできます。

変更する個々のレイヤーをハイライト表示するには、編集可能なフィールドまたは画像をクリックし、「_[!UICONTROL レイヤーを表示]_」をクリックします。

**生成されたバリアントを修正するには**:

* **メタ広告のドラフト名を [ 編集](/help/user-guide/create/manage-variants.md#change-draft-name)** するには、キャンバスの上部にある _名称未設定のドラフト_ タイトルをクリックし、新しいタイトルを入力します。
* **メタ広告を [ 手動で編集](/help/user-guide/create/manage-variants.md#manually-edit-text)** するには、広告セクションのいずれか（件名行など）をクリックします
ヘッダー（本文コピー）を使用し、必要に応じて編集します。
* **コールトゥアクションを変更または選択するには**、「call-to-action」ボタンをクリックし、使用可能なボタンテキストオプションから選択します。 _リンク_ に、call-to-actionテキストの URL を入力します。
<!-- **To [change or select the Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**, click the call-to-action button and select _[!UICONTROL Rephrase]_ or _[!UICONTROL Add link]_. -->
* **バリアント内の画像へのリンクを追加 [ するには](/help/user-guide/create/manage-variants.md#add-image-link)**、画像アセット（画像が現在存在しない場合は画像アセット領域）をクリックし、リンクアイコンをクリックします。
* **バリアントのセクションを [ 再生成](/help/user-guide/create/manage-variants.md#re-generate-sections)** するには、編集可能なテキストフィールドをクリックして _[!UICONTROL 編集候補]_ オプションを使用するか、新しいプロンプトを入力して **[!UICONTROL 生成]** をクリックします。
* **バリアント内の画像を追加 [ 入れ替え](/help/user-guide/create/manage-variants.md#swap-image)** するには、画像アセット（画像が現在存在しない場合は画像アセット領域）をクリックし、**[!UICONTROL コンテンツから入れ替え]** アイコンをクリックします。
* **画像を [ 切り抜きまたは再配置](/help/user-guide/create/manage-variants.md#crop-assets)** するには、画像の上にマウスポインターを置き、表示される切り抜きアイコンをクリックし、画像のサイズと配置を調整します。
* **バリアント内の画像の代替テキストを追加 [ するには](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**、画像アセットをクリックし、「_代替テキスト_」オプションを使用して、画像ごとに代替テキストを手動で追加または生成します。
* **メタ広告を [ 削除](/help/user-guide/create/manage-variants.md#delete-variant)** するには、バリアントのオプションメニューをクリックし、**[!UICONTROL バリアントを削除]** をクリックします。

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

承認パネルは、キャンバスの右側のアクションバーにあるアイコンとしてアクセスでき、レビューを取得したり、レビューのコメントを追跡したり、関係者から承認を得たりできます。

**レビューと承認を取得するには**:

1. [ ドラフトのメタ広告エクスペリエンスの承認 ](/help/user-guide/approvals/request-review.md) を依頼する [ 承認リクエストの開始 ](/help/user-guide/approvals/approve-content.md)。

   ![ レビューおよび承認用のドラフトの送信 ](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. レビュープロセス中に [ レビュー担当者を削除または追加 ](/help/user-guide/approvals/review-and-edit.md#manage-approvals) できます。
1. [ レビュー用にコンテンツにアクセス ](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) し、修正要求を表示します。
1. レビューのコメントごとにドラフトを編集し [ メタ広告エクスペリエンスを公開 ](#publish-and-export-experience) します。

詳しくは、[ レビューと承認 ](/help/user-guide/approvals/overview.md) を参照してください。

## エクスペリエンスの公開と書き出し

生成したメタ広告を現在および将来の使用で使用できるようにするには、[!UICONTROL &#x200B; コンテンツ &#x200B;] に公開し、マーケティングキャンペーンで使用するためにエクスポートします。

1. **新しいメタ広告エクスペリエンスを公開するには** 上部のツールバーまたは承認フロー内の **[!UICONTROL 公開]** をクリックします。
1. **新しいメタ広告エクスペリエンスを書き出すには** 上部のツールバーにある **[!UICONTROL 書き出し]** をクリックします。
   1. 「HTMLと画像」または「CSV と画像（JPGまたは PNG）」のフォーマットを選択し、「**[!UICONTROL 書き出し]**」をクリックします。

詳細は、[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) を参照してください。

## メタを接続

GenStudio for Performance Marketingを Meta に接続して、コンテンツのパフォーマンスに関する高度な分析とインサイトを受け取ることができます。

[ メタ広告の連携 ](/help/user-guide/connectors/meta-ads.md) を参照してください。
