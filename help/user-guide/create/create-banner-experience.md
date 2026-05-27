---
title: バナーエクスペリエンスの構築
description: Adobe [!DNL GenStudio] for Performance Marketingでバナーエクスペリエンスを作成する方法について説明します。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="この機能は現在Betaに搭載されているため、一部の機能が制限されたり、機能が変更されたりする場合があります。"
role: User
level: Beginner
recommendations: noDisplay
exl-id: c5d541a9-a97b-44da-a15c-61aceefd0e8c
TQID: https://experienceleague.adobe.com/bgBb1B5ZzEt-qvNn-U-N-95lrGjFGD9d9vE47vVV7jg
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2: id: be495d08-ecd1-455f-951e-c22de504e667id: de1f9646-abd3-4e21-9de2-df62ce55c8dcid: dee4e9a9-78d1-4953-8179-f8da6117027did: e3878dde-4b87-4290-9e81-ed7ee6eb83feid: f54ee13b-9545-4d68-9842-a12026e60aaf
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
source-git-commit: e8e0898054576454bad9ecdbd1a48b17f955e138
workflow-type: tm+mt
source-wordcount: 1089
ht-degree: 0%

---

# バナーエクスペリエンスの作成

このチュートリアルでは、GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) （左側のナビゲーション領域のペイントブラシアイコン）を使用して、ブランド化された[ バナーエクスペリエンス ](banner-experiences.md)を作成する方法を説明します。

魅力的なバナーエクスペリエンスをデザインするには、開始する前に[GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md)にガイドラインを追加し、[ プロンプトの作成の基本](/help/user-guide/effective-prompts.md)を確認することをお勧めします。

## テンプレートの選択

バナーエクスペリエンスを作成するには、使用可能なテンプレートを使用して、コンテンツのフレームワークを提供します。 サポートされているバナーディメンションについて詳しくは、[ テンプレートのベストプラクティス ](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines)を参照してください。

**バナーテンプレートを選択するには**:

1. _[!DNL Create]_で、**[!UICONTROL バナー]**をクリックします。
1. 特定のバナーテンプレートを検索するには、_フィルター_&#x200B;の横にある検索オプションを使用します。
1. _テンプレートを選択_ ビューで、バナーテンプレートをクリックします。
1. 「**[!UICONTROL 使用]**」をクリックします。

   コンテンツ作成のホームベースとなるカンバスが表示されます。

## パラメーターを追加

[ ガイドライン ](/help/user-guide/guidelines/overview.md)とアセットを&#x200B;_パラメーター_&#x200B;にプロンプト ドロワー内に組み込むと、コンテンツ生成プロセスが強化され、バナーエクスペリエンスを作成するための重要な準備ステップになります。

![ プロンプト ドロワーにパラメーターを入力](/help/assets/prompt-displayad2.png){width="50%" align="center"}

**パラメーターとアセットを追加するには**:

1. _パラメーター_ アイコンをクリックして、プロンプトドロワーを展開します。
1. 「_パラメーター_」セクションで、コンテンツ作成に役立つガイドライン（[!DNL Brands]、[!DNL Personas]、および[!DNL Products]）を選択します。

   これらのメニューから利用できるブランド、ペルソナ、または製品がない場合は、[GenStudio for Performance Marketingにガイドラインを追加します](/help/user-guide/guidelines/add-guidelines.md)。

1. エクスペリエンス *および*&#x200B;で使用するコンテンツを追加して、コンテンツ生成に影響を与えるには：
   * 「**[!UICONTROL コンテンツから選択]**」をクリックして、[!DNL Content] リポジトリからアセット（画像）を選択し、フィルターを実行して1つ以上の画像を選択します。

     接続された[!DNL AEM Assets Content Hub] リポジトリからアセットを使用するには、_場所_ ドロップダウンメニューからリポジトリを選択します。 1つまたは複数の画像をフィルタリングして選択します。

   * または、**[!UICONTROL コンテンツから選択]** セクションにアセットをドラッグ&amp;ドロップして、1つ以上の新しいアセットをアップロードします。
1. 「**[!UICONTROL 使用]**」をクリックします。

