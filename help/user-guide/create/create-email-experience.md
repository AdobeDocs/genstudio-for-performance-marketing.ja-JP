---
title: メール体験の構築
description: Adobe GenStudio for Performance Marketingで電子メール体験を構築する方法を説明します。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 34446202-da98-45ff-869a-b43496a477f8
TQID: https://experienceleague.adobe.com/RPeJQ02q9HXBSpn-uFqjzLCYbbzv5eNnFBXkFn9j5JI
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2: id: a8b28c00-da6e-4d27-8667-80f790ad8972id: be495d08-ecd1-455f-951e-c22de504e667id: de1f9646-abd3-4e21-9de2-df62ce55c8dcid: dee4e9a9-78d1-4953-8179-f8da6117027did: e3878dde-4b87-4290-9e81-ed7ee6eb83feid: f54ee13b-9545-4d68-9842-a12026e60aaf
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
source-git-commit: ecda1f61abaafe858629fc4700f61d89e2ab9e3e
workflow-type: tm+mt
source-wordcount: 1132
ht-degree: 0%

---

# メール体験の構築

このチュートリアルでは、GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) （左側のナビゲーション領域のペイントブラシアイコン）を使用して、ブランドの[ メールエクスペリエンス ](/help/user-guide/create/email-experiences.md)を生成する方法を説明します。

効果的な電子メール体験を実現するには、[GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md)にガイドラインを追加し、[ プロンプトの作成の基本](/help/user-guide/effective-prompts.md)をブラッシュアップしてから開始することをお勧めします。

## テンプレートの選択

新しいメール体験を作成するには、利用可能なテンプレートを使用して、コンテンツのフレームワークを提供します。

**電子メールテンプレートを選択するには**:

1. _[!DNL Create]_で、**[!UICONTROL 電子メール]**をクリックします。
1. _フィルター_&#x200B;の横にある検索オプションを使用して、特定の電子メールテンプレートを検索します。
1. クリックして電子メールテンプレートを選択し、**[!UICONTROL 使用]**&#x200B;をクリックします。

   コンテンツ制作の中心であるカンバスが表示されます。

## パラメーターを追加

プロンプトの引き出しに[ ガイドライン ](/help/user-guide/guidelines/overview.md)と&#x200B;_パラメーター_&#x200B;のアセットを追加すると、コンテンツ生成プロセスが強化され、メール体験を生成するための不可欠な準備ステップになります。

事前に定義されたガイドライン（[!DNL Brands]、[!DNL Personas]、[!DNL Products]など）を含むテンプレートを使用している場合、これらのガイドラインはバリエーションに適用されます。 必要に応じてそれらを変更できます。

**パラメーターとアセットを追加するには**:

1. _パラメーター_ アイコンをクリックして、プロンプトドロワーを展開します。
1. 「_パラメーター_」セクションで、コンテンツ作成に役立つガイドライン（[!DNL Brands]、[!DNL Personas]、および[!DNL Products]）を選択します。

   ![ ペルソナの選択](/help/assets/persona-select-email2.png){width="50%" align="center"}

   これらのメニューから利用できるブランド、ペルソナ、または製品がない場合は、[GenStudio for Performance Marketingにガイドラインを追加します](/help/user-guide/guidelines/add-guidelines.md)。

1. エクスペリエンス *および*&#x200B;で使用するコンテンツを追加して、コンテンツ生成に影響を与えます。
   * 「**[!UICONTROL コンテンツから選択]**」をクリックして、[!DNL Content] リポジトリからアセット（画像）を選択し、フィルターを実行して1つ以上の画像を選択します。

     ![ ビジュアルコンテンツの選択](/help/assets/content-select-email.png){width="500" zoomable="yes"}

     接続された[!DNL AEM Assets Content Hub] リポジトリからアセットを使用するには、_場所_ ドロップダウンメニューからリポジトリを選択します。 1つまたは複数の画像をフィルタリングして選択します。

   * または、**[!UICONTROL コンテンツから選択]** セクションにアセットをドラッグ&amp;ドロップして、1つ以上の新しいアセットをアップロードします。
