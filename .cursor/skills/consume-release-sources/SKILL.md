---
name: consume-release-sources
description: ""
source-git-commit: c3c6aa86f4f520d020f8928612d1be6be1599652
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---


# リリースソースの使用（Jira + Confluence MCP）

**下流作成：** [generate-release-notes](../generate-release-notes/SKILL.md) → optional [polish-release-notes](../polish-release-notes/SKILL.md)

**解析リファレンス：** [reference.md](reference.md)

**ターゲット出力ファイル （ダウンストリームのみ）:** [help/user-guide/release-notes.md](../../help/user-guide/release-notes.md)

## 前提条件

- **Jira MCP** （`jira_getIssue`, `jira_searchIssues`）が認証されました
- **Confluence MCP** （`confluence_getContent`, `confluence_searchContent`）が認証されました
- ブランチ名（`GS-#####`）、ユーザー入力、またはチケット説明からのJira チケットキー

## ワークフローチェックリスト

1. [ ] **Jira チケットを解決** — `jira_getIssue`を`issueKey`で解決します。 式のWiki リンクとリリース月については、`description`をお読みください。
2. [ ] **式ページを探す** — チケットのWiki URLを使用します。フォールバック CQL: `title ~ "YYYY/MM Release Ceremony" AND space = GenStudio`。
3. [ ] **セレモニー本文** — `confluence_getContent` `bodyMode: storage` （必須；`text` KT リンクとテーブル構造が失われます）。
4. [ ] **機能グループを解析** — **GA リリース機能**&#x200B;および&#x200B;**Beta リリース機能**&#x200B;から行を抽出します（[reference.md](reference.md#ceremony-feature-groups)を参照）。
5. [ ] **包含フィルターを適用** — ユーザースコープごと（[reference.md](reference.md#inclusion-filters)を参照）、Beta行数を確定（ゼロの場合があります）。
6. [ ] **KT ページを解決** — KT タイトルごとに`confluence_searchContent`。`confluence_getContent` `bodyMode: text`。
7. [ ] **KT フィールドを抽出** – 説明、エレベーターピッチ、配信機能、問題の概要、リリースタイプと日付。
8. [ ] **Beta セクション行またはタイプ `Beta`のGA テーブル行に対して、Beta フラグ** — `requiresBetaBadge: true`を設定します。
9. [ 構造化された行リストを含む] **ハンドオフ**&#x200B;から[generate-release-notes](../generate-release-notes/SKILL.md) （出荷されたコピーにwiki/Jira参照はありません）。

## Betaのラベル付け（スキルを生成するためのハンドオフ）

`requiresBetaBadge: true`の場合、ダウンストリーム `###` セクションには、見出しの下にすぐに含める必要があります。

```markdown
[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}
```

Betaのイタリック体スケジュールの免責事項を追加しないでください。バッジはサポートされているパターンです。

## 発送されたリリースノートで禁止

内部ID、Wiki URL、KT引用、Jira キーは、この取り込みフェーズでのみ維持されます。 [generate-release-notes prohibited content](../generate-release-notes/SKILL.md#prohibited-content)ごとに、公開ページのユーザー向け結果を要約します。

## フォールバック

MCP呼び出しが失敗した場合は、ユーザーにセレモニーとKT コンテンツを貼り付けるように依頼し、[reference.md KT フィールドマッピング ](../generate-release-notes/reference.md#internal-sources-kt-and-release-wikis)を使用してgenerate-release-notesを続行します。

## 追加のリソース

- [reference.md](reference.md) – 式解析、CQL、包含フィルター、MCP パラメーター
- [generate-release-notes](../generate-release-notes/SKILL.md) — アーカイブ、ドラフト、リンク、品質チェック
- [polish-release-notes](../polish-release-notes/SKILL.md) — `{#latest}`の下の新規`###`のエディトリアルパス
