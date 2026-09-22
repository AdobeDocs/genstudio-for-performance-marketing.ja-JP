---
title: AI アシスタントツールリファレンス
description: AI アシスタントが[!DNL GenStudio for Performance Marketing]で使用できるインサイトの作成、アクティベート、およびフィードバックツールについて説明します。
role: User
source-git-commit: 6fb7ddb7549ea6bcd66b6139fbde9ebe12ddaa22
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 15%
---

# AI アシスタントツールリファレンス

このリファレンスでは、接続されたAI アシスタントが[!DNL GenStudio for Performance Marketing]で使用できるツールについて説明します。 使用可能なツールリストは、組織の設定によって異なります。

ワークフローを開始する前に、AI アシスタントにどのツールにアクセスできるかを尋ねましょう。

## 機能エリア

| 面グラフ | 目的 | 動作 |
|---|---|---|
| Insights | 有料メディアのパフォーマンスをクエリし、クリエイティブなレコメンデーションを取得できます。 | 読み取り専用： |
| 作成 | Express テンプレートやインサイトのレコメンデーションからドラフトを作成し、レビューを管理できます。 | 読み取りと書き込み： Creative Cloudでドキュメントを作成します。 |
| アクティブ化 | 公開ターゲットを解決し、承認済みエクスペリエンスを公開します。 | 書き込みと破壊。 ライブ広告を公開し、広告費を負担することができます。 |
| フィードバック | 製品フィードバックを[!DNL GenStudio for Performance Marketing] チームに送信します。 | 書く： |

ほとんどのインサイトツールは、`meta`、`linkedin`および`innovid`をカバーしています。 コンバージョン指標ツールは、`meta`と`linkedin`をカバーしています。

作成では、`meta`、`linkedin`、`display`、`tiktok`、`youtube`がサポートされています。 アクティブ化は、`META`、`LINKEDIN`、`GOOGLECM360`をサポートしています。

## インサイトツール

### get_insights_capabilities

組織で有効になっているインサイト チャネル、操作、およびカスタム コンバージョン指標を返します。 利用可能性が不明な場合は、まずこのツールを使用してください。

このツールは、キャンペーン、広告、指標の値ではなく、機能のメタデータを返します。

### get_insights_summary

選択した日付範囲の1つのチャネルの見出しのパフォーマンス指標と傾向を返します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channel` | はい | `meta`、`linkedin`または`innovid`。 |
| `startDate` | いいえ | 開始日は`YYYY-MM-DD`形式です。 デフォルトは30日前です。 |
| `endDate` | いいえ | 終了日：`YYYY-MM-DD`形式 デフォルトは今日です。 |
| `metrics` | いいえ | `spend`、`ctr`、`cpc`、`cpm`、`impressions`、`clicks`、または`conversions`などのグラフへの指標。 |

### list_insights_campaigns

キャンペーンパフォーマンス指標と合計行の並べ替え可能なテーブルを返します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channel` | はい | `meta`、`linkedin`または`innovid`。 |
| `startDate`, `endDate` | いいえ | 日付範囲は`YYYY-MM-DD`形式です。 デフォルトは過去30日間です。 |
| `search` | いいえ | キャンペーン名フィルター： |
| `sortBy` | いいえ | `spend`、`impressions`、`clicks`、`ctr`、`cpc`、`cpm`、または`name`などのフィールドを並べ替えます。 |
| `limit`, `offset` | いいえ | ページサイズとページオフセット。 |

### list_insights_ads

広告レベルのパフォーマンスを返します。 並べ替え可能なテーブルにはデフォルトの参照モードを使用し、パフォーマンスの高い広告と低い広告には階層モードを使用します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channel` | はい | `meta`、`linkedin`または`innovid`。 |
| `tier` | いいえ | `all`、`high`または`low`。 デフォルトは、`all` です。 |
| `mainMetric` | 条件 | `high`または`low`階層モードに必要なランキング指標。 |
| `campaigns` | いいえ | 結果を制限するために使用されるキャンペーン ID。 |
| `search` | いいえ | 広告名フィルター： |
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
| `ads` | はい | 説明する広告（`list_insights_ads`が返した識別子を含む）。 |
| `mainMetric` | はい | 広告のランク付けに使用される指標。 |
| `campaigns` | いいえ | 比較母集団の定義に使用されるキャンペーン ID。 |
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
| `tagSource` | いいえ | `ad_tags`または`campaign_tags`。 |
| `sortBy` | いいえ | 結果の並べ替えに使用される指標。 |
| `search` | いいえ | タグ値フィルター： |
| `startDate`, `endDate` | いいえ | 日付範囲は`YYYY-MM-DD`形式です。 |

### get_insights_custom_metrics

組織に設定されたカスタムコンバージョン指標を返します。 `get_insights_conversion_metrics`より前に使用してください。

このツールは、指標の値ではなく、指標の識別子を返します。

### get_insights_conversion_metrics

MetaおよびLinkedIn用に設定されたコンバージョン指標の値とトレンドを返します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channels` | いいえ | サポートされているコンバージョンチャネル： デフォルトは、`meta` です。 |
| `metrics` | いいえ | `get_insights_custom_metrics`が返した指標ID。 |
| `campaigns` | いいえ | 結果を制限するために使用されるキャンペーン ID。 |
| `startDate`, `endDate` | いいえ | 日付範囲は`YYYY-MM-DD`形式です。 |

### get_insights_recommendations

