---
title: AI アシスタントツールリファレンス
description: AI アシスタントが[!DNL GenStudio for Performance Marketing]で使用できるインサイトの作成、計画、有効化、およびフィードバック ツールについて説明します。
role: User
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 244293cf4f83acbc252f1d5f3495db403ed4a9bb
workflow-type: tm+mt
source-wordcount: '2265'
ht-degree: 13%
---

# AI アシスタントツールリファレンス

このリファレンスでは、接続されたAI アシスタントが[!DNL GenStudio for Performance Marketing]で使用できるツールについて説明します。 使用可能なツールリストは、組織の設定によって異なります。

ワークフローを開始する前に、AI アシスタントにどのツールにアクセスできるかを尋ねましょう。

## 機能エリア

| 面グラフ | 目的 | 動作 |
|---|---|---|
| Insights | 有料メディアやメールのパフォーマンスをクエリし、クリエイティブなレコメンデーションを取得できます。 | 読み取り専用： |
| 作成 | アセットを検索し、Adobe Expressのテンプレートやインサイトのレコメンデーションからドラフトを作成して、レビューを管理できます。 | 読み取りと書き込み： Creative Cloudでドキュメントを作成します。 |
| プラン | 概要から施策の詳細を抽出し、Workfront Planningに保存できます。 | 抽出は読み取り専用です。 保存すると、Workfront Planningでレコードが作成され、自動的にロールバックできません。 |
| アクティブ化 | 公開ターゲットを解決し、承認されたエクスペリエンスをプラットフォームに送信します。 | 書く： 広告はプラットフォームに送信され、オフ状態で公開されます。 個別にオンにします。 これらのツールで元に戻すことはできません。 |
| フィードバック | 製品フィードバックを[!DNL GenStudio for Performance Marketing] チームに送信します。 | 書く： |

ほとんどのインサイトツールは、`meta`、`linkedin`および`innovid`をカバーしています。 指標値ツールは、`meta`と`linkedin`をカバーしています。 メールキャンペーンのレポートでは、Adobe Journey Optimizer （`ajo`）とAdobe Campaign （`acc`）が対象となります。

作成では、`meta`、`linkedin`、`display`、`tiktok`、`youtube`がサポートされています。 アクティブ化は、`META`、`LINKEDIN`、`GOOGLECM360`をサポートしています。

## インサイトツール

### get_insights_capabilities

組織で有効になっているインサイトチャネルとレポート操作を返します。 利用可能性が不明な場合は、まずこのツールを使用してください。 サポートされているチャネルは、`meta`、`linkedin`、`innovid`、`ajo`および`acc`です。

このツールは、キャンペーン、広告、指標の値ではなく、機能のメタデータを返します。 組織のカスタム指標キーを検索するには、`list_connected_channels_and_metrics`を使用します。

### list_connected_channels_and_metrics

組織のアクティブなMeta、LinkedIn、Google Campaign Manager 360の接続、サポートされているインサイトチャネルと操作、設定されたカスタムコンバージョン指標を返します。 `get_insights_metric_values`を呼び出す前に指標キーを検索する場合に使用します。

このツールは、指標の値ではなく、指標キー、ラベル、形式を返します。 接続は、履歴レポートデータが利用可能であることを保証しません。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `limit`, `offset` | いいえ | ページサイズとページオフセット。 両方を省略して、カタログ全体を返します。 |

### get_insights_summary

選択した日付範囲の1つのチャネルの見出しのパフォーマンス指標と傾向を返します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channel` | はい | `meta`、`linkedin`または`innovid`。 |
| `startDate` | いいえ | 開始日は`YYYY-MM-DD`形式です。 デフォルトは30日前です。 |
| `endDate` | いいえ | 終了日：`YYYY-MM-DD`形式 デフォルトは今日です。 |
| `metrics` | いいえ | グラフへの指標：`spend`、`ctr`、`cpc`、`cpm`、`cpa`、`impressions`、`clicks`、`conversions`、`videoPlays`、`engagement`、`likes`、`comments`、または`shares`。 デフォルトは`spend`、`ctr`、`cpc`、`cpm`です。 |

### list_insights_campaigns

キャンペーンパフォーマンス指標と合計行の並べ替え可能なテーブルを返します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channel` | はい | `meta`、`linkedin`または`innovid`。 |
| `startDate`, `endDate` | いいえ | 日付範囲は`YYYY-MM-DD`形式です。 デフォルトは過去30日間です。 |
| `search` | いいえ | キャンペーン名フィルター： |
| `sortBy` | いいえ | 並べ替えフィールド：`spend`、`impressions`、`clicks`、`ctr`、`cpc`、`cpm`、または`name`。 デフォルトは、`spend` です。 結果は常に降順で並べ替えられます。 |
| `limit`, `offset` | いいえ | ページサイズとページオフセット。 デフォルトのページサイズは20です。 |

