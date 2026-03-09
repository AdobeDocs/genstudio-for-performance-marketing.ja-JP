---
title: バナーエクスペリエンスの作成
description: パフォーマンスマーケティング用にAdobeでバナーエクスペリエ  [!DNL GenStudio]  スを作成する方法を説明します。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="この機能は現在Betaにあるので、一部の機能が制限されるか、変更される可能性があります。"
role: User
level: Beginner
recommendations: noDisplay
exl-id: c5d541a9-a97b-44da-a15c-61aceefd0e8c
TQID: https://experienceleague.adobe.com/bgBb1B5ZzEt-qvNn-U-N-95lrGjFGD9d9vE47vVV7jg
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2:
  - id: be495d08-ecd1-455f-951e-c22de504e667
  - id: de1f9646-abd3-4e21-9de2-df62ce55c8dc
  - id: dee4e9a9-78d1-4953-8179-f8da6117027d
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
  - id: f54ee13b-9545-4d68-9842-a12026e60aaf
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 1089
ht-degree: 0%

---

# バナーエクスペリエンスの作成

このチュートリアルでは、GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) （左側のナビゲーションエリアにある絵筆のアイコン [&#128279;](banner-experiences.md) を使用して、ブランド化された  バナーエクスペリエンス）を作成する方法を説明します。

魅力的なバナーエクスペリエンスをデザインするには、開始する前に、[GenStudio for Performance Marketingにガイドラインを追加する &#x200B;](/help/user-guide/guidelines/add-guidelines.md)、[&#x200B; プロンプトの記述の基本 &#x200B;](/help/user-guide/effective-prompts.md) を確認することをお勧めします。

## テンプレートを選択

バナーエクスペリエンスを作成するには、使用可能なテンプレートを使用してコンテンツのフレームワークを指定します。 サポートされるバナーディメンションについて詳しくは、[&#x200B; テンプレートのベストプラクティス &#x200B;](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines) を参照してください。

**バナーテンプレートを選択するには**:

1. _[!DNL Create]_&#x200B;で、「バナー&#x200B;**[!UICONTROL をクリック]**&#x200B;ます。
1. _フィルター_ の横にある検索オプションを使用して、特定のバナーテンプレートを見つけます。
1. _テンプレートを選択_ ビューで、バナーテンプレートをクリックします。
1. **[!UICONTROL 使用]** をクリックします。

   コンテンツ作成のホームベースであるキャンバスが表示されます。

## パラメーターを追加

プロンプトドロワー内の _パラメーター_ に [&#x200B; ガイドライン &#x200B;](/help/user-guide/guidelines/overview.md) およびアセットを組み込むと、コンテンツ生成プロセスが強化され、バナーエクスペリエンスを作成するための重要な準備手順となります。

![&#x200B; プロンプト ドロワーにパラメータを入力 &#x200B;](/help/assets/prompt-displayad2.png){width="50%" align="center"}

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

ガイドラインを選択したら、自然言語を使用して、新しいバナーエクスペリエンスのコンテンツ生成を開始するためのプロンプトを作成します。 高品質の結果を確保するためには、詳細で説明的なプロンプトを作成することが不可欠です。

プロンプトの書き込みについて詳しくは、[&#x200B; 効果的なプロンプトの書き込み &#x200B;](/help/user-guide/effective-prompts.md) を参照してください。

**プロンプトを入力するには**:

1. _生成するエクスペリエンスを記述」_ プロンプトボックスにプロンプトを入力します。
1. 「**[!UICONTROL 生成]**」をクリックします。

デフォルトでは、4 つのバリエーション（追加したプロンプト、ガイドラインおよびコンテンツに基づく）が生成され、キャンバスに表示されます。

## 生成されたバナーの変更

承認または公開用に送信する内容を選択する前に [!DNL Content] バナーセクションとテキストフィールドを編集したり、生成されたバリアントを削除したりできます。

**生成されたバリアントを修正するには**:

* **バナーのドラフト名を [&#x200B; 編集](/help/user-guide/create/manage-variants.md#change-draft-name)** するには、キャンバス上部の _名称未設定のドラフト_ タイトルをクリックし、新しいタイトルを入力します。
* **バナーを [&#x200B; 手動で編集](/help/user-guide/create/manage-variants.md#manually-edit-text)** するには、任意のバナーセクションまたはフィールド（ヘッドラインやCTAなど）をダブルクリックし、必要に応じて編集を行います。
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

1. 右側のアクションバーにある _コンテンツチェック_ パネルアイコンをクリックして、[_コンテンツチェック_ パネル &#x200B;](/help/user-guide/guidelines/brand-validation.md#content-check-panel) を開きます。 _レビューが必要_ チェックと _合格_ チェックの概要を表示し、改善が必要なセクションとガイドラインを確認します。

   ![_コンテンツチェック_ パネル &#x200B;](/help/assets/content-check-panel.png){width="300"}

2. [&#x200B; バリアントを手動で改訂 &#x200B;](#revise-generated-banners) し、バリアントが実行されたコンテンツチェックと密接に連携していることを確認します。

[&#x200B; ブランド検証 &#x200B;](/help/user-guide/guidelines/brand-validation.md) を参照してください。

## レビューと承認の取得

キャンバスの右側のアクションバーにあるアイコンとしてアクセスできる _承認_ パネルを使用して、レビューを取得、レビューコメントを追跡、関係者からの承認を取得します。

**レビューと承認を取得するには**:

1. [&#x200B; バナーのエクスペリエンスのドラフトの承認 &#x200B;](/help/user-guide/approvals/request-review.md) を依頼する [&#x200B; 承認リクエストの開始 &#x200B;](/help/user-guide/approvals/approve-content.md)。
1. レビュープロセス中に [&#x200B; レビュー担当者を削除または追加 &#x200B;](/help/user-guide/approvals/review-and-edit.md#manage-approvals) できます。
1. [&#x200B; レビュー用にコンテンツにアクセス &#x200B;](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) し、修正要求を表示します。
1. レビューコメントごとにドラフトを編集し、[&#x200B; バナーエクスペリエンスを公開する &#x200B;](#publish-and-export-experience) ようにします。

[&#x200B; レビューと承認 &#x200B;](/help/user-guide/approvals/overview.md) を参照してください。

## エクスペリエンスの公開と書き出し

生成したバナーを現在および将来の使用で使用できるようにするには、[!UICONTROL &#x200B; コンテンツ &#x200B;] に公開し、マーケティングキャンペーンで使用するためにエクスポートします。

1. **新しいバナーエクスペリエンスを公開するには**、上部のツールバーまたは承認フロー内の **[!UICONTROL 公開]** をクリックします。
   1. 「_[!UICONTROL [!DNL Campaigns]]_」を選択し、必要に応じて&#x200B;_[!UICONTROL &#x200B; 詳細 &#x200B;]_&#x200B;を追加します。
   1. 「**[!UICONTROL 公開する]**」をクリックします。

      ![&#x200B; バナーの公開 &#x200B;](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **新しいバナーを書き出すには**、上部のツールバーにある **[!UICONTROL 書き出し]** をクリックします。
   1. 形式（HTMLと画像、PNG、JPG）を選択し、「**[!UICONTROL 書き出し]**」をクリックします。

      書き出されたHTMLは、テンプレートや `div` コンテナなど、事前に定義された web プロパティ内に配置する必要があります。 これらのサイズを設定しないと、個別に表示した場合に画像がゆがんで見えることがあります。

[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) を参照してください。
