---
title: メールエクスペリエンスの作成
description: Adobe GenStudio for Performance Marketingでメールエクスペリエンスを作成する方法を説明します。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 34446202-da98-45ff-869a-b43496a477f8
source-git-commit: 47195c08f500e50a01db127c6badc461c10afaf9
workflow-type: tm+mt
source-wordcount: '1083'
ht-degree: 0%

---

# メールエクスペリエンスの作成

このチュートリアルでは、GenStudio for Performance Marketing [ （左側のナビゲーションエリアにある絵筆のアイコン ](/help/user-guide/create/email-experiences.md) を使用して、ブランド化された [[!DNL Create]](/help/user-guide/create/overview.md) メールエクスペリエンス）を生成する方法を説明します。

効果的なメールエクスペリエンスを作成するには、開始する前に [GenStudio for Performance Marketingにガイドラインを追加 ](/help/user-guide/guidelines/add-guidelines.md) し、[ プロンプトの作成の基本 ](/help/user-guide/effective-prompts.md) をブラッシュアップすることをお勧めします。

## テンプレートを選択

新しいメールエクスペリエンスを作成するには、使用可能なテンプレートを使用してコンテンツのフレームワークを提供します。

**メールテンプレートを選択するには**:

1. _[!DNL Create]_&#x200B;で、「**[!UICONTROL メール]**」をクリックします。
1. _フィルター_ の横にある検索オプションを使用して、特定のメールテンプレートを検索します。
1. クリックしてメールテンプレートを選択し、「**[!UICONTROL 使用]**」をクリックします。

   コンテンツ作成の中心となるキャンバスが表示されます。

## パラメーターを追加

プロンプトドロワーの [ パラメーター ](/help/user-guide/guidelines/overview.md) に _ガイドライン_ とアセットを追加すると、コンテンツ生成プロセスが過大評価され、メールエクスペリエンスを生成するための不可欠な準備手順となります。

事前定義済みのガイドライン（[!DNL Brands]、[!DNL Personas]、[!DNL Products]）を含むテンプレートを使用する場合、これらのガイドラインはバリアントに適用されます。 必要に応じて変更できます。

**パラメーターとアセットを追加するには**:

1. _パラメーター_ アイコンをクリックして、プロンプトドロワーを展開します。
1. 「_パラメーター_」セクションで、ガイドライン（[!DNL Brands]、[!DNL Personas]、[!DNL Products]）を選択して、コンテンツの作成を通知します。

   ![ ペルソナを選択 ](/help/assets/persona-select.png){width="600" zoomable="yes"}

   これらのメニューから利用できるブランド、ペルソナ、製品がない場合は、[GenStudio for Performance Marketingにガイドラインを追加 ](/help/user-guide/guidelines/add-guidelines.md) します。

1. コンテンツの生成に影響を与えるために、エクスペリエンス *および* で使用するコンテンツを追加します。
   * **[!UICONTROL コンテンツから選択]** をクリックして、[!DNL Content] リポジトリからアセット（画像）を選択し、1 つ以上の画像をフィルタリングして選択します。

     ![ ビジュアルコンテンツを選択 ](/help/assets/content-select-email.png){width="500" zoomable="yes"}

     接続された [!DNL AEM Assets Content Hub] リポジトリのアセットを使用するには、_場所_ ドロップダウンメニューからリポジトリを選択します。 1 つ以上の画像のフィルタリングと選択

   * または、アセットを「**[!UICONTROL コンテンツから選択]** セクションにドラッグ&amp;ドロップして、1 つ以上の新しいアセットをアップロードします。
1. **[!UICONTROL 使用]** をクリックします。

   >[!NOTE]
   >メールテンプレートに複数のセクションがある場合、[!DNL Products] 複数セクションのメール _の各メールセクションに_ とコンテンツ（ビジュアルアセット）を選択します。 複数セクションのメールで、セクションごとに 1 つのビジュアルアセットを使用できます。 [!DNL Content] から複数セクションのメールにビジュアルアセットのみを追加できます。ローカルソースからアセットをドラッグ&amp;ドロップまたはアップロードすることはできません。
   >![ 各メールセクションのコンテンツとパラメーターの追加 ](/help/assets/parameters-multisection-email.png){width="450" zoomable="yes"}

パラメーターの追加が完了したら、「_パラメーター_」アイコンをもう一度クリックすると、プロンプトドロワーを折りたたむことができます。

## プロンプトを入力

ガイドラインを選択したら、自然言語を使用してプロンプトを作成し、新しいメールエクスペリエンスのコンテンツの生成を開始します。 詳細なプロンプトは、あいまいなプロンプトやあいまいなプロンプトよりも高品質の出力を生成します。

プロンプトの書き込みについて詳しくは、[ 効果的なプロンプトの書き込み ](/help/user-guide/effective-prompts.md) を参照してください。

**プロンプトを入力するには**:

1. _生成するエクスペリエンスを記述」_ プロンプトボックスにプロンプトを入力します。
1. 「**[!UICONTROL 生成]**」をクリックします。

デフォルトでは、4 つのバリエーション（追加したプロンプト、ガイドラインおよびコンテンツによってすべて強化される）が生成され、キャンバスに表示されます。

