---
title: Meta Ad Experience の作成
description: Adobe GenStudio for Performance Marketingを使用して、Facebook や Instagram 向けのブランド上のMeta広告エクスペリエンスを作成する方法を説明します。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 42111bbf-70cd-4fd2-a7a9-15abe072d720
source-git-commit: d3ddbefc47d3289041783a1a277aa2e855d13ccb
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 0%

---

# Meta広告エクスペリエンスの作成

このチュートリアルでは、GenStudio for Performance Marketing [&#x200B; （左側のナビゲーションエリアにある絵筆のアイコン）を使用して &#x200B;](/help/user-guide/create/meta-experiences.md) ブランド化された [[!DNL Create]](/help/user-guide/create/overview.md)Meta広告エクスペリエンスを生成する方法を実演します。

Meta広告エクスペリエンスの作成を開始する前に、GenStudio for Performance Marketingで [&#x200B; ガイドラインを組み込む &#x200B;](/help/user-guide/guidelines/add-guidelines.md) ことと、[&#x200B; プロンプトの作成 &#x200B;](/help/user-guide/effective-prompts.md) の基本を理解することが重要です。

## テンプレートを選択

新しいMeta広告エクスペリエンスの生成を開始するには、使用可能なテンプレートを使用してコンテンツのフレームワークを提供します。 サポートされるMetaの広告アスペクト比について詳しくは [&#128279;](/help/user-guide/templates/meta-template.md)Meta広告テンプレートガイドライン &rbrace; を参照してください。

テンプレートを選択する際は、アップロードしたテンプレートの 1 つを使用するか、スターターテンプレートを使用するかを選択できます。

**Meta広告テンプレートを選択するには**:

1. _[!DNL Create]_&#x200B;で、**[!UICONTROL Meta広告]**&#x200B;をクリックします。
1. **[!UICONTROL カスタムテンプレート]** を選択してアップロードしたテンプレートまたは **[!UICONTROL スターターテンプレート]** を選択して、事前定義済みのテンプレートを参照します。

   Metaのバリエーションにビデオアセットを追加する場合は、スターターテンプレートを選択する必要があります。 ビデオの使用を容易にするシステム定義のコンテンツ領域が事前に読み込まれています。

1. テンプレートをクリックして選択し、「**[!UICONTROL 使用]**」をクリックします。

   これにより、コンテンツ作成の中心となるキャンバスが開きます。

## パラメーターを追加

プロンプトドロワーに [&#x200B; ガイドライン &#x200B;](/help/user-guide/guidelines/overview.md) とアセットを _パラメーター_ に追加すると、コンテンツ作成プロセスが強化されます。これは、Meta広告を作成する準備をする際に重要な手順です。

事前定義済みのガイドライン（[!DNL Brands]、[!DNL Personas]、[!DNL Products] など）を含んだテンプレートを使用している場合、これらのガイドラインはバリアントに適用されます。 必要に応じて変更できます。

**パラメーターとアセットを追加するには**:

1. _パラメーター_ アイコンをクリックして、プロンプトドロワーを展開します。
1. 「_パラメーター_」セクションで、ガイドライン（[!DNL Brands]、[!DNL Personas]、[!DNL Products]）を選択して、コンテンツの作成を通知します。

   ![&#x200B; ペルソナを選択 &#x200B;](/help/assets/persona-select-meta.png){width="300" align="center" zoomable="yes"}

   これらのメニューから利用できるブランド、ペルソナ、製品がない場合は、[GenStudio for Performance Marketingにガイドラインを追加 &#x200B;](/help/user-guide/guidelines/add-guidelines.md) します。

1. エクスペリエンス（および *で使用するコンテンツ（画像やビデオ）を追加して* コンテンツの生成に影響を与えます。
   * **[!UICONTROL コンテンツから選択]** をクリックして、[!DNL Content] リポジトリからアセットを選択し、1 つ以上の画像をフィルタリングして選択します。

     ビデオのセクションがあるテンプレートを使用している場合は、ビデオコンテンツ（.mp4）が事前選択され、フィルタリングされます。 ビデオの上にマウスポインターを置くと、自動再生されたプレビューが表示されます。

     ![&#x200B; ビジュアルコンテンツを選択 &#x200B;](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

     接続された [!DNL AEM Assets Content Hub] リポジトリのアセットを使用するには、_場所_ ドロップダウンメニューからリポジトリを選択します。 1 つ以上の画像のフィルタリングと選択

   * または、画像を「**[!UICONTROL コンテンツから選択]**」セクションにドラッグ&amp;ドロップして、1 つ以上の新しいアセットをアップロードします。

1. **[!UICONTROL 使用]** をクリックします。

パラメーターの追加が完了したら、「_パラメーター_」アイコンをもう一度クリックすると、プロンプトドロワーを折りたたむことができます。

## プロンプトを入力

ガイドラインを選択したら、自然言語を使用してプロンプトを作成し、新しいMeta広告エクスペリエンス用のコンテンツの生成を開始します。 詳細なプロンプトは、あいまいなプロンプトやあいまいなプロンプトよりも高品質の出力を生成します。

プロンプトの書き込みについて詳しくは、[&#x200B; 効果的なプロンプトの書き込み &#x200B;](/help/user-guide/effective-prompts.md) を参照してください。

**プロンプトを入力するには**:

1. _生成するエクスペリエンスを記述」_ プロンプトボックスにプロンプトを入力します。
1. 「**[!UICONTROL 生成]**」をクリックします。

   ビデオの生成方法と管理方法について詳しくは、[&#x200B; ビデオの管理 &#x200B;](#manage-videos) を参照してください。

デフォルトでは、4 つのバリエーション（追加したプロンプト、ガイドラインおよびコンテンツによってすべて強化される）が生成され、キャンバスに表示されます。

生成されたコンテンツは徐々に読み込まれます。Meta エクスペリエンスの各セクションが生成されると、キャンバスに表示されます。 これらの変更内容がキャンバスに読み込まれる方法については、[Meta エクスペリエンス &#x200B;](/help/user-guide/create/meta-experiences.md#progressive-loading) を参照してください。

## Meta広告チャネルを選択

Meta広告を作成する際は、Facebook または Instagram の広告から選択できます。

右側のメニューバー（Facebook および Instagram アイコン **でMeta広告チャネルオプションを** Facebook **と** Instagram）の間で切り替えて、各チャネルのバリアントを表示および管理します。

[Meta広告の見直し &#x200B;](#revise-generated-variants) を行う際には、Facebook や Instagram の広告のアスペクト比を変えることができます。

## 生成されたバリアントを修正

承認または公開の対象を選択する前に [!DNL Content]Meta広告を編集するか、生成された広告のセットからバリアントを削除できます。

変更する個々のレイヤーをハイライト表示するには、編集可能なフィールドまたは画像をクリックし、「_[!UICONTROL レイヤーを表示]_」をクリックします。

**生成されたバリアントを修正するには**:

* **Metaとドラフトの名前を [&#x200B; 編集](/help/user-guide/create/manage-variants.md#change-draft-name)** するには、キャンバス上部の _名称未設定のドラフト_ タイトルをクリックし、新しいタイトルを入力します。
* **Meta広告を [&#x200B; 手動で編集](/help/user-guide/create/manage-variants.md#manually-edit-text)** するには、広告セクションのいずれか（件名など）をクリックします。
ヘッダー（本文コピー）を使用し、必要に応じて編集します。
* **call to actionを変更または選択するには** 「call-to-action」ボタンをクリックし、使用可能なボタンテキストオプションから選択します。 _リンク_ に、call-to-actionテキストの URL を入力します。
* **バリアントで [&#x200B; テキストの書式設定を適用](/help/user-guide/create/manage-variants.md#manually-edit-text)** するには、バリアントの画像上のテキストまたはインラインリンクをクリックし、「**[!UICONTROL テキストの書式設定]**」をクリックします。
<!-- **To [change or select the Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**, click the call-to-action button and select _[!UICONTROL Rephrase]_ or _[!UICONTROL Add link]_. -->
* **バリアント内の画像へのリンクを追加 [&#x200B; するには](/help/user-guide/create/manage-variants.md#add-image-link)**、画像アセット（画像が現在存在しない場合は画像アセット領域）をクリックし、リンクアイコンをクリックします。
* **広告のサイズと縦横比を [&#x200B; 変更](/help/user-guide/create/manage-variants.md#change-aspect-ratio)** するには、_[!UICONTROL サイズ変更]_ ボタン（キャンバスの左側にボタンアイコンが表示されたボックス）をクリックし、すべてのバリアントに適用する新しいサイズと縦横比を選択します。 バリアントが複製され、サイズが変更されます。
* **バリアントのセクションを [&#x200B; 再生成](/help/user-guide/create/manage-variants.md#re-generate-sections)** するには、編集可能なテキストフィールドをクリックして _[!UICONTROL 編集候補]_ オプションを使用するか、新しいプロンプトを入力して **[!UICONTROL 生成]** をクリックします。
* **バリアント内の画像を追加 [&#x200B; 入れ替え](/help/user-guide/create/manage-variants.md#swap-image)** するには、画像アセット（画像が現在存在しない場合は画像アセット領域）をクリックし、**[!UICONTROL コンテンツから入れ替え]** アイコンをクリックします。
* **画像を [&#x200B; 切り抜きまたは再配置](/help/user-guide/create/manage-variants.md#crop-assets)** するには、画像をクリックし、**[!UICONTROL 編集]** （鉛筆アイコン）をクリックしてから **[!UICONTROL 切り抜き]** をクリックします。 画像のサイズと配置を調整します。
* **画像のサイズを調整およびフィットするために生成拡張を使用 [&#x200B; するには &#x200B;](/help/user-guide/create/manage-variants.md#use-generative-expand) 作業テンプレートに合わせます**、画像をクリックし、**[!UICONTROL 編集]** （鉛筆アイコン）をクリックしてから **[!UICONTROL 展開]** をクリックします。 必要な縦横比とテンプレートに合わせて画像を調整します。
* **バリアント内の画像の代替テキストを追加 [&#x200B; するには](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**、画像アセットをクリックし、「_代替テキスト_」オプションを使用して、画像ごとに代替テキストを手動で追加または生成します。
* **バリアントに [&#x200B; アクセシビリティラベルを追加 &#x200B;](/help/user-guide/create/manage-variants.md#add-accessibility-labels) するには** 画像またはcall-to-action リンクをクリックし、リンクまたはボタンの機能を説明する簡単な説明を入力します。
* **Meta広告を [&#x200B; 削除](/help/user-guide/create/manage-variants.md#delete-variant)** するには、バリアントのオプションメニューをクリックし、**[!UICONTROL バリアントを削除]** をクリックします。

### ビデオを管理

各ビデオにポインタを合わせると、ループ再生された自動再生が表示されます。

ビデオは、生成時に選択した縦横比に合わせて変更されます。 **[!UICONTROL ビデオを再フレーム]** をクリックしてオフに切り替えて、元の屈折されていないビデオに戻します。

## 生成フィードバックを送信

生成出力の品質に関する [&#x200B; フィードバックを送信 &#x200B;](/help/user-guide/create/manage-variants.md#generation-feedback) するには、オプションアイコン（3 つのドット）をクリックし、**[!UICONTROL 良好な出力]** または **[!UICONTROL 不良な出力]** を選択します。

## コンテンツチェックの整合性の確認

生成されたバリアントを最適化し、ブランド ID、プラットフォームガイドラインおよびアクセシビリティ標準に厳密に準拠するには、[_コンテンツチェック_ パネル &#x200B;](/help/user-guide/guidelines/brand-validation.md#content-check-panel) の機能を活用します。 このパネルには、包括的なコンテンツチェックの詳細が表示され、改善点が明らかになります。

**バリアントに対してコンテンツチェックを実行するには**:

1. 右側のアクションバーにある _コンテンツチェック_ パネルアイコンをクリックして、[_コンテンツチェック_ パネル &#x200B;](/help/user-guide/guidelines/brand-validation.md#content-check-panel) を開きます。 *レビューが必要* チェックと *合格* チェックの概要を表示し、改善が必要なセクションとガイドラインを確認します。

   ![_コンテンツチェック_ パネル &#x200B;](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [&#x200B; バリアントを手動で改訂 &#x200B;](#revise-generated-variants) し、バリアントが実行されたコンテンツチェックと密接に連携していることを確認します。

[&#x200B; ブランド検証 &#x200B;](/help/user-guide/guidelines/brand-validation.md) を参照してください。

## レビューと承認の取得

承認パネルは、キャンバスの右側のアクションバーにあるアイコンとしてアクセスでき、レビューを取得したり、レビューのコメントを追跡したり、関係者から承認を得たりできます。

**レビューと承認を取得するには**:

1. [Meta広告エクスペリエンスのドラフトの承認 &#x200B;](/help/user-guide/approvals/request-review.md) を依頼する [&#x200B; 承認リクエストの開始 &#x200B;](/help/user-guide/approvals/approve-content.md)。

   ![&#x200B; レビューおよび承認用のドラフトの送信 &#x200B;](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. レビュープロセス中に [&#x200B; レビュー担当者を削除または追加 &#x200B;](/help/user-guide/approvals/review-and-edit.md#manage-approvals) できます。
1. [&#x200B; レビュー用にコンテンツにアクセス &#x200B;](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) し、修正要求を表示します。
1. レビューコメントごとにドラフトを編集し、[Meta広告エクスペリエンスを公開する &#x200B;](#publish-and-export-experience) ようにします。

詳しくは、[&#x200B; レビューと承認 &#x200B;](/help/user-guide/approvals/overview.md) を参照してください。

## エクスペリエンスの公開と書き出し

生成したMeta広告を現在および将来の使用で使用できるようにするには、[!UICONTROL &#x200B; コンテンツ &#x200B;] に公開し、マーケティングキャンペーンで使用するためにエクスポートします。

1. **新しいMeta広告エクスペリエンスを公開するには** 上部のツールバーまたは承認フロー内の **[!UICONTROL 公開]** をクリックします。
1. **新しいMeta広告エクスペリエンスを書き出すには** 上部のツールバーにある **[!UICONTROL 書き出し]** をクリックします。
   1. 「HTMLと画像」または「CSV と画像（JPGまたは PNG）」のフォーマットを選択し、「**[!UICONTROL 書き出し]**」をクリックします。

詳細は、[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) を参照してください。

## Metaを接続

GenStudio for Performance MarketingをMetaに接続すると、コンテンツのパフォーマンスに関する高度な分析やインサイトを受け取ることができます。

[Meta広告の連携 &#x200B;](/help/user-guide/connectors/meta-ads.md) を参照してください。