### list_insights_email_campaigns

Adobe Journey OptimizerとAdobe Campaignの配信とエンゲージメントの指標を含むメールキャンペーンの並べ替え可能なテーブルを返します。 広告キャンペーンの場合は、`list_insights_campaigns`を使用してください。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channel` | はい | `ajo`または`acc`。 |
| `startDate`, `endDate` | いいえ | 日付範囲は`YYYY-MM-DD`形式です。 デフォルトは、終了日の前の過去30日間です。 |
| `search` | いいえ | キャンペーン名フィルター： |
| `sortBy` | いいえ | 並べ替えフィールド：`campaignName`、`emailsNumber`、`emailsDelivered`、`totalClicks`、`openRate`、`ctr`、`ctor`、`bounceRate`、`unsubscribeRate`または`spamComplaintRate`。 デフォルトは、`emailsDelivered` です。 結果は常に降順で並べ替えられます。 |
| `limit`, `offset` | いいえ | ページサイズとページオフセット。 |

### list_insights_ads

広告レベルのパフォーマンスを返します。 並べ替え可能なテーブルにはデフォルトの参照モードを使用し、パフォーマンスの高い広告と低い広告には階層モードを使用します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channel` | はい | `meta`、`linkedin`または`innovid`。 |
| `tier` | いいえ | `all`、`high`または`low`。 デフォルトは、`all` です。 |
| `mainMetric` | いいえ | `high`または`low`階層モードのランキング指標：`ctr`、`cpc`、`cpm`、`cpa`、`spend`、`impressions`、または`clicks`。 参照モードでは無視されます。 |
| `metrics` | いいえ | 階層モードで各広告についてレポートする追加指標。 |
| `campaigns` | いいえ | キャンペーンは、結果を最大50に制限するために使用されます。 各キャンペーンには、`channel`、`accountId`および`campaignId`が含まれます。 |
| `search` | いいえ | 広告名フィルター： |
| `sortBy` | いいえ | モードの並べ替えフィールドを参照：`spend`、`impressions`、`clicks`、`ctr`、`cpc`、`cpm`、または`name`。 デフォルトは、`spend` です。 結果は常に降順で並べ替えられます。 |
| `spendMin`, `spendMax` | いいえ | 各広告の総支出額。 階層モードのみ。 |
| `includeUnsupported` | いいえ | クリエイティブをレンダリングできない広告が含まれます。 デフォルトは、`false` です。 |
| `startDate`, `endDate` | いいえ | 日付範囲は`YYYY-MM-DD`形式です。 |
| `limit`, `offset` | いいえ | ページサイズとページオフセット。 |

階層モードは、`get_insights_ad_attributes`が必要とする広告識別子を返します。

### get_insights_ad_details