1. 「**[!UICONTROL 使用]**」をクリックします。

   >[!NOTE]
   >メールテンプレートに複数のセクションがある場合、_複数セクションのメール_&#x200B;の各メールセクションの[!DNL Products]とコンテンツ（ビジュアルアセット）を選択します。 マルチセクションメールでは、セクションごとに1つのビジュアルアセットをサポートします。 ビジュアルアセットを追加できるのは[!DNL Content]のマルチセクションメールのみです。ローカルソースからアセットをドラッグ&amp;ドロップまたはアップロードすることはできません。
   >![各電子メールセクションのコンテンツとパラメーターを追加](/help/assets/parameters-multisection-email.png){width="450" zoomable="yes"}

パラメーターの追加が完了したら、_パラメーター_ アイコンをもう一度クリックして、プロンプトドロワーを折りたたむことができます。

## プロンプトを入力

ガイドラインを選択したら、自然言語を使ってプロンプトを作成し、新しいメール体験用のコンテンツを生成します。 詳細なプロンプトは、曖昧なプロンプトよりも高品質です。

プロンプトの作成について詳しくは、[効果的なプロンプトの作成](/help/user-guide/effective-prompts.md)を参照してください。

**プロンプトを入力するには**:

1. _「生成するエクスペリエンスについて説明する」プロンプト ボックスにプロンプトを入力します。_
1. 「**[!UICONTROL 生成]**」をクリックします。

デフォルトでは、4つのバリエーション（プロンプト、ガイドライン、追加したコンテンツがすべてベース）が生成され、キャンバスに表示されます。