パラメーターの追加が完了したら、_パラメーター_ アイコンをもう一度クリックして、プロンプトドロワーを折りたたみます。

## プロンプトを入力

ガイドラインを選択したら、自然言語を使用してプロンプトを作成し、新しいバナーエクスペリエンスのコンテンツ生成を開始します。 質の高い結果を得るためには、詳細で記述的なプロンプトを作成することが重要です。

プロンプトの作成について詳しくは、[効果的なプロンプトの作成](/help/user-guide/effective-prompts.md)を参照してください。

**プロンプトを入力するには**:

1. _「生成するエクスペリエンスについて説明する」プロンプト ボックスにプロンプトを入力します。_
1. 「**[!UICONTROL 生成]**」をクリックします。

デフォルトでは、プロンプト、ガイドライン、追加したコンテンツをベースにした4つのバリエーションが生成され、キャンバスに表示されます。

## 生成されたバナーを修正

承認または[!DNL Content]への公開のために送信するものを選択する前に、バナーセクションとテキストフィールドを編集するか、生成されたバリエーションを削除できます。

**生成されたバリエーションを修正するには**:

* **バナーのドラフト名](/help/user-guide/create/manage-variants.md#change-draft-name)**&#x200B;を[編集するには、キャンバスの上部にある&#x200B;_名称未設定のドラフト_ タイトルをクリックし、新しいタイトルを入力します。
* **バナーを手動で編集するには](/help/user-guide/create/manage-variants.md#manually-edit-text)**&#x200B;で、バナーセクションまたはフィールド（見出しやCTAなど）をダブルクリックし、必要に応じて編集します。[
* **バリエーションで[ テキストの書式設定](/help/user-guide/create/manage-variants.md#manually-edit-text)**&#x200B;を適用するには、バリエーションの画像テキストまたはインラインリンクをクリックし、**[!UICONTROL テキストの書式設定]**&#x200B;をクリックします。
* **バリアント](/help/user-guide/create/manage-variants.md#re-generate-sections)**&#x200B;のセクションを[再生成するには、編集可能なテキストフィールドをクリックし、_[!UICONTROL おすすめの編集]_ オプションを使用するか、_[!UICONTROL 新しいテキストを生成_ セクション ]に新しいプロンプトを入力して、**[!UICONTROL 生成]**&#x200B;をクリックします。
* **バリアントの画像を[追加または入れ替えるには、](/help/user-guide/create/manage-variants.md#swap-image)**&#x200B;画像アセット （または画像が現在存在しない場合は画像アセット領域）をクリックし、**[!UICONTROL コンテンツから入れ替え]** アイコンをクリックします。
* **バリアント](/help/user-guide/create/manage-variants.md#add-image-link)**&#x200B;の画像にリンクを[追加するには、画像アセット（または画像が現在存在しない場合は画像アセット領域）をクリックし、リンクアイコンをクリックします。
* **バリアント](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**&#x200B;の画像に代替テキストを[追加するには、画像アセットをクリックし、_代替テキスト_ オプションを使用して、画像ごとに代替テキストを手動で追加または生成します。
* **バリエーションに[ アクセシビリティラベル ](/help/user-guide/create/manage-variants.md#add-accessibility-labels)を追加するには**&#x200B;画像またはcall-to-action リンクをクリックし、リンクまたはボタンの機能を説明する簡単な説明を入力します。
* **広告](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**&#x200B;のサイズと縦横比を[変更するには、_[!UICONTROL サイズ変更]_ ボタン（キャンバスの左側にボタンアイコン付きのボックス）をクリックし、新しいサイズと縦横比を選択して、すべてのバリエーションに適用します。 バリエーションが重複し、サイズが変更されます。
* **画像を[切り抜きまたは再配置](/help/user-guide/create/manage-variants.md#crop-assets)**&#x200B;するには、画像をクリックし、**[!UICONTROL 編集]** （鉛筆アイコン）をクリックしてから&#x200B;**[!UICONTROL 切り抜き]**&#x200B;をクリックします。 画像のサイズと配置を調整します。
* **生成拡張を使用して画像のサイズを変更し、画像を作業中のテンプレート**&#x200B;に合わせるには、画像をクリックし、**[!UICONTROL 編集]** （鉛筆アイコン）をクリックしてから&#x200B;**[!UICONTROL 拡張]**&#x200B;します。 [](/help/user-guide/create/manage-variants.md#use-generative-expand)必要なアスペクト比とテンプレートに合わせて画像を調整します。

<!-- 
# Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. 
-->

## 生成フィードバックを送信

生成出力の品質に関するフィードバック ](/help/user-guide/create/manage-variants.md#generation-feedback)を[送信するには、オプションアイコン（3つのドット）をクリックし、**[!UICONTROL 良好な出力]**&#x200B;または&#x200B;**[!UICONTROL 不良な出力]**&#x200B;を選択します。

## コンテンツチェックの整合性の確認

生成されたバリエーションを最適化し、ブランドアイデンティティ、プラットフォームガイドライン、アクセシビリティ標準を厳密に遵守するには、[_コンテンツチェック_ パネル ](/help/user-guide/guidelines/brand-validation.md#content-check-panel)の機能を活用します。 このパネルには、包括的なコンテンツチェックの詳細が表示され、改善点が示されます。

**バリアントに対してコンテンツチェックを実行するには**:

1. 右側のアクションバーの&#x200B;_コンテンツチェック_ パネルアイコンをクリックして、[_コンテンツチェック_ パネル ](/help/user-guide/guidelines/brand-validation.md#content-check-panel)を開きます。 _Needs review_&#x200B;および&#x200B;_Passed_&#x200B;のチェックの概要を表示して、改善が必要なセクションとガイドラインを確認します。

   ![_コンテンツチェック_ パネル ](/help/assets/content-check-panel.png){width="300"}

2. [ バリエーションを手動で修正](#revise-generated-banners)して、バリエーションが実行されたコンテンツチェックと密接に連携していることを確認します。

[ ブランド検証](/help/user-guide/guidelines/brand-validation.md)を参照してください。

## レビューと承認を取得

キャンバスの右側のアクションバーのアイコンとしてアクセスできる&#x200B;_承認_ パネルを使用して、レビューの取得、レビューコメントの追跡、関係者からの承認の取得を行います。

**レビューと承認を取得するには**:

1. [承認要求](/help/user-guide/approvals/request-review.md)を開始して、ドラフトされたバナーエクスペリエンスの[承認を求めます](/help/user-guide/approvals/approve-content.md)。
1. レビュープロセス中に[ レビュー担当者](/help/user-guide/approvals/review-and-edit.md#manage-approvals)を削除または追加します。
1. [ レビュー用のコンテンツにアクセス ](/help/user-guide/approvals/review-and-edit.md#access-content-for-review)し、リビジョンのリクエストを表示します。
1. レビューのコメントごとにドラフトを編集し、[ バナーエクスペリエンスを公開](#publish-and-export-experience)します。

[ レビューと承認](/help/user-guide/approvals/overview.md)を参照してください。

## エクスペリエンスの公開と書き出し

生成されたバナーを現在および将来の使用に使用できるようにするには、それを[!UICONTROL  コンテンツ ]に公開し、マーケティングキャンペーンで使用するために書き出します。

1. **新しいバナーエクスペリエンスを公開するには、上部のツールバーまたは承認フロー内の**[!UICONTROL &#x200B;公開&#x200B;]**をクリックします。**
   1. _[!UICONTROL [!DNL Campaigns]]_を選択し、必要に応じて_[!UICONTROL &#x200B;詳細&#x200B;]_を追加します。
   1. 「**[!UICONTROL 公開する]**」をクリックします。

      ![ バナーを公開](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **新しいバナーを書き出すには**、上部のツールバーの&#x200B;**[!UICONTROL 書き出し]**&#x200B;をクリックします。
   1. HTMLと画像、PNGまたはJPGのフォーマットを選択し、**[!UICONTROL 書き出し]**&#x200B;をクリックします。

      書き出されたHTMLは、テンプレートや`div` コンテナなど、事前定義されたweb プロパティ内に配置する必要があります。 これらの設定された寸法を使用しない場合、画像は独立して表示されるときに歪んで表示される可能性があります。

[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) を参照してください。