コピー、call to action、アセット、プレースメントなど、1つの広告のクリエイティブメタデータを返します。 パフォーマンス指標は返されません。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channel` | はい | `meta`、`linkedin`または`innovid`。 |
| `accountId` | はい | 有料メディアアカウントのID。 |
| `campaignId` | はい | キャンペーン ID: |
| `adId` | はい | 広告ID: |
| `adgroupId` | いいえ | チャネルで広告グループを使用する場合の広告グループの識別子。 |

### get_insights_ad_attributes

選択した広告のクリエイティブ特性をチャネル平均と比較します。 `list_insights_ads`がパフォーマンスの高い広告または低い広告を識別した後に使用します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `ads` | はい | 1から200件の広告を表示します。 各広告には、`channel`、`accountId`、`campaignId`、および`adId`、オプションで`adGroupId`および`performanceTier` （`high`または`low`）が含まれます。 `list_insights_ads`から返された識別子を階層モードで使用します。 |
| `mainMetric` | はい | 広告のランク付けに使用される指標：`ctr`、`cpc`、`cpm`、`cpa`、`spend`、`impressions`、または`clicks`。 |
| `campaigns` | いいえ | 比較母集団を定義するために使用されるキャンペーン（最大50）。 各キャンペーンには、`channel`、`accountId`および`campaignId`が含まれます。 |
| `spendMin`, `spendMax` | いいえ | 比較母集団に対する支出の境界。 |
| `startDate`, `endDate` | いいえ | 日付範囲は`YYYY-MM-DD`形式です。 |

### get_insights_tag_categories

リクエストされた期間に組織で使用可能なタグカテゴリを返します。 パフォーマンス指標ではなく、カテゴリ名を返します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channels` | はい | 1つ以上のサポートされているチャネル。 |
| `startDate`, `endDate` | いいえ | 日付範囲は`YYYY-MM-DD`形式です。 |

### get_insights_ad_tags

製品、地域、クリエイティブテーマなど、1つのカテゴリ内のタグ値でパフォーマンスを返します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channel` | はい | `meta`、`linkedin`または`innovid`。 |
| `tagCategory` | はい | `get_insights_tag_categories`様がカテゴリを返しました。 |
| `tagSource` | いいえ | `ad_tags`または`campaign_tags`。 デフォルトは、`ad_tags` です。 |
| `sortBy` | いいえ | 並べ替えフィールド：`adsCount`、`spend`、`impressions`、`clicks`、`conversionCount`、`ctr`、`cpc`、`cpm`または`cpa`。 デフォルトは、`adsCount` です。 |
| `search` | いいえ | タグ値フィルター： |
| `startDate`, `endDate` | いいえ | 日付範囲は`YYYY-MM-DD`形式です。 |
| `limit`, `offset` | いいえ | ページサイズとページオフセット。 |

### get_insights_metric_values

MetaとLinkedInに対して、見込み顧客や登録数、広告費用対効果など、追跡された組織の指標の値とトレンドを返します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channels` | いいえ | `meta`、`linkedin`、またはその両方。 |
| `metrics` | いいえ | `list_connected_channels_and_metrics`が返すメトリック キーは最大20個です。 デフォルトは、組織のデフォルトの表示セットです。 |
| `campaigns` | いいえ | キャンペーンは、結果を最大50に制限するために使用されます。 各キャンペーンには、`channel`、`accountId`および`campaignId`が含まれます。 |
| `startDate`, `endDate` | いいえ | 日付範囲は`YYYY-MM-DD`形式です。 デフォルトは過去30日間です。 |

### get_insights_recommendations

組織のパフォーマンスデータに基づいて提案されたクリエイティブの変更を返します。 選択したスコープに適格な広告が含まれていない場合、リクエストは推奨事項を返すことができません。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channels` | はい | `meta`、`linkedin`、または`innovid`の1つ以上。 |
| `campaigns` | いいえ | キャンペーンは、結果を最大50に制限するために使用されます。 各キャンペーンには、`channel`、`accountId`および`campaignId`が含まれます。 |
| `search` | いいえ | キャンペーン名フィルター： |
| `recommendationId` | いいえ | 1つのレコメンデーションの`adUid`は、詳細な取得に使用されます。 |
| `onlyWithPreview` | いいえ | サンプルのクリエイティブプレビューがないレコメンデーションを除外します。 デフォルトは、`true` です。 |
| `limit`, `offset` | いいえ | ページサイズとページオフセット。 |

## ツールの作成

エクスペリエンスのアクティベーションに進む前に、ツールを作成してアセットを検索し、Adobe Expressテンプレートからドラフトを作成して、レビューを管理できます。

### list_express_templates

フィルターとファセット数を含む利用可能なExpress テンプレートを一覧表示します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channel` | いいえ | `meta`、`display`、`linkedin`、`tiktok`、`youtube`または`__unspecified__`。 |
| `query` | いいえ | テンプレートの検索語。 |
| `activatableMimeType`, `aspectRatios`, `externalTemplateSource`, `isHTML5Template`, `keywords`, `languages`, `mediaFormat`, `regions`, `timeframes` | いいえ | テンプレートファセットフィルター： |
| `sortBy` | いいえ | `modified`または`created`。 デフォルトは、`modified` です。 |
| `order` | いいえ | `asc`または`desc`。 デフォルトは、`desc` です。 |
| `limit`, `offset` | いいえ | ページサイズとページオフセット。 |

