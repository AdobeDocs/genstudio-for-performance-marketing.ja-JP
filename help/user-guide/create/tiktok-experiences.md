---
title: TikTokのエクスペリエンス
description: Adobe GenStudio for Performance MarketingでTikTokのフィード内ビデオ広告を作成、レビュー、公開、アクティブ化する方法について説明します。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
TQID: https://experienceleague.adobe.com/aK9mP2vR8xT4nW6yB1cF3hJ5kL7mN9pQ2rS4tU6vW8x
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2:
  - id: be495d08-ecd1-455f-951e-c22de504e667
  - id: dd48f9df-f2e2-49fe-a918-332a8e240ffe
  - id: dee4e9a9-78d1-4953-8179-f8da6117027d
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
  - id: f54ee13b-9545-4d68-9842-a12026e60aaf
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 5f02a3076ca875f9819e5da55824bbf9c5337bb4
workflow-type: tm+mt
source-wordcount: 896
ht-degree: 100%

---

# TikTok エクスペリエンス

[!DNL GenStudio for Performance Marketing] を使用すると、[[!DNL Create]](/help/user-guide/create/overview.md) ワークフローでTikTok広告を有料メディアエクスペリエンスとして作成できます。 クリエイティブバリアントを生成し、ブランドとチャネルのチェックを実行し、[!DNL Content] に公開し、[[!DNL Activate]](/help/user-guide/activation/overview.md) を通じてアクティブ化して、コンテンツをTikTok Ads Manager に配信して最終的なレビューとローンチを行います。

[!DNL GenStudio for Performance Marketing] のTikTokは、より広範なオムニチャネルワークフローに適合します。個別のレポートツールに切り替える代わりに、他のソーシャルチャネルやディスプレイチャネル（Metaや LinkedIn など）と並行して、[[!DNL Insights]](/help/user-guide/insights/overview.md) でTikTok キャンペーンや広告のパフォーマンスを分析できます。

次 [!DNL Insights] ような指標を表示できます。

* インプレッション
* クリック数
* クリックスルー率（CTR）
* クリック単価（CPC）
* 獲得あたりのコスト（CPA）
* マイルあたりのコスト （CPM）
* 費用

結果を確認し、クリエイティブの有効性を比較し、ターゲティングと予算をすべて 1 か所で調整します。 毎日のデータ更新により、[!DNL GenStudio for Performance Marketing] ータを離れることなく、より迅速に最適化できます。

## 前提条件

TikTok広告を作成またはアクティブ化する前に、次の手順を実行します。

### アクセスと役割

GenStudio for Performance Marketingに **編集者** 以上の役割があることを確認します。 [ ユーザーの役割と権限 ](/help/user-guide/user-roles.md) を参照してください。

### TikTok Ads アカウントを接続

1. **[!UICONTROL 設定]** / **[!UICONTROL TikTok]** / **[!UICONTROL 管理]** / **[!UICONTROL アカウントを追加]** に移動します。
1. ポップアップで、TikTok Ads Manager にログインします。
1. 広告アカウントに対する **オペレーター** または **管理者** アクセス権があることを確認します。
1. TikTokをチャネルとして追加し、TikTok Ads Manager への OAuth ログインを完了します。

### 設定をアクティベート

System Manager が [!DNL Activate] のTikTok Ads アカウントに接続しました：

* 少なくとも 1 つのTikTok広告アカウントが使用に対して有効になっています。

### 設定の作成

* [ ブランド、製品、ペルソナ ](/help/user-guide/guidelines/overview.md) は、アプリがブランド上のコピーとレイアウトを生成できるように設定されます。
* 1 つ以上のTikTok テンプレートがアップロードされています。 Adobeでは、フィード内に配置するために最適化され、アスペクト比が **9:16** で、上部と下部の UI にセーフゾーンが付いた、TikTokの縦向きビデオテンプレートをお勧めします。
* ビデオが [!DNL Content] にアップロードされています。

## TikTokのフィード内広告の生成

### TikTok エクスペリエンスの開始

![ 作成ワークフローのTikTok チャネル ](../../assets/tiktok/create-tiktok-experience.png){width="90%"}
**TikTok エクスペリエンスを開始するには**:

1. **[!UICONTROL 作成]** に移動し、「**[!UICONTROL TikTok]**」を選択します。
1. TikTok テンプレートを選択して、「**[!UICONTROL 使用]**」をクリックします。
1. キャンバスで、「**[!UICONTROL ブランド]**」、「**[!UICONTROL 製品]**」、「**[!UICONTROL ペルソナ]**」および「**[!UICONTROL 言語]**」を選択します。
1. [!DNL Content] からビデオを選択します。
1. TikTokのヘッドラインのコピーを入力するプロンプトを入力します。
1. 「**[!UICONTROL 生成]**」をクリックします。
   ![Tiktok キャンバス コントロールの作成 ](../../assets/tiktok/tiktok-prompt.png){width="40%"}

GenStudio for Performance Marketingでは、4 つのクリエイティブのバリアントが生成されます。

実行できる操作：

