---
title: メタ広告エクスペリエンスの作成
description: Performance Marketing のAdobe GenStudioを使用して、FacebookまたはInstagram向けのオンブランドのメタ広告エクスペリエンスを作成する方法を説明します。
feature: Content, Brands Service, Guidelines, Content Generation, Create, Experiences, Variant Generation
role: User
level: Beginner
type: Tutorial
recommendations: noDisplay
exl-id: 42111bbf-70cd-4fd2-a7a9-15abe072d720
source-git-commit: 30cd73ba1beb582ea4ac73eca7e17715f9aafc66
workflow-type: tm+mt
source-wordcount: '1074'
ht-degree: 0%

---

# メタ広告エクスペリエンスの作成

このチュートリアルでは、GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) （左側のナビゲーションエリアにある絵筆のアイコン ](/help/user-guide/create/meta-experiences.md) を使用して、ブランド化された [ メタ広告エクスペリエンス）を生成する方法を説明します。

メタ広告エクスペリエンスの生成を開始する前に、GenStudio for Performance Marketing で [ ガイドラインを組み込む ](/help/user-guide/guidelines/add-guidelines.md) ことが重要です。また、[ プロンプトの作成 ](/help/user-guide/effective-prompts.md) の基本を理解しておく必要があります。

## テンプレートを選択

新しいメタ広告エクスペリエンスの生成を開始するには、使用可能なテンプレートを使用して、コンテンツのフレームワークを提供します。

**メタ広告テンプレートを選択するには**:

1. _[!DNL Create]_**[!UICONTROL で、「今日は何を作成しますか？」の_ メタ広告]** をクリックします。_セクション。
1. _フィルター_ の横にある検索オプションを使用して、特定のメタ広告テンプレートを見つけます。
1. テンプレートをクリックして選択し、「**[!UICONTROL 使用]**」をクリックします。

   これにより、コンテンツ作成の中心となるキャンバスが開きます。

## パラメーターを追加

[ ガイドライン ](/help/user-guide/guidelines/overview.md) とアセットを _パラメーター_ のプロンプト領域に追加すると、コンテンツ生成プロセスが強化されます。これは、メタ広告を生成するための準備における重要な手順です。

**パラメーターとアセットを追加するには**:

1. _パラメーター_ アイコンをクリックして、プロンプト領域を展開します。
1. 「_パラメーター_」セクションで、ガイドライン（[!DNL Brands]、[!DNL Personas]、[!DNL Products]）を選択して、コンテンツの作成を通知します。

   これらのメニューに表示されるブランド、ペルソナまたは商品がない場合は、[ パフォーマンスマーケティングのGenStudioにガイドラインを追加してください ](/help/user-guide/guidelines/add-guidelines.md)。

1. 「**[!UICONTROL コンテンツを選択]**」をクリックして、エクスペリエンスで使用するコンテンツを追加 *および* をクリックすると、コンテンツの生成に影響が及びます。
   * [!DNL Content] に公開済みのアセット（画像）を選択するには、**[!UICONTROL コンテンツから選択]** をクリックし、目的の画像をクリックして選択します。 フィルターを使用して、検索結果をさらに絞り込みます。

     接続されたAEM Content Hub リポジトリに既に存在するアセットを使用する場合は、_場所_ ドロップダウンメニューから該当する場所を選択し、クリックして目的の画像を選択します。

   * **[!UICONTROL アップロード]** をクリックしてファイルを参照し、使用するアセットを選択します。 デバイスの参照に加えて、Microsoft OneDrive またはDropboxから読み込むこともできます。 目的の画像をクリックして選択します。
   * アセットを「_コンテンツ_ セクションにドラッグ&amp;ドロップします。
1. **[!UICONTROL 使用]** をクリックします。

パラメーターの追加が完了したら、「_パラメーター_」アイコンを再度クリックすると、プロンプト領域を折りたたむことができます。

## プロンプトを入力

ガイドラインを選択したら、自然言語を使用してプロンプトを作成し、新しいメタ広告エクスペリエンスのコンテンツの生成を開始します。 詳細なプロンプトは、曖昧なプロンプトや説明のつかないプロンプトよりも高品質の出力を生成します。

プロンプトの書き込みについて詳しくは、[ 効果的なプロンプトの書き込み ](/help/user-guide/effective-prompts.md) を参照してください。

**プロンプトを入力するには**:

1. _生成するエクスペリエンスを記述」_ プロンプトボックスにプロンプトを入力します。
1. 「**[!UICONTROL 生成]**」をクリックします。

デフォルトでは、4 つのバリエーション（追加したプロンプト、ガイドラインおよびコンテンツによってすべて強化される）が生成され、キャンバスに表示されます。

生成されたコンテンツは徐々に読み込まれます。メタエクスペリエンスの各セクションが生成されると、キャンバスに表示されます。 これらの変更がキャンバスにどのように読み込まれるかを学ぶには、[ メタエクスペリエンス ](/help/user-guide/create/meta-experiences.md#progressive-loading) を参照してください。

## メタ広告チャネルを選択

メタ広告を生成する際は、Facebook広告またはInstagram広告を選択できます。

右側のメニューバー（FacebookとInstagramのアイコン **で「** Facebook」と「**Instagram**」の間のメタ広告チャネルオプションを切り替えて、各チャネルのバリアントを表示および管理します。

[ メタ広告の変更 ](#revise-generated-meta-ads) を行う場合、Facebook広告とInstagram広告の縦横比を変更できます。

## 生成されたメタ広告を変更

承認または公開用に送信する内容を選択する前に [!DNL Content] メタ広告を編集したり、生成された広告のセットからバリアントを削除したりできます。

**生成されたバリアントを修正するには**:

* **メタ広告のドラフト名を [ 編集](/help/user-guide/create/manage-variants.md#change-draft-name)** するには、キャンバスの上部にある _名称未設定のドラフト_ タイトルをクリックし、新しいタイトルを入力します。
* **メタ広告を [ 手動で編集](/help/user-guide/create/manage-variants.md#manually-edit-text)** するには、任意の広告セクション（件名行、ヘッダー、本文コピーなど）をダブルクリックし、必要に応じて編集します。
* **コールトゥアクションを変更または選択するには**、コールトゥアクションボタンをクリックし、使用可能なボタンテキストオプションから選択します。 _[!UICONTROL リンク]_ に、コールトゥアクションテキストの URL を入力します。
* **広告のサイズと縦横比を [ 変更](/help/user-guide/create/manage-variants.md#change-aspect-ratio)** するには、_[!UICONTROL サイズ変更]_ ボタン（キャンバスの左側にボタンアイコンが表示されたボックス）をクリックし、すべてのバリアントに適用する新しいサイズと縦横比を選択します。 バリアントが複製され、サイズが変更されます。
<!-- * **To [regenerate a section of a variant](/help/user-guide/create/manage-variants.md#re-generate-sections)**, click an editable text field and use the _[!UICONTROL Suggested edits]_ options or enter a new prompt and click **[!UICONTROL Generate]**. -->
* **画像を [ 切り抜きまたは再配置](/help/user-guide/create/manage-variants.md#crop-assets)** するには、画像の上にマウスポインターを置き、表示される切り抜きアイコンをクリックし、画像のサイズと配置を調整します。
* **メタ広告を [ 削除](/help/user-guide/create/manage-variants.md#delete-variant)** するには、広告タイトル（「Meta 4」など）をクリックし、**[!UICONTROL バリアントを削除]** をクリックします。

## 生成フィードバックを送信

生成出力の品質に関する [ フィードバックを送信 ](/help/user-guide/create/manage-variants.md#generation-feedback) するには、オプションアイコン（3 つのドット）をクリックし、**[!UICONTROL 良好な出力]** または **[!UICONTROL 不良な出力]** を選択します。

## ブランドの整合性の確認

生成される広告を最適化し、ブランドアイデンティティに厳密に準拠するには、[_ブランドガイドラインチェック_](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) の機能を活用して、バリアントのブランド調整の概要を提供します。また、[_ブランド検証_ パネル ](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) を使用して、包括的なブランド検証の詳細を表示し、改善点を明確にします。

**ブランドの整合性を検証するには**:

1. バリアントの [**[!UICONTROL [!DNL Brand] guidelines check]**](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) アイコンをクリックすると、ブランドに対してチェックされたときのそのバリアントのパフォーマンスの概要が表示されます。
1. 改善が必要なセクションとガイドラインの詳細を取得するには、**[!UICONTROL 確認]**_をクリックするか_ 上部のメニューバーにあるブランド検証アイコンをクリックして [_ブランド検証パネル_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) を開きます。

1. 各広告を切り替えて、生成されたコンテンツを改善してブランドに合わせる方法を確認します。
1. [ 手動で広告を改訂 ](#revise-generated-meta-ads) して、広告がブランドと密接に連携していることを確認します。

[ ブランド検証 ](/help/user-guide/guidelines/brand-validation.md) を参照してください。

## レビューと承認の取得

キャンバスの上部のメニューバーからアクセスできる承認パネルを使用して、レビューを取得、レビューコメントを追跡、関係者からの承認を取得します。

**レビューと承認を取得するには**:

1. [ ドラフトのメタ広告エクスペリエンスの承認 ](/help/user-guide/approvals/request-review.md) を依頼する [ 承認リクエストの開始 ](/help/user-guide/approvals/approve-content.md)。
1. レビュープロセス中に [ レビュー担当者を削除または追加 ](/help/user-guide/approvals/review-and-edit.md#manage-approvals) できます。
1. [ レビュー用にコンテンツにアクセス ](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) し、修正要求を表示します。
1. レビューのコメントごとにドラフトを編集し [ メタ広告エクスペリエンスを公開 ](#publish-and-export-experience) します。

詳しくは、[ レビューと承認 ](/help/user-guide/approvals/overview.md) を参照してください。

## Publishと書き出しの経験

生成したメタ広告を現在および将来の使用で使用できるようにするには、[!UICONTROL  コンテンツ ] に公開し、マーケティングキャンペーンで使用するためにエクスポートします。

1. **新しいメタ広告エクスペリエンスを公開するには**、上部のツールバーの **[!UICONTROL Publish]** をクリックします。
1. **新しいメタ広告エクスペリエンスを書き出すには** 上部のツールバーにある **[!UICONTROL 書き出し]** をクリックします。
   1. CSV 形式と画像またはHTML形式のみを選択し、「**[!UICONTROL 書き出し]**」をクリックします。

詳細は、[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) を参照してください。

## メタを接続

GenStudio for Performance Marketing を Meta に接続して、コンテンツのパフォーマンスに関する高度な分析と [ インサイト ](/help/user-guide/insights/overview.md) を受け取ることができます。

詳しくは、[ チャネルアカウントの接続 ](/help/user-guide/insights/connect-channel.md) を参照してください。