### describe_express_template

テンプレート内の編集可能なテキストフィールドと画像の配置を返します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `templateId` | はい | Express テンプレート ID。 |

### list_cta_options

チャネルで許可されているcall-to-action値を返します。 Displayは自由形式のテキストを受け入れるので、空のリストを返します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channel` | はい | `linkedin`、`meta`、`display`、`tiktok`または`youtube`。 |
| `limit`, `offset` | いいえ | ページサイズとページオフセット。 両方を省略して、すべてのオプションを返します。 |

### search_assets

GenStudio コンテンツ内の画像とビデオを検索します。 ドラフトの既存のアセットを選択する場合に使用します。 派生アセット、外部アセット、期限切れのアセットは除外されます。 このツールは、アセットをアップロード、編集、削除、生成することはなく、GenStudio コンテンツの使用権限が必要です。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `query` | いいえ | アセットのメタデータをまたいだキーワードまたは自然言語検索。 |
| `mediaTypes` | いいえ | `image`、`video`、またはその両方。 デフォルトでは、両方が含まれます。 |
| `aspectRatios` | いいえ | `1:1`や`16:9`などの縦横比。 比率が使用できない場合、ツールは使用可能な選択肢を返します。 |
| `brands`, `campaigns`, `products`, `personas`, `channels` | いいえ | 名前でフィルター。 |
| `customMetadata` | いいえ | 1つ以上の値を持つ、最大5つのメタデータフィールド。 |
| `uploadedBy` | いいえ | `me`またはアップローダーの電子メールアドレス。 |
| `createdAtFrom`, `createdAtTo` | いいえ | ISO 8601形式の作成時間の境界。 |
| `aiGenerated` | いいえ | AI生成のステータス別にフィルタリング。 |
| `contentCredentials` | いいえ | Content Credentialsのステータス別にフィルタリングします。 |
| `limit`, `offset` | いいえ | ページサイズとページオフセット。 |

この結果には、`create_draft`と有効期間が短い署名済みURLの安定したアセット参照が含まれます。

### create_draft

1つ以上のエクスペリエンスを含むExpress テンプレートから編集可能なドラフトを作成します。 各呼び出しによって新しいドラフトが作成されます。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `templateId` | はい | Express テンプレート ID。 |
| `prompt` | はい | Creativeの概要とコピーの手順がドラフトに保存されます。 |
| `experiences` | はい | 1つ以上のエクスペリエンス： 次の表を参照してください。 |
| `name` | いいえ | ドキュメント名。 |
| `allowAssetReuse` | いいえ | 選択した1つのアセットを複数のエクスペリエンスで再利用できます。 デフォルトは、`false` です。 |

各エクスペリエンスはこれらのフィールドをサポートします。

| フィールド | 必須 | 説明 |
|---|---|---|
| `channel` | はい | `linkedin`、`meta`、`display`、`tiktok`または`youtube`。 |
| `title` | いいえ | エクスペリエンスのタイトル： デフォルトは「概念&#x200B;*n*」です。 |
| `headline` | MetaとLinkedIn | プライマリの見出し： |
| `body` | Meta、LinkedIn、TikTok | 本文のコピー： LinkedInの場合、これは紹介テキストです。 TikTokの場合、これはプライマリテキストです。 |
| `description` | YouTube | 広告の説明： MetaとLinkedInではオプションです。 |
| `display_url` | MetaとLinkedIn | 広告に表示されるURLを表示します。 |
| `destination_url` | いいえ | 広告がリンクするURL。 |
| `cta` | いいえ | `list_cta_options`からのCall-to-action テキスト。 |
| `templateFields` | いいえ | `describe_express_template`の名前付きテンプレート要素の上書き。 各オーバーライドは、テキスト、ディメンションを含む画像URL、またはビデオ URLを設定します。 |
| `assetTemplateFields` | いいえ | テンプレート内の画像またはビデオフィールドの`search_assets`からのコンテンツアセット。 |

固定されたcall-to-action値を持つチャネルのドラフトを作成する前に、`list_cta_options`を使用してください。

### create_draft_from_recommendation

特定のインサイトのレコメンデーションから編集可能なドラフトを作成します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channel` | はい | `meta`または`linkedin`。 |
| `adUid` | はい | `get_insights_recommendations`様がレコメンデーション IDを返しました。 |
| `prompt` | はい | 提案にもとづいたCreativeの概要を作成できます。 |
| `name` | いいえ | ドキュメント名。 |