生成されたコンテンツは、電子メールエクスペリエンスの各セクションが生成されるにつれて、段階的に読み込まれます。 それらの変更がキャンバスにどのように読み込まれるかについては、[電子メールエクスペリエンス ](/help/user-guide/create/meta-experiences.md#progressive-loading)を参照してください。

## 生成したバリエーションを修正

承認または[!DNL Content]への公開のために送信するものを選択する前に、生成されたメールのセットからメールセクションを編集したり、バリエーションを削除したりできます。

**生成されたバリエーションを修正するには**:

* **メールのドラフト名](/help/user-guide/create/manage-variants.md#change-draft-name)**&#x200B;を[編集するには、キャンバスの上部にある&#x200B;_名称未設定のドラフト_ タイトルをクリックし、新しいタイトルを入力します。
* **手動で電子メールを編集するには](/help/user-guide/create/manage-variants.md#manually-edit-text)**、編集可能なテキストフィールド（件名、ヘッダー、本文など）のいずれかをクリックし、必要に応じて編集します[
* **承認済みコンテンツフラグメントをメールのバリエーション [で使用するには、[!DNL GenStudio for Performance Marketing]が生成フィールド、挿入コンテンツフラグメントフィールド、ロックされたフィールドを1つのキャンバスに組み合わせる方法について説明します。](/help/user-guide/create/email-experiences.md#content-fragment-swap)**&#x200B;管理者は、[ コンテンツフラグメント拡張機能の検索](/help/extensibility/deploy-app.md#find-content-fragment-extension)の説明に従ってフラグメントソースを設定します。
* **Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**&#x200B;を[変更または選択するには、「call-to-action」ボタンをクリックし、_[!UICONTROL 言い換え]_&#x200B;または&#x200B;_[!UICONTROL リンクを追加]_&#x200B;を選択します。
* **バリエーションで[ テキストの書式設定](/help/user-guide/create/manage-variants.md#manually-edit-text)**&#x200B;を適用するには、バリエーションの画像テキストをクリックし、**[!UICONTROL テキストの書式設定]**&#x200B;をクリックします。
* **バリアント](/help/user-guide/create/manage-variants.md#re-generate-sections)**&#x200B;のセクションを[再生成するには、編集可能なテキストフィールドをクリックして&#x200B;_[!UICONTROL おすすめ編集]_ オプションを使用するか、新しいプロンプトを入力して&#x200B;**[!UICONTROL 生成]**&#x200B;をクリックします。
* **バリアントの画像を[追加または入れ替えるには、](/help/user-guide/create/manage-variants.md#swap-image)**&#x200B;画像アセット （または画像が現在存在しない場合は画像アセット領域）をクリックし、**[!UICONTROL コンテンツから入れ替え]** アイコンをクリックします。
* **バリアント](/help/user-guide/create/manage-variants.md#add-image-link)**&#x200B;の画像にリンクを[追加するには、画像アセット（または画像が現在存在しない場合は画像アセット領域）をクリックし、リンクアイコンをクリックします。
* **バリアント](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**&#x200B;の画像に代替テキストを[追加するには、画像アセットをクリックし、_代替テキスト_ オプションを使用して、画像ごとに代替テキストを手動で追加または生成します。
* **バリエーションに[ アクセシビリティラベル ](/help/user-guide/create/manage-variants.md#add-accessibility-labels)を追加するには**&#x200B;画像またはcall-to-action リンクをクリックし、リンクまたはボタンの機能を説明する簡単な説明を入力します。
* **メールを[削除](/help/user-guide/create/manage-variants.md#delete-variant)**&#x200B;するには、クリックしてメールタイトル（「メール 1/4」など）を選択し、**[!UICONTROL バリアントを削除]**&#x200B;をクリックします。

## 生成フィードバックを送信

生成出力の品質に関するフィードバック ](/help/user-guide/create/manage-variants.md#generation-feedback)を[送信するには、オプションアイコン（3つのドット）をクリックし、**[!UICONTROL 良好な出力]**&#x200B;または&#x200B;**[!UICONTROL 不良な出力]**&#x200B;を選択します。

## デバイスのプレビュー

電子メールエクスペリエンスを修正および準備する際に、ドラフトのバリエーションの一貫性と視覚的な訴求力を確保するために、[ デスクトップ版とモバイル版のプレビューを切り替え](/help/user-guide/create/manage-variants.md#preview-for-device)できます。

## コンテンツチェックの整合性の確認

生成されたバリエーションを最適化し、ブランドアイデンティティ、プラットフォームガイドライン、アクセシビリティ標準を厳密に遵守するには、[_コンテンツチェック_ パネル ](/help/user-guide/guidelines/brand-validation.md#content-check-panel)の機能を活用します。 このパネルには、包括的なコンテンツチェックの詳細が表示され、改善点が示されます。

**バリアントに対してコンテンツチェックを実行するには**:

1. 右側のアクションバーの&#x200B;_コンテンツチェック_ パネルアイコンをクリックして、[_コンテンツチェック_ パネル ](/help/user-guide/guidelines/brand-validation.md#content-check-panel)を開きます。 *Needs review*&#x200B;および&#x200B;*Passed*&#x200B;のチェックの概要を表示して、改善が必要なセクションとガイドラインを確認します。

   ![_コンテンツチェック_ パネル ](/help/assets/content-check-panel.png){width="300"}

2. [ バリエーションを手動で修正](#revise-generated-variants)して、バリエーションが実行されたコンテンツチェックと密接に連携していることを確認します。

[ ブランド検証](/help/user-guide/guidelines/brand-validation.md)を参照してください。

## レビューと承認を取得

カンバスの右側のアクションバーのアイコンとしてアクセスできる承認パネルを使用して、レビューの取得、レビューコメントの追跡、関係者からの承認の取得を行います。

**レビューと承認を取得するには**:

1. [承認要求](/help/user-guide/approvals/request-review.md)を開始して、ドラフトされたメールエクスペリエンスの[承認を依頼します](/help/user-guide/approvals/approve-content.md)。
1. レビュープロセス中に[ レビュー担当者](/help/user-guide/approvals/review-and-edit.md#manage-approvals)を削除または追加します。
1. [ レビュー用のコンテンツにアクセス ](/help/user-guide/approvals/review-and-edit.md#access-content-for-review)し、リビジョンのリクエストを表示します。
1. レビューのコメントごとにドラフトを編集し、[ メールエクスペリエンスを公開](#publish-and-export-experience)します。

詳しくは、[ レビューと承認](/help/user-guide/approvals/overview.md)を参照してください。

## エクスペリエンスの公開と書き出し

生成されたメールを現在および将来の使用に使用できるようにするには、それを[!UICONTROL  コンテンツ ]に公開し、マーケティングキャンペーンで使用するために書き出します。

1. **新しいメールエクスペリエンスを公開するには、上部のツールバーまたは承認フロー内の**[!UICONTROL &#x200B;公開&#x200B;]**をクリックします。**
1. **新しいメールエクスペリエンスを書き出すには**、上部のツールバーの「**[!UICONTROL 書き出し]**」をクリックします。
   1. 書式（CSVと画像またはHTMLのみ）を選択し、**[!UICONTROL 書き出し]**&#x200B;をクリックします。

詳しくは、[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content)を参照してください。
