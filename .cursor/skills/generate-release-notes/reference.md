---
source-git-commit: f6a305c6a4e700525b570bbe280e5d1049d06537
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 6%

---
# リファレンス：リリースノートのオーサリング

## Frontmatter

ライブページ [help/user-guide/release-notes.md](../../help/user-guide/release-notes.md)には、最小限のセットを超えたExperience League メタデータが含まれています（例：`TQID`、`product_v2`、`feature_v2`、分類ID）。

**ルール：**

- リリースノート **body**&#x200B;のコンテンツを編集する場合、タスクがメタデータの変更を明示的に求めない限り、**既存のfrontmatter**&#x200B;のキーと値を保持します。
- より短いテンプレートに合わせて、分類や商品メタデータを削除しないでください。
- ExL ページに必要な概念には、通常、`title`、`description`および`role`が含まれます。新しいページについては、[Experience League メタデータガイダンス &#x200B;](https://experienceleague.adobe.com/en/docs/authoring-guide/using/authoring/using-metadata)に従ってください。

## 内部ソース（KTおよびリリースウィキ）

これらのフィールドは&#x200B;**ドラフト**&#x200B;中にのみ使用してください。公開されたリリースノートでは、内部ドキュメントを参照することはできません。

### ナレッジトランスファー（KT）文書

次から抽出：

| フィールド | 用途 |
|-------|-----|
| 説明 | コア機能の説明 |
| エレベーターピッチ | 価値提案 |
| 配信済み機能 | 具体的な行動 |
| 問題提起 | 利用者の課題 |
| リリースタイプと日付 | タイミング |

### Wiki ページのリリース

グループ化と範囲：

| フィールド | 用途 |
|-------|-----|
| リリース日（修正バージョン） | 同じ日付→同じリリースノートのバッチ |
| イニシアチブ | コンテキストのみ。公開テキスト内で内部リンクを行わないでください |
| PMはKTを使用して機能を提示します | シグナルより深いKTの詳細が存在する可能性がある |

**スコープ ルール：**&#x200B;同じリリース日（修正バージョン）を共有するアイテムは、同じ月次リリース ブロックに属しています。

## ドキュメントへのリンク

- **最も関連性の高い** フレーズへのリンク（例：「サポートされていない画像と動画のアセット」を広告フォーマットのセクションにリンク）。
- 右側のサブセクションに`#anchor`個のリンクを配置する。
- 概要ページは、より深いアンカーが存在しない場合に使用できます。

## 一般的なドキュメントのパス

| 面グラフ | パス接頭辞 |
|------|-------------|
| 作成 | `/help/user-guide/create/` |
| コンテンツ | `/help/user-guide/content/` |
| アクティブ化 | `/help/user-guide/activation/` |
| 承認 | `/help/user-guide/approvals/` |
| インサイト | `/help/user-guide/insights/` |
| ガイドライン | `/help/user-guide/guidelines/` |
| テンプレート | `/help/user-guide/templates/` |
| キャンペーン | `/help/user-guide/campaigns/` |
| 拡張機能 | `/help/extensibility/` |
