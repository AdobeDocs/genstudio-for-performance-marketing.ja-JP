---
title: 画像を生成
description: パフォーマンスマーケティング用に、Adobeで参照画像のスタイルに合  [!DNL GenStudio]  た画像を作成します。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="この機能は現在Betaにあるので、一部の機能が制限されるか、変更される可能性があります。"
role: User
level: Beginner
recommendations: noDisplay
exl-id: c1118ada-7fee-43cd-aff4-eab69539afb4
source-git-commit: 47195c08f500e50a01db127c6badc461c10afaf9
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 1%

---

# 画像の生成

GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) （絵筆のアイコン）を使用すると、選択した画像からインスピレーションを得て、その視覚的なインパクトと全体的な美学をキャプチャする _[!DNL On-brand images]_ール生成されたアセットを生成できます。<!-- [two types of images](#image-types) using GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (paintbrush icon)—_[!DNL On-brand images]_ and _[!DNL Similar images]_. -->

人目を引く効果的な画像をデザインするには、[GenStudio for Performance Marketingにガイドラインを追加する ](/help/user-guide/guidelines/add-guidelines.md)、[ プロンプトの記述の基本 ](/help/user-guide/effective-prompts.md) を確認することをお勧めします。

## 画像タイプ

選択し _[!DNL On-brand images]_画像からインスピレーションを得て、その視覚的なインパクトと全体的な美学をキャプチャする生成されたアセットです。 これらの画像は、[!DNL Content] で既に使用可能な画像と、デザインをガイドする慎重に作成されたプロンプトを使用して作成されます。 生成プロセス中に選択したブランドガイドラインとパラメーターの両方に厳密に従います。

設定 _[!DNL On-brand images]_れたガイドライン、パラメーター、<!-- and _[!DNL Similar images]_ --> 慎重に作成されたプロンプト [ を組み込んで、人目を引く画像アセットを配信で ](/help/user-guide/effective-prompts.md) ます。

<!-- * _[!DNL Similar images]_—Image assets created with strong similarity to an existing selected image available in [!DNL Content]. When generating similar images, GenStudio for Performance Marketing redesigns the selected image, giving slight variations on the content to provide variety and nuance. -->

## オンブランド画像の生成

定義済みのガイドライン、パラメーター、選択した参照画像を使用して、[!DNL On-brand images] を生成できます。 これらの要素は、プロンプトと共に、一貫性のある [!DNL On-brand image] バリエーションの生成をガイドします。

### 参照画像を選択

_[!DNL On-brand images]_を作成するには、[!DNL Content] に保存されている既存の画像を選択します。 サポートされる [ ディメンションについて詳しくは、](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) テンプレートのベストプラクティス [!DNL on-brand image] を参照してください。

**参照画像を選択するには**:

1. _[!DNL Create]_で、**[!UICONTROL ブランド上画像]**をクリックします。
1. _フィルター_ の横にある検索オプションを使用して、特定の画像を検索します。

   ![ 参照画像を選択 ](/help/assets/select-img.png){width="400" zoomable="yes"}

   接続された [!DNL AEM Assets Content Hub] リポジトリのアセットを使用するには、_場所_ ドロップダウンメニューからリポジトリを選択します。 1 つの画像をフィルタリングして選択します。

1. _画像を選択_ ビューで、画像をクリックします。

   選択する画像のサイズは最大 10 MB です。

1. **[!UICONTROL 使用]** をクリックします。

   コンテンツ作成の中央ハブとして機能するキャンバスが表示されます。

### パラメーターを追加

[ ガイドライン ](/help/user-guide/guidelines/overview.md) およびパラメーターを組み込むと、コンテンツ生成プロセスが強化され、コンテン [!DNL on-brand image] を生成するための重要な準備手順となります。

**ガイドラインとパラメーターを追加するには**:

1. 「_基本_」タブで、コンテンツの作成を通知する [!DNL Brand] を選択します。

   このメニューから利用できるブランドがない場合は、[GenStudio for Performance Marketingにガイドラインを追加 ](/help/user-guide/guidelines/add-guidelines.md) します。

1. 目的に合った画像カテゴリを _[!UICONTROL 画像カテゴリ]_ から選択します。

   画像カテゴリは、[!DNL Brand] を選択した場合に使用できます。 オプションは、選択した [!DNL Brand] によって決定されます。

<!-- 1. _(Optional)_ Select a custom model from _[!UICONTROL Model]_.

   Models are available if you access to [custom models in Firefly](https://adobedx.slack.com/archives/CMF1JGMLY/p1743534402774569). The _Models_ list will be blank if you do not have access. -->

1. _[!UICONTROL 縦横比]_ から目的の縦横比を選択します。
1. **[!UICONTROL スタイル参照]** の _[!UICONTROL コンテンツから選択]_ をクリックして、参照画像を追加します。 選択する画像は、生成する画像の視覚的な美しさと深さに影響を与えます。

   接続された [!DNL AEM Assets Content Hub] リポジトリのアセットを使用するには、_場所_ ドロップダウンメニューからリポジトリを選択します。 1 つの画像をフィルタリングして選択します。

1. 「_詳細_」タブで、「_コンテンツタイプ_」を選択します。

   これは、選択したア [!DNL Brand] ット（_アート_ または _写真_ に存在する画像カテゴリに基づいて事前に選択されており、編集できません。

1. 画像の既存の視覚特性の全体的な強さを _[!UICONTROL 視覚強度]_ で調整します。

### プロンプトを入力

パラメーターを選択したら、自然言語を使用してプロンプトを作成し、ブランド画像での生成を開始します。

[ 有効なプロンプトの記述 ](/help/user-guide/effective-prompts.md) を参照してください。

**プロンプトを入力するには**:

1. プロンプトボックスにプロンプトを入力します。
1. 「**[!UICONTROL 生成]**」をクリックします。

デフォルトでは、4 つのバリエーション（追加したプロンプト、パラメーター、コンテンツによって促進される）が生成され、キャンバスに表示されます。

### Adobe Expressで編集

画像のバリアントを生成したら、Adobe Expressを使用してAdobe GenStudio for Performance Marketingで直接編集できます。

**Adobe Expressを使用して個々の画像を編集するには**:

1. 生成された画像バリアントの上にマウスポインターを置いて、「_[!UICONTROL Adobe Expressで編集]_」をクリックします。

   _Adobe Expressを使用_ ウィンドウが表示されます。

1. [ 画像の切り抜き ](https://helpx.adobe.com/express/create-and-edit-images/edit-images/crop-images.html)、[ オブジェクトの削除 ](https://helpx.adobe.com/express/create-and-edit-images/create-and-modify-with-generative-ai/remove-objects-generative-fill.html)、エフェクトの適用などの画像編集を実行します。

   Adobe Expressを使用してAdobe Expressで画像を変更する方法については [](https://helpx.adobe.com/express/user-guide.html)GenStudio for Performance Marketing ドキュメント } を参照してください。

1. 「_[!UICONTROL 変更を適用]_」をクリックして編集内容を保存します。
1. 必要に応じて個々の画像のバリエーションを編集し、変更を適用して進行状況を保存します。

### コンテンツチェックの整合性の確認

生成されたバリアントを最適化し、ブランド ID、プラットフォームガイドラインおよびアクセシビリティ標準に厳密に準拠するには、[_コンテンツチェック_ パネル ](/help/user-guide/guidelines/brand-validation.md#content-check-panel) の機能を活用します。 このパネルには、包括的なコンテンツチェックの詳細が表示され、改善点が明らかになります。

**コンテンツチェックを実行するには**:

1. 右側のアクションバーにある _コンテンツチェック_ パネルアイコンをクリックして、[_コンテンツチェック_ パネル ](/help/user-guide/guidelines/brand-validation.md#content-check-panel) を開きます。 *レビューが必要* チェックと *合格* チェックの概要を表示し、改善が必要なセクションとガイドラインを確認します。

   ![_コンテンツチェック_ パネル ](/help/assets/content-check-img.png){width="500" zoomable="yes"}

1. 画像のバリアントを改訂し、バリアントが実行されるコンテンツチェックと密接に合致するようにします。

[ ブランド検証 ](/help/user-guide/guidelines/brand-validation.md) を参照してください。

<!-- ## Generate Similar images

You can quickly generate images similar to a selected image within [!DNL Content] from the [!DNL Create] home.

**To create _[!DNL Similar images]_**:

1. In _[!DNL Create]_, click **[!UICONTROL Similar images]**.
1. Use the search option, adjacent to _Filter_, to find a specific image.

   To use assets from a connected [!DNL AEM Assets Content Hub] repository, choose a repository from the _Location_ drop-down menu. Filter and select one image.

1. In the _Select image_ view, click on an image.
1. Click **[!UICONTROL Use]**.

   The Canvas, which serves as the central hub for content creation, is displayed. Four image variations similar to the original selected image appear.

   ![Generate similar images](/help/assets/generate-similar.png){width="400" zoomable="yes"} -->

## 画像の公開と書き出し

生成された画像のドラフトは、_ホームの_ 最近 [!DNL Create] セクションに表示されます。

生成した画像を現在および将来の使用で使用できるようにするには、画像を [!UICONTROL  コンテンツ ] に公開し、マーケティングキャンペーンで使用するために書き出します。

1. **新しい画像を公開するには**、上部のツールバーにある **[!UICONTROL 公開]** をクリックします。
   1. 必要に応じて _[!UICONTROL キャンペーン]_ や _[!UICONTROL チャネル]_ などの _[!UICONTROL 詳細を追加]_ します。
   1. 「**[!UICONTROL 公開する]**」をクリックします。

1. **新しい画像を書き出すには**、上部のツールバーにある **[!UICONTROL 書き出し]** をクリックします。
   1. フォーマット（JPGまたは PNG）を選択し、「**[!UICONTROL エクスポート]**」をクリックします。

詳しくは、[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) を参照してください。