* トーン、長さ、強調を調整するには、**[!UICONTROL 再生成]** または **[!UICONTROL リファイン]** を使用します。
* キャンバス内でテキストを直接編集します。
* **[!UICONTROL スワップ]** を使用して、[!DNL Content] から代替ビデオを選択します。
* **[!UICONTROL 9:16** フレーム内のビデオのレイアウトを調整するには、**[!UICONTROL 切り抜き]** または **再フレーム]** を使用します。

### ブランドチェックとチャネルチェックの実行

レビュー用にエクスペリエンスを保存または送信する前に、コンテンツチェックを実行します。

1. **[!UICONTROL コンテンツチェック]** （ブランドチェックとチャネルチェック）をクリックします。
1. 検証結果のレビュー：
   * **ブランドガイドライン** - トーン、制限付き用語、ロゴの使用。
   * **TikTok チャネルルール** – 縦横比、ファイルタイプ、長さをコピー。
1. フラグの付いた問題（長さのコピーや複雑なオンスクリーンテキストなど）を解決します。

コンテンツのチェックについて詳しくは、[ ブランドの検証 ](/help/user-guide/guidelines/brand-validation.md) を参照してください。

## GenStudio for Performance MarketingでのTikTok広告の保存

TikTokのエクスペリエンスを [!DNL Content] ライブラリに移動して、レビュー、再利用、アクティブ化できるようにします。
次の 2 つの状態があります。

* **ドラフトエクスペリエンス** – 処理中の作業で、承認されていません。
* **公開済みのエクスペリエンス** - コンテンツが承認され、アクティベーション用に [!DNL Content] で使用できるようになりました。

### レビュー用に送信

**レビュー用に送信するには**:

1. **[!DNL Experience]** ヘッダーで、「**[!UICONTROL レビューをリクエスト]**」をクリックします。
1. 承認者（ブランド、法務、パフォーマンスなど）を選択します。
   * （任意）「**[!UICONTROL 設定]**」にメモを追加します。
1. **[!UICONTROL レビュー用に送信]** をクリックします。

承認者は、ビデオのプレビュー、説明およびcall to action（CTA）と、ブランドおよびチャネルのチェック結果を表示できます。 レビュー担当者は、エクスペリエンスを承認したり、変更をリクエストしたりできます。

### [!DNL Content] に公開

すべての必要な承認後：

1. **[!UICONTROL コンテンツに公開]** をクリックします。
1. メタデータを確認：
   * キャンペーン名またはアクティブ化名
   * 地域，言語，ペルソナ，funnel ステージ
   * チャンネル：TikTok
1. 「**[!UICONTROL 公開する]**」をクリックします。

TikTok広告が [!DNL Content] に表示されます。 [!DNL Channel] や [!DNL Campaign] などのフィルターを使用して検出でき、[!DNL Activate] で選択する準備が整いました。

## TikTok広告のアクティブ化

TikTok アクティベーションでは、Metaおよび Campaign Manager 360 （CM360）と同じ [!DNL Activate] モジュールを使用します。 [!DNL Content] ワークフローまたは [!DNL Activate] ワークフローから開始できます。

**TikTokのアクティベーションを開始するには**:

1. TikTok チャネルタイルを開きます。
1. **[!UICONTROL アクティベーションを作成]** をクリックします。
1. [!DNL Content] から 1 つ以上の公開済みTikTok エクスペリエンスを選択します。

通常、各エクスペリエンスは 1 つのTikTok広告に 1 つ以上のビデオバリアントをマッピングします。

### エクスペリエンス設定の指定

選択した各エクスペリエンスに対して、次の内容を確認します。

* プライマリテキスト
* Call to action
* 宛先 URL

### プラットフォーム設定の指定

次のようなTikTok Ads Manager の詳細を指定します。

* TikTok広告アカウント
* Campaign
* 広告グループ
* 広告名（TikTok広告ごとに 1 つ）

### レビューと公開

1. クリエイティブおよびプラットフォームの詳細をすべて確認します。
1. 「**[!UICONTROL 公開する]**」をクリックします。

GenStudio for Performance Marketingが、一時停止またはドラフトの状態でTikTok Ads Manager に広告をプッシュします。

### 次の手順

_公開中_ モーダルが表示され、自動的に閉じます。 TikTokのアクティベーションテーブルにリダイレクトされます。

![GenStudio公開モーダル ](../../assets/tiktok/publishing-modal.png){width="30%"}

アクティベーションテーブルには、最新のアクティベートが、処理中のステータスが **保留中** で表示されます。公開中に移動できます。

![TikTok詳細ページ ](../../assets/tiktok/tiktok-details-page.png){width="90%"}

完了すると、確認ポップアップに成功または失敗のメッセージが表示されます。 そのポップアップをクリックするか、アクティベーションテーブルのTikTok アクティベーションをクリックすると、**詳細** ページが開きます。 **詳細** ページには、アクティベーション情報の完全な情報と、TikTok Ads Manager で公開された広告へのディープリンクが含まれています。

アクティベーションに失敗した場合は、TikTokからのエラーメッセージと共に **失敗** ステータスが表示されます。

TikTok Ads Manager では、メディアチームは次のことができます。

* 最終チェックを実行します。
* 広告または広告グループをライブにします。

他のチャネルと同様に、GenStudio for Performance Marketingはクリエイティブを非アクティブな状態で配信するので、チャネルの所有者が最終的なローンチのタイミングと予算を制御できます。
