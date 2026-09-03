---
title: LinkedIn エクスペリエンスの構築
description: Adobe GenStudio for Performance Marketingを利用して、ブランドに即したLinkedIn体験を構築する方法をご紹介します。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
badgeBeta: label="ベータ版" tooltip="この機能は、現在ベータ版なので、一部の機能が制限されるか、変更される場合があります。"
recommendations: noDisplay
exl-id: abe10fc8-d6d5-4cad-9273-400b622f22b7
TQID: https://experienceleague.adobe.com/6ydfKraxfvL6j24ImEAs-P5xV5dldGbQ7Kg8wMsWuOs
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2: id: be495d08-ecd1-455f-951e-c22de504e667id: de1f9646-abd3-4e21-9de2-df62ce55c8dcid: dee4e9a9-78d1-4953-8179-f8da6117027did: e3878dde-4b87-4290-9e81-ed7ee6eb83feid: f54ee13b-9545-4d68-9842-a12026e60aaf
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 1240
ht-degree: 1%

---

# LinkedIn エクスペリエンスの構築

このチュートリアルでは、GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) （左側のナビゲーション領域のペイントブラシアイコン）を使用して、ブランドガイドラインに準拠する[LinkedIn エクスペリエンス ](/help/user-guide/create/meta-experiences.md)を生成する方法を説明します。

LinkedIn広告の作成を開始する前に、[GenStudio for Performance Marketingでガイドライン ](/help/user-guide/guidelines/add-guidelines.md)を追加し、[ プロンプトの作成](/help/user-guide/effective-prompts.md)の基本を学ぶことが重要です。

## テンプレートの選択

新しいLinkedIn エクスペリエンスを生成するには、コンテンツのフレームワークを提供するテンプレートが必要です。 サポートされているLinkedInの縦横比について詳しくは、[LinkedIn テンプレートガイドライン ](/help/user-guide/templates/linkedin-template.md)を参照してください。

カスタムテンプレートのリストから選択するか、スターターテンプレートを選択できます。

**LinkedIn テンプレートを選択するには**:

1. _[!DNL Create]_で、**[!UICONTROL LinkedIn]**をクリックします。
1. アップロードしたテンプレートを参照するには&#x200B;**[!UICONTROL カスタムテンプレート]**&#x200B;を選択し、事前定義済みのテンプレートを参照するには&#x200B;**[!UICONTROL スターターテンプレート]**&#x200B;を選択します。

   Meta バリエーションにビデオアセットを追加する場合は、スターターテンプレートを選択する必要があります。 ビデオの使用を容易にする、システム定義のコンテンツ領域が事前に読み込まれています。

1. クリックしてテンプレートを選択し、**[!UICONTROL 使用]**&#x200B;をクリックします。

   このアクションにより、コンテンツ作成の中心的なハブであるカンバスが開きます。

## パラメーターを追加

プロンプトドロワーに[ ガイドライン ](/help/user-guide/guidelines/overview.md)と&#x200B;_パラメーター_&#x200B;のアセットを追加すると、コンテンツ生成プロセスが強化され、LinkedIn エクスペリエンスを生成する準備を行う上で非常に重要なステップです。

**パラメーターとアセットを追加するには**:

1. _パラメーター_ アイコンをクリックして、プロンプトドロワーを展開します。
1. 「_パラメーター_」セクションで、コンテンツ作成に役立つガイドライン（[!DNL Brands]、[!DNL Personas]、および[!DNL Products]）を選択します。

   ![ ペルソナの選択](/help/assets/persona-select-linkedin2.png){width="50%" align="center"}

   これらのメニューから利用できるブランド、ペルソナ、または製品がない場合は、[GenStudio for Performance Marketingにガイドラインを追加します](/help/user-guide/guidelines/add-guidelines.md)。

