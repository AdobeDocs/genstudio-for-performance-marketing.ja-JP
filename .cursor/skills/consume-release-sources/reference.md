---
source-git-commit: c3c6aa86f4f520d020f8928612d1be6be1599652
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 3%

---
# リファレンス：リリースソースの使用（MCP）

## 儀式ページの発見

| パターン | 例 |
|---------|---------|
| タイトル | **GenStudio** スペースの`YYYY/MM Release Ceremony` |
| Jiraから | チケット `description`のWiki リンク （推奨） |
| CQL フォールバック | `title ~ "2026/06 Release Ceremony" AND space = GenStudio` |

## 式典特集

リリース式Wikiには、最大&#x200B;**2**&#x200B;個の機能テーブルが含まれます。 **storage** HTMLの両方を解析します。

### GA リリース機能

- セクション見出し：`GA Release Features` （`<h2>`）
- 小見出し：`Feature Group:` （オプションのFloodgate リンク付き）
- テーブル列には、**Type** （`GA`、`Limited`、`EA`、`Beta`、または空）が含まれます
- **KT ドキュメント**&#x200B;列：`<ac:link><ri:page ri:content-title="..."/></ac:link>`

行単位の抽出：

| フィールド | ソース |
|-------|--------|
| `featureDescription` | データ行の最初の`<td>` |
| `type` | 列のセルのテキストを入力 |
| `ktPageTitle` | KT列の`ri:content-title` |
| `jiraKeys` | `ac:macro ac:name="jira"` → `key` パラメーター（内部のみ） |
| `releaseTier` | Typeが`GA`の場合は`ga`、その他のGA テーブル値のTypeを継承 |

### Beta リリース機能

- セクションの見出し：`Beta Release Features` （数か月に&#x200B;**不在**&#x200B;になる可能性があります）
- 2番目のテーブル；**タイプ列** – すべての行がBetaです
- GA テーブルと同じKTおよびJira抽出
- すべてのBeta セクション行に`releaseTier: beta`と`requiresBetaBadge: true`を設定

Beta セクションが見つからない場合は、Beta行を0行としてログに記録して続行します。

### Storage HTML パターン

```html
<ac:link><ri:page ri:content-title="Translation on HZ Canvas" /></ac:link>
<ac:structured-macro ac:name="jira" ...><ac:parameter ac:name="key">GS-23218</ac:parameter></ac:structured-macro>
```

## MCP ツールの使用状況

| ステップ | ツール | パラメーター |
|------|------|------------|
| チケット | `jira_getIssue` | `issueKey`、オプション `expand: renderedFields` |
| セレモニー | `confluence_getContent` | `contentId`, `bodyMode: storage` |
| KT ルックアップ | `confluence_searchContent` | `cql: title = "<KT title>" AND space = GenStudio` |
| KT ボディ | `confluence_getContent` | `contentId`, `bodyMode: text`, `maxBodyChars: 50000` |

**KT リンクを解析する際に、儀式ページに`bodyMode: text`を使用しないでください。**

## KT フィールドマッピング（ドラフト入力）

generate-release-notesにマッピングします。公開リリースノートにverbatimでペーストしないでください。

| KT セクション | 用途 |
|------------|-----|
| 説明 | コア機能 |
| エレベーターピッチ | 価値提案 |
| 配信済み機能 | 具体的な行動 |
| 問題の特定 | ユーザーの課題（コンテキストのみ） |
| リリースタイプと日付 | GA/Beta/制限付き（社内）、バッジ決定を促進 |

## 包含フィルター

不明確な場合は、利用者に範囲を確認する。 共通プリセット：

| プリセット | 含む |
|--------|----------|
| `ga_only` | タイプ = `GA`のGA テーブル行 |
| `ga_and_beta` | **今後数か月の推奨されるデフォルト** — GA行（Type = `GA` **に加えてすべての** Beta リリース機能テーブル行） |
| `ga_plus_empty` | GA テーブル：タイプ = `GA`または空のタイプ |
| `all_except_pilot` | `Limited`を除くGA テーブル行。`ga_and_beta`を使用する場合はBeta セクションを加える |
| `all_with_badges` | すべてのGA テーブル行、Beta セクション行には常にBeta バッジが付与されます |

## Beta バッジのハンドオフ

| 状況 | `requiresBetaBadge` |
|-----------|---------------------|
| **Beta リリース機能** テーブルの行 | `true` |
| タイプ = `Beta`のGA テーブル行 | `true` |
| タイプ = `GA`のGA テーブル行 | `false` |

ダウンストリーム：[generate-release-notes Decision rules](../generate-release-notes/SKILL.md#decision-rules)および[Beta バッジスニペット ](../generate-release-notes/SKILL.md#beta-badge)。

## ハンドオフペイロード（非公式）

アイテムのリストとしてgenerate-release-notesに渡します。

```yaml
- featureDescription: "YouTube Shorts"
  releaseTier: ga
  requiresBetaBadge: false
  ktPageTitle: "YouTube Shorts (Create + Activate)"
  # extracted KT fields: description, elevatorPitch, featuresDelivered, ...
```