生成されたコンテンツは徐々に読み込まれます。メールエクスペリエンスの各セクションが生成されると、キャンバスに表示されます。 これらの変更がキャンバスにどのように読み込まれるかを学ぶには、[ メールエクスペリエンス ](/help/user-guide/create/meta-experiences.md#progressive-loading) を参照してください。

## 生成されたバリアントを修正

承認または公開用に送信する内容を選択する前に [!DNL Content] メールセクションを編集したり、生成された一連のメールからバリアントを削除したりできます。

**生成されたバリアントを修正するには**:

* **メールドラフト名を [ 編集](/help/user-guide/create/manage-variants.md#change-draft-name)** するには、キャンバスの上部にある _名称未設定のドラフト_ タイトルをクリックし、新しいタイトルを入力します。
* **メールを [ 手動で編集](/help/user-guide/create/manage-variants.md#manually-edit-text)** するには、編集可能なテキストフィールド（件名行、ヘッダー、本文コピーなど）のいずれかをクリックし、必要に応じて編集します
* **Call to actionを [ 変更または選択](/help/user-guide/create/manage-variants.md#revise-call-to-action)** するには、「call-to-action」ボタンをクリックし、「_[!UICONTROL フレーズ変更]_」または _[!UICONTROL リンクを追加]_ を選択します。
* **バリアントの [ テキストの書式設定を適用する](/help/user-guide/create/manage-variants.md#manually-edit-text)** には、バリアントの画像上のテキストをクリックし、**[!UICONTROL テキストの書式設定]** をクリックします。
* **バリアントのセクションを [ 再生成](/help/user-guide/create/manage-variants.md#re-generate-sections)** するには、編集可能なテキストフィールドをクリックして _[!UICONTROL 編集候補]_ オプションを使用するか、新しいプロンプトを入力して **[!UICONTROL 生成]** をクリックします。
* **バリアント内の画像を追加 [ 入れ替え](/help/user-guide/create/manage-variants.md#swap-image)** するには、画像アセット（画像が現在存在しない場合は画像アセット領域）をクリックし、**[!UICONTROL コンテンツから入れ替え]** アイコンをクリックします。
* **バリアント内の画像へのリンクを追加 [ するには](/help/user-guide/create/manage-variants.md#add-image-link)**、画像アセット（画像が現在存在しない場合は画像アセット領域）をクリックし、リンクアイコンをクリックします。
* **バリアント内の画像の代替テキストを追加 [ するには](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**、画像アセットをクリックし、「_代替テキスト_」オプションを使用して、画像ごとに代替テキストを手動で追加または生成します。
* **バリアントに [ アクセシビリティラベルを追加 ](/help/user-guide/create/manage-variants.md#add-accessibility-labels) するには** 画像またはcall-to-action リンクをクリックし、リンクまたはボタンの機能を説明する簡単な説明を入力します。
* **メールを [ 削除](/help/user-guide/create/manage-variants.md#delete-variant)** するには、をクリックしてメールのタイトル（「メール 1/4」など）を選択し、「**[!UICONTROL バリアントを削除]**」をクリックします。

## 生成フィードバックを送信

生成出力の品質に関する [ フィードバックを送信 ](/help/user-guide/create/manage-variants.md#generation-feedback) するには、オプションアイコン（3 つのドット）をクリックし、**[!UICONTROL 良好な出力]** または **[!UICONTROL 不良な出力]** を選択します。

## デバイスのプレビュー

メールエクスペリエンスを修正および準備する際に、ドラフトバリアントの一貫性と視覚的魅力を確保するために、[ デスクトップビューとモバイルビューのプレビューを切り替える ](/help/user-guide/create/manage-variants.md#preview-for-device) ことができます。

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

1. [ ドラフトのメールエクスペリエンスの承認 ](/help/user-guide/approvals/request-review.md) を依頼する [ 承認リクエストの開始 ](/help/user-guide/approvals/approve-content.md)。
1. レビュープロセス中に [ レビュー担当者を削除または追加 ](/help/user-guide/approvals/review-and-edit.md#manage-approvals) できます。
1. [ レビュー用にコンテンツにアクセス ](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) し、修正要求を表示します。
1. レビューコメントごとにドラフトを編集し、[ メールエクスペリエンスを公開する ](#publish-and-export-experience) ようにします。

詳しくは、[ レビューと承認 ](/help/user-guide/approvals/overview.md) を参照してください。

## エクスペリエンスの公開と書き出し

生成されたメールを現在および将来の使用で使用できるようにするには、メールを [!UICONTROL &#x200B; コンテンツ &#x200B;] に公開し、マーケティングキャンペーンで使用するために書き出します。

1. **新しいメールエクスペリエンスを公開するには** 上部のツールバーまたは承認フロー内の **[!UICONTROL 公開]** をクリックします。
1. **新しいメールエクスペリエンスを書き出すには**、上部のツールバーにある **[!UICONTROL 書き出し]** をクリックします。
   1. 形式（CSV と画像またはHTMLのみ）を選択し、「**[!UICONTROL 書き出し]**」をクリックします。

詳細は、[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) を参照してください。
