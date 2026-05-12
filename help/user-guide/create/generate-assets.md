---
title: 画像のバリエーションを生成
description: Performance Marketing用Adobe [!DNL GenStudio] で、参照画像のスタイルに一致する画像を作成します。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="この機能は現在Betaに搭載されているため、一部の機能が制限されたり、機能が変更されたりする場合があります。"
role: User
level: Beginner
recommendations: noDisplay
exl-id: c1118ada-7fee-43cd-aff4-eab69539afb4
TQID: https://experienceleague.adobe.com/NXtN00EKTe0lGI8jJMJWJfWx6mHoMQI1of1mJhgrR5U
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
  - id: e4a0febc-5163-4017-82ce-fc7594509fb6
  - id: f54ee13b-9545-4d68-9842-a12026e60aaf
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
source-git-commit: 6d1053bf94b0a0ba65be90359e4d176e64dfffae
workflow-type: tm+mt
source-wordcount: 752
ht-degree: 0%

---

# 画像のバリエーションを生成

GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) （ペイントブラシアイコン）を使用すると、選択した画像からインスピレーションを得て、視覚的なインパクトと全体的なデザインをキャプチャする&#x200B;_[!DNL Image variants]_&#x200B;生成アセットを生成できます。<!-- [two types of images](#image-types) using GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (paintbrush icon)—_[!DNL Image variants]_ and _[!DNL Similar images]_. -->

