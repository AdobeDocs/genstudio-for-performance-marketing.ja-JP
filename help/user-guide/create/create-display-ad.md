---
title: ディスプレイとエクスペリエンスの作成
description: パフォーマンスマーケティング用にAdobeでディスプレイ広告エクスペリエンス  [!DNL GenStudio]  作成する方法を説明します。
feature: Brands Service, Guidelines, Content Generation, Generative AI, Create, Experiences, Variant Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 7d5e777b-7a30-48f4-b253-9823e38eecce
source-git-commit: 6d70de011493e34a72a3d25e1aae23491034a9e2
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 0%

---

# ディスプレイとエクスペリエンスの作成

このチュートリアルでは、GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) （左側のナビゲーションエリアにある絵筆のアイコン ](display-ad-experiences.md) を使用してブランド化 [ ディスプレイ広告エクスペリエンス）を生成する方法を説明します。

魅力的なディスプレイ広告体験をデザインするには、開始する前に [GenStudio for Performance Marketingにガイドラインを追加 ](/help/user-guide/guidelines/add-guidelines.md)、「プロンプトの記述の基本 [ を確認するこ ](/help/user-guide/effective-prompts.md) をお勧めします。

## テンプレートを選択

ディスプレイとエクスペリエンスを作成するには、使用可能なテンプレートを使用してコンテンツのフレームワークを提供します。 サポートされるディスプレイ広告ディメンションについて詳しくは、[ テンプレートのベストプラクティス ](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) を参照してください。

**ディスプレイ広告テンプレートを選択するには**:

1. _[!DNL Create]_**[!UICONTROL で、「今日は何を作成しますか？」の_ 広告を表示]** をクリックします。_セクション。
1. _フィルター_ の横にある検索オプションを使用して、特定のディスプレイ広告テンプレートを見つけます。
1. _テンプレートを選択_ ビューで、ディスプレイ広告テンプレートをクリックします。
1. **[!UICONTROL 使用]** をクリックします。

   コンテンツ作成の中央ハブとして機能するキャンバスが表示されます。

## パラメーターを追加

プロンプトドロワーの _パラメーター_ に [ ガイドライン ](/help/user-guide/guidelines/overview.md) とアセットを追加することは、コンテンツ生成プロセスをスーパーチャージし、ディスプレイ広告エクスペリエンスを生成するための不可欠な準備手順です。

**パラメーターとアセットを追加するには**:

1. _パラメーター_ アイコンをクリックして、プロンプトドロワーを展開します。
1. 「_パラメーター_」セクションで、ガイドライン（[!DNL Brands]、[!DNL Personas]、[!DNL Products]）を選択して、コンテンツの作成を通知します。

   これらのメニューから利用できるブランド、ペルソナ、製品がない場合は、[GenStudio for Performance Marketingにガイドラインを追加 ](/help/user-guide/guidelines/add-guidelines.md) します。

1. エクスペリエンス *および* で使用するコンテンツを追加して、コンテンツの生成に影響を与えるには、次のようにします。
   * **[!UICONTROL コンテンツから選択]** をクリックして、[!DNL Content] リポジトリからアセット（画像）を選択し、1 つ以上の画像をフィルタリングして選択します。

     接続された [!DNL AEM Assets Content Hub] リポジトリのアセットを使用するには、_場所_ ドロップダウンメニューからリポジトリを選択します。 1 つ以上の画像のフィルタリングと選択

   * または、アセットを「**[!UICONTROL コンテンツから選択]** セクションにドラッグ&amp;ドロップして、1 つ以上の新しいアセットをアップロードします。
1. **[!UICONTROL 使用]** をクリックします。

パラメーターの追加が完了したら、「_パラメーター_ アイコンをもう一度クリックして、プロンプトドロワーを折りたたみます。

## プロンプトを入力

ガイドラインを選択したら、自然言語を使用してプロンプトを作成し、新しいディスプレイとエクスペリエンスのコンテンツの生成を開始します。 生成されるディスプレイとエクスペリエンスの品質を高めるには、詳細で説明的なプロンプトを作成することが重要です。

![ プロンプトを入力 ](/help/assets/prompt-displayad.png){width="650" zoomable="yes"}

プロンプトの書き込みについて詳しくは、[ 効果的なプロンプトの書き込み ](/help/user-guide/effective-prompts.md) を参照してください。

**プロンプトを入力するには**:

1. _生成するエクスペリエンスを記述」_ プロンプトボックスにプロンプトを入力します。
1. 「**[!UICONTROL 生成]**」をクリックします。

デフォルトでは、4 つのバリエーション（追加したプロンプト、ガイドラインおよびコンテンツに基づく）が生成され、キャンバスに表示されます。

## 生成されたディスプレイ広告を変更

に承認または公開するために送信する内容を選択する前に [!DNL Content] ディスプレイ広告セクションとテキストフィールドを編集したり、生成されたバリアントを削除したりできます。

**生成されたバリアントを修正するには**:

* **ディスプレイとドラフトの名前を [ 編集](/help/user-guide/create/manage-variants.md#change-draft-name)** するには、キャンバスの上部にある _名称未設定のドラフト_ タイトルをクリックし、新しいタイトルを入力します。
* **ディスプレイ広告を [ 手動で編集](/help/user-guide/create/manage-variants.md#manually-edit-text)** するには、ディスプレイ広告の任意のセクションまたはフィールド（件名行、ヘッダー、本文コピーなど）をダブルクリックし、必要に応じて編集します。
* **バリアントのセクションを [ 再生成](/help/user-guide/create/manage-variants.md#re-generate-sections)** するには、編集可能なテキストフィールドをクリックし、使用可能なオプションを使用して、新しいテキストのフレーズ変更、短縮、延長または生成を行います。
* **広告のサイズと縦横比を [ 変更](/help/user-guide/create/manage-variants.md#change-aspect-ratio)** するには、_[!UICONTROL サイズ変更]_ ボタン（キャンバスの左側にボタンアイコンが表示されたボックス）をクリックし、すべてのバリアントに適用する新しいサイズと縦横比を選択します。 バリアントが複製され、サイズが変更されます。
* **画像を [ 切り抜きまたは再配置](/help/user-guide/create/manage-variants.md#crop-assets)** するには、画像の上にマウスポインターを置き、表示される切り抜きアイコンをクリックし、画像のサイズと配置を調整します。 「**[!UICONTROL 適用]**」をクリックします。

<!-- # Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

## 生成フィードバックを送信

生成出力の品質に関する [ フィードバックを送信 ](/help/user-guide/create/manage-variants.md#generation-feedback) するには、オプションアイコン（3 つのドット）をクリックし、**[!UICONTROL 良好な出力]** または **[!UICONTROL 不良な出力]** を選択します。

## ブランドの整合性の確認

生成される広告を最適化し、ブランドアイデンティティに厳密に準拠するには、[_ブランド検証パネル_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) の機能を活用します。このパネルは、包括的なブランド検証の詳細を表示し、改善点を明確にします。

**ブランドの整合性を検証するには**:

1. 上部メニューバーのブランド検証アイコンをクリックして、[_ブランド検証パネル_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) を開きます。 改善が必要なフラグメントとガイドラインの詳細を確認できます。

1. 各広告を切り替えて、生成されたコンテンツを改善してブランドに合わせる方法を確認します。
1. [ 手動で広告を改訂 ](#revise-generated-display-ads) し、メールがブランドと密接に連携するようにします。

[ ブランド検証 ](/help/user-guide/guidelines/brand-validation.md) を参照してください。

## レビューと承認の取得

キャンバスの上部のメニューバーからアクセスできる承認パネルを使用して、レビューを取得、レビューコメントを追跡、関係者からの承認を取得します。

**レビューと承認を取得するには**:

1. [ ドラフトのメールエクスペリエンスの承認 ](/help/user-guide/approvals/request-review.md) を依頼する [ 承認リクエストの開始 ](/help/user-guide/approvals/approve-content.md)。
1. レビュープロセス中に [ レビュー担当者を削除または追加 ](/help/user-guide/approvals/review-and-edit.md#manage-approvals) できます。
1. [ レビュー用にコンテンツにアクセス ](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) し、修正要求を表示します。
1. レビューのコメントごとにドラフトを編集し、[ ディスプレイ広告エクスペリエンスを公開する ](#publish-and-export-experience) ようにします。

[ レビューと承認 ](/help/user-guide/approvals/overview.md) を参照してください。

## Publishと書き出しの経験

生成したディスプレイ広告を現在および将来の使用で使用できるようにするには、[!UICONTROL  コンテンツ ] に公開し、マーケティングキャンペーンで使用するために書き出します。

1. **新しいディスプレイ広告エクスペリエンスを公開するには** 上部のツールバーまたは承認フロー内の **[!UICONTROL Publish]** をクリックします。
   1. 「_[!UICONTROL [!DNL Campaigns]]_」を選択し、必要に応じて_[!UICONTROL  詳細 ]_を追加します。
   1. 「**[!UICONTROL 公開する]**」をクリックします。

      ![ ディスプレイ広告をPublish](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **新しいディスプレイ広告エクスペリエンスを書き出すには**、上部のツールバーにある **[!UICONTROL 書き出し]** をクリックします。
   1. フォーマット（HTMLと画像、PNG、JPG）を選択し、「**[!UICONTROL エクスポート]**」をクリックします。

      書き出されたHTMLは、テンプレートや `div` コンテナなど、事前に定義された web プロパティ内に配置する必要があります。 これらのサイズを設定しないと、個別に表示した場合に画像がゆがんで見えることがあります。

詳しくは、[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) を参照してください。