1. エクスペリエンス *および*&#x200B;で使用するコンテンツ（画像またはビデオ）を追加して、**[!UICONTROL コンテンツから選択]**&#x200B;をクリックしてコンテンツ生成に影響を与えます。 または、画像を&#x200B;**[!UICONTROL コンテンツから選択]** セクションにドラッグ&amp;ドロップして、1つ以上の新しいアセットをアップロードします。

   フィルターを使用してコンテンツを検索し、1つ以上の画像を選択します。

   ビデオ用のセクションを含むテンプレートを使用している場合、ビデオコンテンツ（.mp4）が事前に選択され、フィルタリングされます。 ビデオにカーソルを合わせると、自動再生プレビューが表示されます。

   ![ ビジュアルコンテンツの選択](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

   接続された[!DNL AEM Assets Content Hub] リポジトリからアセットを使用するには、_場所_ ドロップダウンメニューからリポジトリを選択します。 1つまたは複数の画像をフィルタリングして選択します。

1. 「**[!UICONTROL 使用]**」をクリックします。

パラメーターの追加が完了したら、_パラメーター_ アイコンをもう一度クリックして、プロンプトドロワーを折りたたむことができます。

## プロンプトを入力

ガイドラインを選択したら、自然言語を使用してプロンプトを作成し、新しいLinkedIn エクスペリエンスのコンテンツを生成します。 詳細なプロンプトを活用して、高品質で有益なコンテンツを生成できます。

プロンプトの作成について詳しくは、[効果的なプロンプトの作成](/help/user-guide/effective-prompts.md)を参照してください。

**プロンプトを入力するには**:

1. _「生成するエクスペリエンスについて説明する」プロンプト ボックスにプロンプトを入力します。_
1. 「**[!UICONTROL 生成]**」をクリックします。

   ビデオの生成方法と管理方法については、[ ビデオの管理](#manage-videos)を参照してください。

デフォルトでは、4つのバリエーション（プロンプト、ガイドライン、追加したコンテンツがすべてベース）が生成され、キャンバスに表示されます。

生成されたコンテンツは段階的に読み込まれます。LinkedIn エクスペリエンスの各セクションが生成されると、キャンバスに表示されます。 これらの変更がキャンバスにどのように読み込まれるかについては、[LinkedIn エクスペリエンス ](/help/user-guide/create/linkedin-experiences.md#progressive-loading)を参照してください。

## 生成されたLinkedIn広告を修正

承認または[!DNL Content]への公開のためにバリエーションを送信する前に、LinkedIn広告を編集するか、生成された広告セットからバリエーションを削除できます。

**生成されたバリエーションを修正するには**:

* **LinkedIn広告のドラフト名](/help/user-guide/create/manage-variants.md#change-draft-name)**&#x200B;を[編集するには、キャンバスの上部にある&#x200B;_名称未設定のドラフト_ タイトルをクリックし、新しいタイトルを入力します。
* **LinkedIn広告](/help/user-guide/create/manage-variants.md#manually-edit-text)**&#x200B;を手動で編集するには、任意の広告セクション（件名、ヘッダー、本文コピーなど）をクリックし、必要に応じて編集します。[
* **call to action**&#x200B;を変更または選択するには、「call-to-action」ボタンをクリックし、使用可能なボタンのテキストオプションから選択します。 _リンク_&#x200B;に、call-to-action テキストのURLを入力します。
* **バリエーションで[ テキストの書式設定](/help/user-guide/create/manage-variants.md#manually-edit-text)**&#x200B;を適用するには、バリエーションの画像テキストをクリックし、**[!UICONTROL テキストの書式設定]**&#x200B;をクリックします。
* **バリアント](/help/user-guide/create/manage-variants.md#re-generate-sections)**&#x200B;のセクションを[再生成するには、編集可能なテキストフィールドをクリックし、_[!UICONTROL おすすめの編集]_ オプションを使用するか、_[!UICONTROL 新しいテキストを生成_ セクション ]に新しいプロンプトを入力して、**[!UICONTROL 生成]**&#x200B;をクリックします。
* **生成拡張を使用して画像のサイズを変更し、画像を作業中のテンプレート**&#x200B;に合わせるには、画像をクリックし、**[!UICONTROL 編集]** （鉛筆アイコン）をクリックしてから&#x200B;**[!UICONTROL 拡張]**&#x200B;します。 [](/help/user-guide/create/manage-variants.md#use-generative-expand)必要なアスペクト比とテンプレートに合わせて画像を調整します。
* **画像の切り抜きまたは再配置](/help/user-guide/create/manage-variants.md#crop-assets)**&#x200B;を行うには、画像にカーソルを合わせて、表示される切り抜きアイコンをクリックし、画像のサイズと配置を調整します。[
* **広告](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**&#x200B;のサイズと縦横比を[変更するには、_[!UICONTROL サイズ変更]_ ボタン（キャンバスの左側にボタンアイコン付きのボックス）をクリックし、新しいサイズと縦横比を選択して、すべてのバリエーションに適用します。 バリエーションが重複し、サイズが変更されます。
* **バリアント](/help/user-guide/create/manage-variants.md#swap-image)**&#x200B;のアセット（画像またはビデオ）を[追加またはスワップするには、アセット（またはアセット領域）をクリックし、**[!UICONTROL コンテンツからスワップ]** アイコンをクリックします。
* **バリアント](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**&#x200B;の画像に代替テキストを[追加するには、画像アセットをクリックし、_代替テキスト_ オプションを使用して、画像ごとに代替テキストを手動で追加または生成します。
* **バリエーションに[ アクセシビリティラベル ](/help/user-guide/create/manage-variants.md#add-accessibility-labels)を追加するには**&#x200B;画像またはcall-to-action リンクをクリックし、リンクまたはボタンの機能を説明する簡単な説明を入力します。
* **LinkedIn広告](/help/user-guide/create/manage-variants.md#delete-variant)**&#x200B;を[削除するには、バリエーションのオプションメニューをクリックし、**[!UICONTROL バリエーションを削除]**&#x200B;をクリックします。

### ビデオの管理

各ビデオにカーソルを合わせると、ループされた自動再生が表示されます。

生成時に、選択した縦横比に合わせてビデオのフレームが変更されます。 「**[!UICONTROL リフレーム ビデオ]**」をクリックしてオフに切り替えることで、元のリフレームされていないビデオに戻すことができます。

## 生成フィードバックを送信

生成出力の品質に関するフィードバック ](/help/user-guide/create/manage-variants.md#generation-feedback)を[送信するには、オプションアイコン（3つのドット）をクリックし、**[!UICONTROL 良好な出力]**&#x200B;または&#x200B;**[!UICONTROL 不良な出力]**&#x200B;を選択します。

## コンテンツチェックの整合性の確認

生成されたバリエーションを最適化し、ブランドアイデンティティ、プラットフォームガイドライン、アクセシビリティ標準を厳密に遵守するには、[_コンテンツチェック_ パネル ](/help/user-guide/guidelines/brand-validation.md#content-check-panel)の機能を活用します。 このパネルには、包括的なコンテンツチェックの詳細が表示され、改善点が示されます。

**バリアントに対してコンテンツチェックを実行するには**:

1. 右側のアクションバーの&#x200B;_コンテンツチェック_ パネルアイコンをクリックして、[_コンテンツチェック_ パネル ](/help/user-guide/guidelines/brand-validation.md#content-check-panel)を開きます。 *Needs review*&#x200B;および&#x200B;*Passed*&#x200B;のチェックの概要を表示して、改善が必要なセクションとガイドラインを確認します。

   ![_コンテンツチェック_ パネル ](/help/assets/content-check-panel.png){width="300"}

2. [ バリエーションを手動で修正](#revise-generated-linkedin-ads)して、バリエーションが完了したコンテンツのチェックと密接に連携していることを確認します。

[ブランドの検証](/help/user-guide/guidelines/brand-validation.md)を参照してください。

## レビューと承認を取得

カンバスの上部メニューバーでアクセスできる承認パネルを使用して、レビューの取得、レビューコメントの追跡、関係者からの承認の取得を行います。

**レビューと承認を取得するには**:

1. [承認依頼](/help/user-guide/approvals/request-review.md)を開始して、ドラフトされたMeta広告エクスペリエンスの[承認を依頼します](/help/user-guide/approvals/approve-content.md)。

   ![ レビューと承認のために下書きを送信](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. レビュープロセス中に[ レビュー担当者](/help/user-guide/approvals/review-and-edit.md#manage-approvals)を削除または追加します。
1. [ レビュー用のコンテンツにアクセス ](/help/user-guide/approvals/review-and-edit.md#access-content-for-review)し、リビジョンのリクエストを表示します。
1. レビューのコメントごとにドラフトを編集し、[Meta広告エクスペリエンスを公開](#publish-and-export-experience)します。

詳しくは、[ レビューと承認](/help/user-guide/approvals/overview.md)を参照してください。

## エクスペリエンスの公開と書き出し

生成されたLinkedIn広告を現在および将来の使用に使用できるようにするには、[!UICONTROL  コンテンツ ]に公開し、マーケティングキャンペーンで使用するために書き出します。

1. **新しいエクスペリエンスを公開するには、上部のツールバーまたは承認フロー内の**[!UICONTROL &#x200B;公開&#x200B;]**をクリックします。**
1. **新しいエクスペリエンスを書き出すには**、上部のツールバーの&#x200B;**[!UICONTROL 書き出し]**&#x200B;をクリックします。
   1. 書式（JPG、PNG、またはGIF）を選択し、**[!UICONTROL 書き出し]**&#x200B;をクリックします。

詳しくは、[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content)を参照してください。