人目を引く効果的な画像をデザインするには、[GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md)にガイドラインを追加し、[&#x200B; プロンプトの作成の基本](/help/user-guide/effective-prompts.md)を確認することをお勧めします。

## 画像タイプ

_[!DNL Image variants]_&#x200B;は、選択した画像からインスピレーションを得て、視覚的なインパクトと全体的な美的感覚を捉えた生成アセットです。 これらの画像は、[!DNL Content]で既に利用可能な画像と、デザインをガイドする慎重に作成されたプロンプトを使用して作成されます。 生成プロセスで選択したブランドガイドラインとパラメーターの両方に厳密に従います。

_[!DNL Image variants]_<!-- and _[!DNL Similar images]_ -->には、人目を引く画像アセットを配信するために、設定されたガイドライン、パラメーター、および[考え抜かれたプロンプト &#x200B;](/help/user-guide/effective-prompts.md)が組み込まれています。

<!-- * _[!DNL Similar images]_—Image assets created with strong similarity to an existing selected image available in [!DNL Content]. When generating similar images, GenStudio for Performance Marketing redesigns the selected image, giving slight variations on the content to provide variety and nuance. -->

## 画像のバリエーションを生成

定義されたガイドライン、パラメーター、選択した参照画像を使用して、[!DNL Image variants]を生成できます。 これらの要素は、プロンプトと共に、一貫性のある[!DNL Image variants]の生成を導きます。

### 参照画像の選択

_[!DNL Image variants]_&#x200B;を作成するには、[!DNL Content]に保存されている既存の画像を選択します。 サポートされている画像ディメンションについて詳しくは、[&#x200B; テンプレートのベストプラクティス &#x200B;](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines)を参照してください。

**参照画像を選択するには**:

1. _[!DNL Create]_&#x200B;で、**[!UICONTROL 画像のバリエーションを生成]**&#x200B;をクリックします。
   ![画像のバリエーションを生成](./gen-image-variants.png){width="400" zoomable="yes"}
1. 参照画像を選択するには、「_[!UICONTROL コンテンツから選択]_」ボタンを使用して、特定の画像を検索します。
   ![&#x200B; コンテンツから選択](./gen-variant-select-from-content.png){width="200" zoomable="yes"}

   接続された[!DNL AEM Assets Content Hub] リポジトリからアセットを使用するには、_場所_ ドロップダウンメニューからリポジトリを選択します。 1つの画像をフィルタリングして選択します。

   ![参照画像を選択](/help/assets/select-img.png){width="400" zoomable="yes"}

1. _画像を選択_ ビューで、画像をクリックして選択ボックスをオンにします。

   選択した画像のサイズは最大10 mbです。 一度に選択できる画像は1つだけです。

1. 「**[!UICONTROL 使用]**」をクリックします。

   コンテンツ制作の中心的なハブとなるカンバスが表示されます。

### パラメーターを追加

[&#x200B; ガイドライン &#x200B;](/help/user-guide/guidelines/overview.md)とパラメーターを組み込むと、コンテンツ生成プロセスが強化され、[!DNL Image variants]を作成するための重要な準備ステップになります。

**ガイドラインとパラメーターを追加するには**:

1. 「_基本_」タブで、[!DNL Brand]を選択して、コンテンツの作成を通知します。

   このメニューで利用できるブランドがない場合は、[GenStudio for Performance Marketingにガイドラインを追加します](/help/user-guide/guidelines/add-guidelines.md)。
1. _[!UICONTROL モデル]_&#x200B;から画像生成に使用するモデルを選択します。
1. _[!UICONTROL 縦横比]_&#x200B;から目的の縦横比を選択します。

### プロンプトを入力

パラメーターを選択したら、自然言語を使用してプロンプトを作成し、画像のバリエーションを生成します。

[効果的なプロンプトの作成](/help/user-guide/effective-prompts.md)を参照してください。

**プロンプトを入力するには**:

1. プロンプト ボックスにプロンプトを入力します。
1. 「**[!UICONTROL 生成]**」をクリックします。

デフォルトでは、4つのバリエーション（プロンプト、パラメーター、追加したコンテンツをベース）が生成され、キャンバスに表示されます。

### Adobe Expressで編集

バリエーションを生成した後は、Adobe Expressを使用してAdobe GenStudio for Performance Marketingで直接編集できます。

**Adobe Expressを使用して個々の画像を編集するには**:

1. 生成された画像のバリエーションにカーソルを合わせ、_[!UICONTROL Adobe Expressで編集]_&#x200B;をクリックします。

   「_Powered by Adobe Express_」ウィンドウが表示されます。

1. [画像の切り抜き](https://helpx.adobe.com/express/create-and-edit-images/edit-images/crop-images.html)、[&#x200B; オブジェクトの削除](https://helpx.adobe.com/express/create-and-edit-images/create-and-modify-with-generative-ai/remove-objects-generative-fill.html)、エフェクトの適用などの画像編集を実行します。

   GenStudio for Performance MarketingでAdobe Expressを使用して画像を修正する方法については、[Adobe Express ドキュメント &#x200B;](https://helpx.adobe.com/express/user-guide.html)を参照してください。

1. 「_[!UICONTROL 変更を適用]_」をクリックして、編集内容を保存します。
1. 必要に応じて、個々の画像のバリエーションの編集を継続し、変更を適用して進行状況を保存します。

### コンテンツチェックの整合性の確認

生成されたバリエーションを最適化し、ブランドアイデンティティ、プラットフォームガイドライン、アクセシビリティ標準を厳密に遵守するには、[_コンテンツチェック_ パネル &#x200B;](/help/user-guide/guidelines/brand-validation.md#content-check-panel)の機能を活用します。 このパネルには、包括的なコンテンツチェックの詳細が表示され、改善点が示されます。

**コンテンツチェックを実行するには**:

1. 右側のアクションバーの&#x200B;_コンテンツチェック_ パネルアイコンをクリックして、[_コンテンツチェック_ パネル &#x200B;](/help/user-guide/guidelines/brand-validation.md#content-check-panel)を開きます。 *Needs review*&#x200B;および&#x200B;*Passed*&#x200B;のチェックの概要を表示して、改善が必要なセクションとガイドラインを確認します。

   ![_コンテンツチェック_ パネル &#x200B;](/help/assets/content-check-img.png){width="500" zoomable="yes"}

1. 画像のバリエーションを修正し、バリエーションが実行されたコンテンツチェックと密接に連携するようにします。

[&#x200B; ブランド検証](/help/user-guide/guidelines/brand-validation.md)を参照してください。

<!-- 
## Generate Similar images

You can quickly generate images similar to a selected image within [!DNL Content] from the [!DNL Create] home.

**To create _[!DNL Similar images]_**:

1. In _[!DNL Create]_, click **[!UICONTROL Similar images]**.
1. Use the search option, adjacent to _Filter_, to find a specific image.

   To use assets from a connected [!DNL AEM Assets Content Hub] repository, choose a repository from the _Location_ drop-down menu. Filter and select one image.

1. In the _Select image_ view, click on an image.
1. Click **[!UICONTROL Use]**.

   The Canvas, which serves as the central hub for content creation, is displayed. Four image variations similar to the original selected image appear.

   ![Generate similar images](/help/assets/generate-similar.png){width="400" zoomable="yes"} 
-->

## 画像の公開と書き出し

生成された画像のドラフトは、[!DNL Create] ホームの&#x200B;_最近使用した_ セクションに表示されます。

生成された画像を現在および将来の使用に使用できるようにするには、それらを[!UICONTROL &#x200B; コンテンツ &#x200B;]に公開し、マーケティングキャンペーンで使用するために書き出します。

1. **新しい画像を公開するには、上部のツールバーの**&#x200B;[!UICONTROL &#x200B;公開&#x200B;]&#x200B;**をクリックします。**
   1. _[!UICONTROL 必要に応じて、_[!UICONTROL &#x200B; キャンペーン &#x200B;]_&#x200B;または&#x200B;_[!UICONTROL &#x200B; チャネル &#x200B;]_&#x200B;などの詳細]_&#x200B;を追加します。
   1. 「**[!UICONTROL 公開する]**」をクリックします。

1. **新しい画像を書き出すには**、上部のツールバーの&#x200B;**[!UICONTROL 書き出し]**&#x200B;をクリックします。
   1. 書式（JPGまたはPNG）を選択し、**[!UICONTROL 書き出し]**&#x200B;をクリックします。

[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) を参照してください。