### list_recent_drafts

最近のExpress テンプレートのドラフトと、そのステータスとリンクを一覧表示します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `limit`, `offset` | いいえ | ページサイズとページオフセット。 |

### get_draft_metadata

ドラフトの名前、チャネル、承認ステータス、レビュー担当者の結果、共同作業者のアクセスを返します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `draftId` | はい | ドラフトアセットのID: |

### share_draft

承認を依頼することなく、共同作業者がドラフトを表示または編集できるようにします。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `draftId` | はい | ドラフトアセットのID: |
| `emails` | はい | 1人から20人の共同作業者のメールアドレス。 |
| `role` | はい | `editor`または`viewer`。 |
| `message` | いいえ | 招待メッセージ。 |

### request_draft_approval

ドラフトを1人以上の関係者に送信して承認を得る。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `draftId` | はい | ドラフトアセットのID: |
| `emails` | はい | 1人から20人のレビュアーのメールアドレス。 |

### list_experiences

承認済みの公開されたエクスペリエンスを返し、アクティベートする準備が整います。 ドラフトは含まれません。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channel` | いいえ | `email`、`meta`、`meta_organic`、`display`、`ctv`、`linkedin`、`linkedin_organic`、`tiktok`、`chatgpt`または`youtube`。 |
| `createdByMe` | いいえ | 結果は、現在のユーザーが作成したエクスペリエンスに限定されます。 |
| `campaignNames` | いいえ | キャンペーン名フィルターを最大5つまで指定できます。 |
| `creatorEmail` | いいえ | 作成者のメールフィルター： |
| `createdAtFrom`, `createdAtTo` | いいえ | 作成日の制限： |
| `language` | いいえ | BCP 47言語タグ。 |
| `limit`, `cursor` | いいえ | ページサイズ（1 ～ 50、デフォルト 20）とページネーションカーソル。 |

## プランツール

プランツールは、キャンペーン概要をレビュー可能なキャンペーンドラフトに変換し、Workfront Planningに保存できます。

### extract_campaign_from_brief

貼り付けられたマーケティングブリーフから、レビュー可能なキャンペーンドラフトを抽出します。 このツールはレコードを保存しません。 欠落している事実と日付は推測されません。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `briefText` | はい | 1つのキャンペーン概要の完全なプレーンテキスト（最大100,000文字）。 ファイルとリンクはサポートされていません。 |

その結果には、キャンペーンのドラフト、関連見積もりを含む調査結果、推奨オーディエンス、警告が含まれます。

### create_workfront_campaign

レビューして承認したドラフトから、リンクされた製品とペルソナを含むWorkfront計画キャンペーンを作成します。 このツールは無効であり、レコードを自動的にロールバックすることはできません。 成功した可能性のある書き込みを再試行する前に、Workfrontを調べます。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `campaignDraft` | はい | 承認済みのドラフト。 `name`が必要です。 オプションのフィールドは、`description`、`objective`、`keyMessaging`、`startDate`、`endDate` （`YYYY-MM-DD`）、`status`、`channels`、`products`および`personas`です。 |
| `channelSelections` | いいえ | あいまいなチャネル名の使用は承認済み。 |
| `entitySelections` | いいえ | 既存製品とペルソナのレコードを承認。 `null`を使用して新しいレコードをリクエストします。 |
| `createMissingEntities` | いいえ | 新しい商品として選択した商品とペルソナを作成します。 デフォルトは、`false` です。 |

製品、ペルソナ、チャネルが曖昧な場合、確認するための選択肢が返され、変更は行われません。

## ツールを有効化

ツールをアクティベートして有料メディアターゲットを解決し、承認されたエクスペリエンスをプラットフォームに送信します。 広告はオフ状態（Metaが一時停止、LinkedIn ドラフト、Campaign Manager 360が非アクティブ）で公開されるので、配信する前に個別にオンにする必要があります。 これらのツールを通じて広告をプラットフォームに送信することは元に戻すことができません。

### configure_activation_target

必要に応じて、有料メディアアカウント、キャンペーン、広告セット、およびFacebook ページを解決して検証します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `platform` | はい | `META`、`LINKEDIN`または`GOOGLECM360`。 |
| `platformAccountId` | いいえ | 有料メディアアカウントのID。 アカウントの発見は省略します。 |
| `campaignId` | いいえ | MetaまたはLinkedInのキャンペーン ID。 Campaign Manager 360には使用されません。 |
| `adsetId` | いいえ | Metaの広告セット、またはLinkedInのキャンペーン ID。 Campaign Manager 360には使用されません。 |
| `pageId` | いいえ | MetaのFacebook ページ ID。 |

Campaign Manager 360では、広告アカウントのみが必要です。

### create_activation

検証済みのターゲットを使用して、承認されたエクスペリエンスを広告としてプラットフォームに送信します。 広告はオフ状態で公開されます。 Metaでは、各縦横比の最初の画像を含む広告が1つ作成されます。 LinkedInとCampaign Manager 360は、解決された画像ごとに1つの広告を作成します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `platform` | はい | `META`、`LINKEDIN`または`GOOGLECM360`。 |
| `targetId` | はい | `configure_activation_target`様が検証済みのターゲットを返しました。 |
| `experienceId` | はい | `list_experiences`さんが承認済みのエクスペリエンス IDを返しました。 |
| `name` | いいえ | 広告プレースメント表示名。 デフォルトは、エクスペリエンスの広告タイトルです。 |

結果には、作成、キュー、スキップされた広告の数が一覧表示され、各広告の初期ステータスと[!DNL GenStudio for Performance Marketing]へのリンクが表示されます。 `PENDING`のステータスは、ジョブがキューに入っていることを意味します。ただし、広告が配信しているわけではありません。

`create_activation`を2回呼び出すと、最初の広告を更新する代わりに、追加の広告が作成されます。

## フィードバックツール

### submit_mcp_feedback

ツールまたはワークフローに関するフィードバックを[!DNL GenStudio for Performance Marketing] チームに送信します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `category` | はい | `bug`、`feature_request`または`workflow_friction`。 |
| `comment` | はい | フィードバックの簡潔な説明。 |
| `tags` | いいえ | フィードバックを分類するために使用されるタグ。 |
| `tool_name` | いいえ | フィードバックに関連付けられたツール。 |

## 共通ワークフロー

あるツールが別のツールに識別子または設定を提供する場合は、これらのシーケンスを使用します。

- **広告を診断：** `high`または`low`階層モードで`list_insights_ads`を呼び出してから、同じランキング指標で`get_insights_ad_attributes`を呼び出します。
- **タグで分析：** `get_insights_tag_categories`を呼び出してから、返されたカテゴリで`get_insights_ad_tags`を呼び出します。
- **追跡された指標を確認：**&#x200B;呼び出し`list_connected_channels_and_metrics`、返された指標キーを使用して`get_insights_metric_values`を呼び出します。
- **レコメンデーションをドラフトに変換：** `get_insights_recommendations`に電話してから`create_draft_from_recommendation`に電話してください。
- **テンプレートからビルド：** `list_express_templates`、`describe_express_template`、`list_cta_options`を呼び出してから`create_draft`を呼び出します。
- **既存のアセットからビルド：** `search_assets`を呼び出してから、返されたアセット参照を`assetTemplateFields`の`create_draft`に渡します。
- **キャンペーン概要をWorkfrontに保存します：** `extract_campaign_from_brief`に連絡し、ドラフトを確認してから`create_workfront_campaign`に連絡します。
- **承認されたエクスペリエンスをプラットフォームに送信します：** `list_experiences`に電話してから、`configure_activation_target`および`create_activation`に電話してください。

## 関連する機能

- [AI アシスタントの概要](overview.md)
- [AI アシスタントに接続する](connect-ai-assistants.md)
- [AI アシスタントの使用](use-ai-assistants.md)