組織のパフォーマンスデータに基づいて提案されたクリエイティブの変更を返します。 選択したスコープに適格な広告が含まれていない場合、リクエストは推奨事項を返すことができません。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channels` | はい | 1つ以上のサポートされているチャネル。 |
| `campaigns` | いいえ | 結果を制限するために使用されるキャンペーン ID。 |
| `search` | いいえ | キャンペーン名フィルター： |
| `recommendationId` | いいえ | 1つの推奨事項を詳細に取得するために使用される識別子。 |
| `limit`, `offset` | いいえ | ページサイズとページオフセット。 |

## ツールの作成

ツールの作成Adobe Expressテンプレートからドラフトを作成し、エクスペリエンスがアクティベートされる前にレビューを管理できます。

### list_express_templates

フィルターとファセット数を含む利用可能なExpress テンプレートを一覧表示します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channel` | いいえ | `meta`、`display`、`linkedin`、`tiktok`、`youtube`または`__unspecified__`。 |
| `query` | いいえ | テンプレートの検索語。 |
| `aspectRatios`, `keywords`, `languages`, `mediaFormat`, `regions`, `timeframes` | いいえ | テンプレートファセットフィルター： |
| `sortBy`, `order` | いいえ | フィールドと順序を並べ替えます。 |
| `limit`, `offset` | いいえ | ページサイズとページオフセット。 |

### describe_express_template

テンプレート内の編集可能なテキストフィールドと画像の配置を返します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `templateId` | はい | Express テンプレート ID。 |

### list_cta_options

チャネルで許可されているcall-to-action値を返します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channel` | はい | `linkedin`、`meta`、`display`、`tiktok`または`youtube`。 |

### create_draft

1つ以上のエクスペリエンスを含むExpress テンプレートから編集可能なドラフトを作成します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `templateId` | はい | Express テンプレート ID。 |
| `prompt` | はい | Creativeの概要とコピーの手順がドラフトに保存されます。 |
| `experiences` | はい | 各エクスペリエンスのチャネル、コンテンツフィールド、テンプレートフィールドのオーバーライド（オプション）。 |
| `name` | いいえ | ドキュメント名。 |

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
| `emails` | はい | 1つ以上の共同作業者のメールアドレス。 |
| `role` | はい | `editor`または`viewer`。 |
| `message` | いいえ | 招待メッセージ。 |

### request_draft_approval

ドラフトを1人以上の関係者に送信して承認を得る。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `draftId` | はい | ドラフトアセットのID: |
| `emails` | はい | 1つ以上のレビュアーのメールアドレス。 |

### list_experiences

承認済みの公開されたエクスペリエンスを返し、アクティベートする準備が整います。 ドラフトは含まれません。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `channel` | いいえ | エクスペリエンスチャネルフィルター： |
| `createdByMe` | いいえ | 結果は、現在のユーザーが作成したエクスペリエンスに限定されます。 |
| `campaignNames` | いいえ | キャンペーン名フィルターを正確に表示。 |
| `creatorEmail` | いいえ | 作成者のメールフィルター： |
| `createdAtFrom`, `createdAtTo` | いいえ | 作成日の制限： |
| `language` | いいえ | BCP 47言語タグ。 |
| `limit`, `cursor` | いいえ | ページサイズとページネーションカーソル。 |

## ツールを有効化

ツールを活用して有料メディアターゲットを解決し、承認済みのエクスペリエンスを公開します。 公開はこれらのツールで元に戻すことができず、広告費が発生する可能性があります。

### configure_activation_target

必要に応じて、有料メディアアカウント、キャンペーン、広告セット、およびFacebook ページを解決して検証します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `platform` | はい | `META`、`LINKEDIN`または`GOOGLECM360`。 |
| `platformAccountId` | いいえ | 有料メディアアカウントのID。 アカウントの発見は省略します。 |
| `campaignId` | いいえ | MetaまたはLinkedInのキャンペーン ID。 |
| `adsetId` | いいえ | Metaの広告セット、またはLinkedInのキャンペーン ID。 |
| `pageId` | いいえ | MetaのFacebook ページ ID。 |

### create_activation

承認済みのエクスペリエンスと検証済みのターゲットから、ライブの単一イメージ広告を公開します。

| パラメーター | 必須 | 説明 |
|---|---|---|
| `platform` | はい | `META`、`LINKEDIN`または`GOOGLECM360`。 |
| `targetId` | はい | `configure_activation_target`様が検証済みのターゲットを返しました。 |
| `experienceId` | はい | `list_experiences`さんが承認済みのエクスペリエンス IDを返しました。 |
| `assetId` | いいえ | 複数の適格なバリアントを持つエクスペリエンスのバリアント識別子。 |
| `name` | いいえ | 広告プレースメント表示名。 |

`create_activation`を2回呼び出すと、最初の広告を更新する代わりに2つの別々の広告が作成されます。

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
- **コンバージョン指標を確認：** `get_insights_custom_metrics`を呼び出してから、返された指標IDを使用して`get_insights_conversion_metrics`を呼び出します。
- **レコメンデーションをドラフトに変換：** `get_insights_recommendations`に電話してから`create_draft_from_recommendation`に電話してください。
- **テンプレートからビルド：** `list_express_templates`、`describe_express_template`、`list_cta_options`を呼び出してから`create_draft`を呼び出します。
- **承認済みのエクスペリエンスを公開します：** `list_experiences`に電話してから、`configure_activation_target`および`create_activation`に電話してください。

## 関連する機能

- [AI アシスタントの概要](overview.md)
- [AI アシスタントに接続する](connect-ai-assistants.md)
- [AI アシスタントの使用](use-ai-assistants.md)
