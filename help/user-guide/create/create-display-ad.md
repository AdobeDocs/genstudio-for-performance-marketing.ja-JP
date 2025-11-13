---
title: ディスプレイ広告エクスペリエンスの作成
description: パフォーマンスマーケティング用にAdobeでディスプレイ広告エクスペリエンス  [!DNL GenStudio]  作成する方法を説明します。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 7d5e777b-7a30-48f4-b253-9823e38eecce
source-git-commit: 4658a759f5a4e03c54f645cfa1d1bbcc84fe1d91
workflow-type: tm+mt
source-wordcount: '1132'
ht-degree: 0%

---

# ディスプレイとエクスペリエンスの作成

このチュートリアルでは、GenStudio for Performance Marketing [&#x200B; （左側のナビゲーションエリアにある絵筆のアイコン &#x200B;](display-ad-experiences.md) を使用してブランド化 [[!DNL Create]](/help/user-guide/create/overview.md) ディスプレイ広告エクスペリエンス）を生成する方法を説明します。

魅力的なディスプレイ広告体験をデザインするには、開始する前に [GenStudio for Performance Marketingにガイドラインを追加 &#x200B;](/help/user-guide/guidelines/add-guidelines.md)、「プロンプトの記述の基本 [&#x200B; を確認するこ &#x200B;](/help/user-guide/effective-prompts.md) をお勧めします。

## テンプレートを選択

ディスプレイとエクスペリエンスを作成するには、使用可能なテンプレートを使用してコンテンツのフレームワークを提供します。 サポートされるディスプレイ広告ディメンションについて詳しくは、[&#x200B; ディスプレイ広告テンプレートガイドライン &#x200B;](/help/user-guide/templates/display-template.md) を参照してください。

**ディスプレイ広告テンプレートを選択するには**:

1. _[!DNL Create]_&#x200B;で、**[!UICONTROL 広告を表示]**&#x200B;をクリックします。
1. _フィルター_ の横にある検索オプションを使用して、特定のディスプレイ広告テンプレートを見つけます。
1. _テンプレートを選択_ ビューで、ディスプレイ広告テンプレートをクリックします。
1. **[!UICONTROL 使用]** をクリックします。

   コンテンツ作成の中央ハブとして機能するキャンバスが表示されます。

## パラメーターを追加

プロンプトドロワーの [&#x200B; パラメーター &#x200B;](/help/user-guide/guidelines/overview.md) に _ガイドライン_ とアセットを追加することは、コンテンツ生成プロセスをスーパーチャージし、ディスプレイ広告エクスペリエンスを生成するための不可欠な準備手順です。

事前定義済みのガイドライン（[!DNL Brands]、[!DNL Personas]、[!DNL Products] など）を含んだテンプレートを使用している場合、これらのガイドラインはバリアントに適用されます。 必要に応じて変更できます。

**パラメーターとアセットを追加するには**:

1. _パラメーター_ アイコンをクリックして、プロンプトドロワーを展開します。
1. 「_パラメーター_」セクションで、ガイドライン（[!DNL Brands]、[!DNL Personas]、[!DNL Products]）を選択して、コンテンツの作成を通知します。

   これらのメニューから利用できるブランド、ペルソナ、製品がない場合は、[GenStudio for Performance Marketingにガイドラインを追加 &#x200B;](/help/user-guide/guidelines/add-guidelines.md) します。

1. エクスペリエンス *および* で使用するコンテンツを追加して、コンテンツの生成に影響を与えるには、次のようにします。
   * **[!UICONTROL コンテンツから選択]** をクリックして、[!DNL Content] リポジトリからアセット（画像）を選択し、1 つ以上の画像をフィルタリングして選択します。

     接続された [!DNL AEM Assets Content Hub] リポジトリのアセットを使用するには、_場所_ ドロップダウンメニューからリポジトリを選択します。 1 つ以上の画像のフィルタリングと選択

   * または、アセットを「**[!UICONTROL コンテンツから選択]** セクションにドラッグ&amp;ドロップして、1 つ以上の新しいアセットをアップロードします。
1. **[!UICONTROL 使用]** をクリックします。

パラメーターの追加が完了したら、「_パラメーター_ アイコンをもう一度クリックして、プロンプトドロワーを折りたたみます。

## プロンプトを入力

ガイドラインを選択したら、自然言語を使用してプロンプトを作成し、新しいディスプレイとエクスペリエンスのコンテンツの生成を開始します。 生成されるディスプレイとエクスペリエンスの品質を高めるには、詳細で説明的なプロンプトを作成することが重要です。

![&#x200B; プロンプトを入力 &#x200B;](/help/assets/prompt-displayad.png){width="650" zoomable="yes"}

プロンプトの書き込みについて詳しくは、[&#x200B; 効果的なプロンプトの書き込み &#x200B;](/help/user-guide/effective-prompts.md) を参照してください。

**プロンプトを入力するには**:

1. _生成するエクスペリエンスを記述」_ プロンプトボックスにプロンプトを入力します。
1. 「**[!UICONTROL 生成]**」をクリックします。

デフォルトでは、4 つのバリエーション（追加したプロンプト、ガイドラインおよびコンテンツに基づく）が生成され、キャンバスに表示されます。

## 生成されたバリアントを修正

に承認または公開するために送信する内容を選択する前に [!DNL Content] ディスプレイ広告セクションとテキストフィールドを編集したり、生成されたバリアントを削除したりできます。

変更する個々のレイヤーをハイライト表示するには、編集可能なフィールドまたは画像をクリックし、「_[!UICONTROL レイヤーを表示]_」をクリックします。

**生成されたバリアントを修正するには**:

* **ディスプレイとドラフトの名前を [&#x200B; 編集](/help/user-guide/create/manage-variants.md#change-draft-name)** するには、キャンバスの上部にある _名称未設定のドラフト_ タイトルをクリックし、新しいタイトルを入力します。
* **ディスプレイ広告を [&#x200B; 手動で編集](/help/user-guide/create/manage-variants.md#manually-edit-text)** するには、ディスプレイ広告の任意のセクションまたはフィールド（件名行、ヘッダー、本文コピーなど）をダブルクリックし、必要に応じて編集します。
* **バリアントで [&#x200B; テキストの書式設定を適用](/help/user-guide/create/manage-variants.md#manually-edit-text)** するには、バリアントの画像上のテキストまたはインラインリンクをクリックし、「**[!UICONTROL テキストの書式設定]**」をクリックします。
* **バリアントのセクションを [&#x200B; 再生成](/help/user-guide/create/manage-variants.md#re-generate-sections)** するには、編集可能なテキストフィールドをクリックして _[!UICONTROL 編集候補]_ オプションを使用するか、_[!UICONTROL Generate new text_ セクションに新しいプロンプトを入力して &#x200B;]&#x200B;**[!UICONTROL Generate]** をクリックします。
* **バリアント内の画像を追加 [&#x200B; 入れ替え](/help/user-guide/create/manage-variants.md#swap-image)** するには、画像アセット（画像が現在存在しない場合は画像アセット領域）をクリックし、**[!UICONTROL コンテンツから入れ替え]** アイコンをクリックします。
* **バリアント内の画像へのリンクを追加 [&#x200B; するには](/help/user-guide/create/manage-variants.md#add-image-link)**、画像アセット（画像が現在存在しない場合は画像アセット領域）をクリックし、リンクアイコンをクリックします。
* **バリアント内の画像の代替テキストを追加 [&#x200B; するには](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**、画像アセットをクリックし、「_代替テキスト_」オプションを使用して、画像ごとに代替テキストを手動で追加または生成します。
* **バリアントに [&#x200B; アクセシビリティラベルを追加 &#x200B;](/help/user-guide/create/manage-variants.md#add-accessibility-labels) するには** 画像またはcall-to-action リンクをクリックし、リンクまたはボタンの機能を説明する簡単な説明を入力します。
* **広告のサイズと縦横比を [&#x200B; 変更](/help/user-guide/create/manage-variants.md#change-aspect-ratio)** するには、_[!UICONTROL サイズ変更]_ ボタン（キャンバスの左側にボタンアイコンが表示されたボックス）をクリックし、すべてのバリアントに適用する新しいサイズと縦横比を選択します。 バリアントが複製され、サイズが変更されます。
* **画像を [&#x200B; 切り抜きまたは再配置](/help/user-guide/create/manage-variants.md#crop-assets)** するには、画像をクリックし、**[!UICONTROL 編集]** （鉛筆アイコン）をクリックしてから **[!UICONTROL 切り抜き]** をクリックします。 画像のサイズと配置を調整します。
* **画像のサイズを調整およびフィットするために生成拡張を使用 [&#x200B; するには &#x200B;](/help/user-guide/create/manage-variants.md#use-generative-expand) 作業テンプレートに合わせます**、画像をクリックし、**[!UICONTROL 編集]** （鉛筆アイコン）をクリックしてから **[!UICONTROL 展開]** をクリックします。 必要な縦横比とテンプレートに合わせて画像を調整します。

<!-- # Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

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

1. [&#x200B; ドラフトのディスプレイ広告エクスペリエンスの承認 &#x200B;](/help/user-guide/approvals/request-review.md) を依頼する [&#x200B; 承認リクエストの開始 &#x200B;](/help/user-guide/approvals/approve-content.md)。
1. レビュープロセス中に [&#x200B; レビュー担当者を削除または追加 &#x200B;](/help/user-guide/approvals/review-and-edit.md#manage-approvals) できます。
1. [&#x200B; レビュー用にコンテンツにアクセス &#x200B;](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) し、修正要求を表示します。
1. レビューのコメントごとにドラフトを編集し、[&#x200B; ディスプレイ広告エクスペリエンスを公開する &#x200B;](#publish-and-export-experience) ようにします。

[&#x200B; レビューと承認 &#x200B;](/help/user-guide/approvals/overview.md) を参照してください。

## エクスペリエンスの公開と書き出し

生成したディスプレイ広告を現在および将来の使用で使用できるようにするには、[!UICONTROL &#x200B; コンテンツ &#x200B;] に公開し、マーケティングキャンペーンで使用するために書き出します。

1. **新しいディスプレイ広告エクスペリエンスを公開するには** 上部のツールバーまたは承認フロー内の **[!UICONTROL 公開]** をクリックします。
   1. 「_[!UICONTROL [!DNL Campaigns]]_」を選択し、必要に応じて&#x200B;_[!UICONTROL &#x200B; 詳細 &#x200B;]_&#x200B;を追加します。
   1. 「**[!UICONTROL 公開する]**」をクリックします。

      ![&#x200B; ディスプレイ広告の公開 &#x200B;](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **新しいディスプレイ広告エクスペリエンスを書き出すには**、上部のツールバーにある **[!UICONTROL 書き出し]** をクリックします。
   1. 形式（HTMLと画像、PNG、JPG）を選択し、「**[!UICONTROL 書き出し]**」をクリックします。

      書き出されたHTMLは、テンプレートや `div` コンテナなど、事前に定義された web プロパティ内に配置する必要があります。 これらのサイズを設定しないと、個別に表示した場合に画像がゆがんで見えることがあります。

詳しくは、[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) を参照してください。
