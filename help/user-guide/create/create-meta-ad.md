---
title: Meta広告エクスペリエンスの構築
description: Adobe GenStudio for Performance Marketingを利用して、FacebookやInstagram向けに、ブランドに即したMeta広告エクスペリエンスを構築する方法をご紹介します。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 42111bbf-70cd-4fd2-a7a9-15abe072d720
TQID: https://experienceleague.adobe.com/ht5ZJBghEPMEL--WNyl5uam-Mb92dsgp-4g9jQ9aO-g
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
  - id: b03d2162-d906-40a0-9cbd-001391e22d4a
  - id: be495d08-ecd1-455f-951e-c22de504e667
  - id: de1f9646-abd3-4e21-9de2-df62ce55c8dc
  - id: dee4e9a9-78d1-4953-8179-f8da6117027d
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
  - id: ee4b6e5f-5b7a-421b-9859-0f964841a866
  - id: f54ee13b-9545-4d68-9842-a12026e60aaf
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 1414
ht-degree: 0%

---

# Meta広告エクスペリエンスの作成

このチュートリアルでは、GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) （左側のナビゲーション領域のペイントブラシアイコン）を使用して、ブランドの[Meta広告エクスペリエンス &#x200B;](/help/user-guide/create/meta-experiences.md)を生成する方法を説明します。

Meta広告エクスペリエンスの作成を開始する前に、[GenStudio for Performance Marketingにガイドライン &#x200B;](/help/user-guide/guidelines/add-guidelines.md)を組み込み、[&#x200B; プロンプトの作成の基本に慣れることが重要です](/help/user-guide/effective-prompts.md)。

## テンプレートの選択

新しいMeta広告エクスペリエンスの作成を開始するには、使用可能なテンプレートを使用して、コンテンツのフレームワークを提供します。 サポートされているMetaと縦横比について詳しくは、[Meta広告テンプレートガイドライン &#x200B;](/help/user-guide/templates/meta-template.md)を参照してください。

テンプレートを選択する際には、アップロードしたテンプレートまたはスターターテンプレートのいずれかを使用するオプションがあります。

**Meta広告テンプレートを選ぶには**:

1. _[!DNL Create]_&#x200B;で、**[!UICONTROL Meta ads]**&#x200B;をクリックします。
1. アップロードしたテンプレートを参照するには&#x200B;**[!UICONTROL カスタムテンプレート]**&#x200B;を選択し、事前定義済みのテンプレートを参照するには&#x200B;**[!UICONTROL スターターテンプレート]**&#x200B;を選択します。

   Meta バリエーションにビデオアセットを追加する場合は、スターターテンプレートを選択する必要があります。 ビデオの使用を容易にする、システム定義のコンテンツ領域が事前に読み込まれています。

1. クリックしてテンプレートを選択し、**[!UICONTROL 使用]**&#x200B;をクリックします。

   このアクションにより、コンテンツ作成の中心的なハブであるカンバスが開きます。

## パラメーターを追加

プロンプトドロワーに[&#x200B; ガイドライン &#x200B;](/help/user-guide/guidelines/overview.md)とアセットを&#x200B;_パラメーター_&#x200B;に追加すると、コンテンツ生成プロセスが強化され、Meta広告を生成する準備を行う上で非常に重要なステップとなります。

事前に定義されたガイドライン（[!DNL Brands]、[!DNL Personas]、[!DNL Products]など）を含むテンプレートを使用している場合、これらのガイドラインはバリエーションに適用されます。 必要に応じてそれらを変更できます。

**パラメーターとアセットを追加するには**:

1. _パラメーター_ アイコンをクリックして、プロンプトドロワーを展開します。
1. 「_パラメーター_」セクションで、コンテンツ作成に役立つガイドライン（[!DNL Brands]、[!DNL Personas]、および[!DNL Products]）を選択します。

   ![&#x200B; ペルソナの選択](/help/assets/persona-select-meta2.png){width="50%" align="center"}

   これらのメニューから利用できるブランド、ペルソナ、または製品がない場合は、[GenStudio for Performance Marketingにガイドラインを追加します](/help/user-guide/guidelines/add-guidelines.md)。

1. エクスペリエンス *および*&#x200B;で使用するコンテンツ（画像またはビデオ）を追加して、コンテンツ生成に影響を与えます。
   * 「**[!UICONTROL コンテンツから選択]**」をクリックして、[!DNL Content] リポジトリからアセットを選択し、フィルターを適用して1つ以上の画像を選択します。

     ビデオ用のセクションを含むテンプレートを使用している場合、ビデオコンテンツ（.mp4）が事前に選択され、フィルタリングされます。 ビデオにカーソルを合わせると、自動再生プレビューが表示されます。

     ![&#x200B; ビジュアルコンテンツの選択](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

     接続された[!DNL AEM Assets Content Hub] リポジトリからアセットを使用するには、_場所_ ドロップダウンメニューからリポジトリを選択します。 1つまたは複数の画像をフィルタリングして選択します。

   * または、画像を&#x200B;**[!UICONTROL コンテンツから選択]** セクションにドラッグ&amp;ドロップして、1つ以上の新しいアセットをアップロードします。

1. 「**[!UICONTROL 使用]**」をクリックします。

パラメーターの追加が完了したら、_パラメーター_ アイコンをもう一度クリックして、プロンプトドロワーを折りたたむことができます。

## プロンプトを入力

ガイドラインを選択したら、自然言語を使用してプロンプトを作成し、新しいMeta広告エクスペリエンスのコンテンツを生成します。 詳細なプロンプトは、曖昧なプロンプトよりも高品質です。

プロンプトの作成について詳しくは、[効果的なプロンプトの作成](/help/user-guide/effective-prompts.md)を参照してください。

**プロンプトを入力するには**:

1. _「生成するエクスペリエンスについて説明する」プロンプト ボックスにプロンプトを入力します。_
1. 「**[!UICONTROL 生成]**」をクリックします。

   ビデオの生成方法と管理方法については、[&#x200B; ビデオの管理](#manage-videos)を参照してください。

デフォルトでは、4つのバリエーション（プロンプト、ガイドライン、追加したコンテンツがすべてベース）が生成され、キャンバスに表示されます。

生成されたコンテンツは、Meta エクスペリエンスの各セクションが生成されると、カンバスに表示されるので、プログレッシブに読み込まれます。 これらの変更がCanvasでどのように読み込まれるかについては、[Meta エクスペリエンス &#x200B;](/help/user-guide/create/meta-experiences.md#progressive-loading)を参照してください。

## Meta広告チャネルを選択

Meta広告を生成する際には、Facebook広告とInstagram広告のどちらかを選ぶことができます。

右側のメニューバー（FacebookおよびInstagramのアイコン）で、**Facebook**&#x200B;と&#x200B;**Instagram**&#x200B;の間のMeta広告チャネルオプションを切り替えて、各チャネルのバリエーションを表示および管理します。

[Meta広告を修正する](#revise-generated-variants)場合、Facebook広告とInstagram広告の縦横比を変更できます。

## 生成したバリエーションを修正

[!DNL Content]への承認または公開のために送信するものを選択する前に、Meta広告を編集するか、生成された広告セットからバリエーションを削除できます。

修正する個々のレイヤーをハイライト表示するには、編集可能なフィールドまたは画像をクリックし、_[!UICONTROL レイヤーを表示]_&#x200B;をクリックします。

**生成されたバリエーションを修正するには**:

* **Meta広告のドラフト名[&#128279;](/help/user-guide/create/manage-variants.md#change-draft-name)**&#x200B;を編集するには、キャンバスの上部にある&#x200B;_名称未設定のドラフト_ タイトルをクリックし、新しいタイトルを入力します。
* **Meta広告[&#128279;](/help/user-guide/create/manage-variants.md#manually-edit-text)**&#x200B;を手動で編集するには、任意の広告セクション（「件名」など）をクリックします。
ヘッダー、または本文コピー）を編集し、必要に応じて編集します。
* **call to action**&#x200B;を変更または選択するには、「call-to-action」ボタンをクリックし、使用可能なボタンのテキストオプションから選択します。 _リンク_&#x200B;に、call-to-action テキストのURLを入力します。
* **バリエーションで[&#x200B; テキストの書式設定](/help/user-guide/create/manage-variants.md#manually-edit-text)**&#x200B;を適用するには、バリエーションの画像テキストまたはインラインリンクをクリックし、**[!UICONTROL テキストの書式設定]**&#x200B;をクリックします。
<!-- **To [change or select the Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**, click the call-to-action button and select _[!UICONTROL Rephrase]_ or _[!UICONTROL Add link]_. -->
* **バリアント[&#128279;](/help/user-guide/create/manage-variants.md#add-image-link)**&#x200B;の画像にリンクを追加するには、画像アセット（または画像が現在存在しない場合は画像アセット領域）をクリックし、リンクアイコンをクリックします。
* **広告[&#128279;](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**&#x200B;のサイズと縦横比を変更するには、_[!UICONTROL サイズ変更]_ ボタン（キャンバスの左側にボタンアイコン付きのボックス）をクリックし、新しいサイズと縦横比を選択して、すべてのバリエーションに適用します。 バリエーションが重複し、サイズが変更されます。
* **バリアント[&#128279;](/help/user-guide/create/manage-variants.md#re-generate-sections)**&#x200B;のセクションを再生成するには、編集可能なテキストフィールドをクリックして&#x200B;_[!UICONTROL おすすめ編集]_ オプションを使用するか、新しいプロンプトを入力して&#x200B;**[!UICONTROL 生成]**&#x200B;をクリックします。
* **バリアントの画像を[追加または入れ替えるには、](/help/user-guide/create/manage-variants.md#swap-image)**&#x200B;画像アセット （または画像が現在存在しない場合は画像アセット領域）をクリックし、**[!UICONTROL コンテンツから入れ替え]** アイコンをクリックします。
* **画像を[切り抜きまたは再配置](/help/user-guide/create/manage-variants.md#crop-assets)**&#x200B;するには、画像をクリックし、**[!UICONTROL 編集]** （鉛筆アイコン）をクリックしてから&#x200B;**[!UICONTROL 切り抜き]**&#x200B;をクリックします。 画像のサイズと配置を調整します。
* **生成拡張を使用して画像のサイズを変更し、画像を作業中のテンプレート**&#x200B;に合わせるには、画像をクリックし、**[!UICONTROL 編集]** （鉛筆アイコン）をクリックしてから&#x200B;**[!UICONTROL 拡張]**&#x200B;します。 [&#128279;](/help/user-guide/create/manage-variants.md#use-generative-expand)必要なアスペクト比とテンプレートに合わせて画像を調整します。
* **バリアント[&#128279;](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**&#x200B;の画像に代替テキストを追加するには、画像アセットをクリックし、_代替テキスト_ オプションを使用して、画像ごとに代替テキストを手動で追加または生成します。
* **バリエーションに[&#x200B; アクセシビリティラベル &#x200B;](/help/user-guide/create/manage-variants.md#add-accessibility-labels)を追加するには**&#x200B;画像またはcall-to-action リンクをクリックし、リンクまたはボタンの機能を説明する簡単な説明を入力します。
* **Meta広告[&#128279;](/help/user-guide/create/manage-variants.md#delete-variant)**&#x200B;を削除するには、バリエーションのオプションメニューをクリックし、**[!UICONTROL バリエーションを削除]**&#x200B;をクリックします。

### ビデオの管理

各ビデオにカーソルを合わせると、ループされた自動再生が表示されます。

生成時に、選択した縦横比に合わせてビデオのフレームが変更されます。 「**[!UICONTROL リフレーム ビデオ]**」をクリックしてオフに切り替えることで、元のリフレームされていないビデオに戻すことができます。

## 生成フィードバックを送信

生成出力の品質に関するフィードバック [&#128279;](/help/user-guide/create/manage-variants.md#generation-feedback)を送信するには、オプションアイコン（3つのドット）をクリックし、**[!UICONTROL 良好な出力]**&#x200B;または&#x200B;**[!UICONTROL 不良な出力]**&#x200B;を選択します。

## コンテンツチェックの整合性の確認

生成されたバリエーションを最適化し、ブランドアイデンティティ、プラットフォームガイドライン、アクセシビリティ標準を厳密に遵守するには、[_コンテンツチェック_ パネル &#x200B;](/help/user-guide/guidelines/brand-validation.md#content-check-panel)の機能を活用します。 このパネルには、包括的なコンテンツチェックの詳細が表示され、改善点が示されます。

**バリアントに対してコンテンツチェックを実行するには**:

1. 右側のアクションバーの&#x200B;_コンテンツチェック_ パネルアイコンをクリックして、[_コンテンツチェック_ パネル &#x200B;](/help/user-guide/guidelines/brand-validation.md#content-check-panel)を開きます。 *Needs review*&#x200B;および&#x200B;*Passed*&#x200B;のチェックの概要を表示して、改善が必要なセクションとガイドラインを確認します。

   ![_コンテンツチェック_ パネル &#x200B;](/help/assets/content-check-panel.png){width="300"}

2. [&#x200B; バリエーションを手動で修正](#revise-generated-variants)して、バリエーションが実行されたコンテンツチェックと密接に連携していることを確認します。

[ブランドの検証](/help/user-guide/guidelines/brand-validation.md)を参照してください。

## レビューと承認を取得

カンバスの右側のアクションバーのアイコンとしてアクセスできる承認パネルを使用して、レビューの取得、レビューコメントの追跡、関係者からの承認の取得を行います。

**レビューと承認を取得するには**:

1. [承認依頼](/help/user-guide/approvals/request-review.md)を開始して、ドラフトされたMeta広告エクスペリエンスの[承認を依頼します](/help/user-guide/approvals/approve-content.md)。

   ![&#x200B; レビューと承認のために下書きを送信](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. レビュープロセス中に[&#x200B; レビュー担当者](/help/user-guide/approvals/review-and-edit.md#manage-approvals)を削除または追加します。
1. [&#x200B; レビュー用のコンテンツにアクセス &#x200B;](/help/user-guide/approvals/review-and-edit.md#access-content-for-review)し、リビジョンのリクエストを表示します。
1. レビューのコメントごとにドラフトを編集し、[Meta広告エクスペリエンスを公開](#publish-and-export-experience)します。

詳しくは、[&#x200B; レビューと承認](/help/user-guide/approvals/overview.md)を参照してください。

## エクスペリエンスの公開と書き出し

生成されたMeta広告を現在および将来の使用に使用できるようにするには、それを[!UICONTROL &#x200B; コンテンツ &#x200B;]に公開し、マーケティングキャンペーンで使用するために書き出します。

1. **新しいMeta広告エクスペリエンスを公開するには、上部のツールバーまたは承認フロー内の**&#x200B;[!UICONTROL &#x200B;公開&#x200B;]&#x200B;**をクリックします。**
1. **新しいMeta広告エクスペリエンスを書き出すには、上部のツールバーの「**&#x200B;[!UICONTROL &#x200B;書き出し&#x200B;]&#x200B;**」をクリックします。**
   1. 書式（HTMLと画像またはCSVと画像（JPGまたはPNG））を選択し、**[!UICONTROL 書き出し]**&#x200B;をクリックします。

詳しくは、[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content)を参照してください。

## Metaとの連携

GenStudio for Performance MarketingとMetaを連携させることで、コンテンツのパフォーマンスに関する高度な分析とインサイトを獲得できます。

[Meta ads connect](/help/user-guide/connectors/meta-ads.md)を参照してください。
