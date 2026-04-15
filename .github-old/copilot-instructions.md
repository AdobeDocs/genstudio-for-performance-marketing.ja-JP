---
source-git-commit: f6a305c6a4e700525b570bbe280e5d1049d06537
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---
## 目的

AI コーディングアシスタントが、GenStudio for Performance Marketingのドキュメントリポジトリを安全に編集できるように支援します。

## 高度なアーキテクチャ（短い）
- このリポジトリは、`help/`の下のMarkdownで構成されるドキュメントサイトで、共有されたインクルードは`help/_includes/`に、キュレーションされた画像は`help/_includes/assets/`に含まれています。
- リリースノート、ユーザーガイド、および拡張性コンテンツは`help/`の下にあります。 コンテンツを大きく変更する場合は、前頭部分と既存の見出し構造を保持する必要があります。
- このサイトはJekyllを使って構築され、GitHub Pagesでホストされています。 ビルドプロセスでは、標準のJekyll規則といくつかのカスタムプラグインを使用します。

## プロジェクトに特化した取り決め
- カーソル ルール：カスタム自動化とガイダンスは`.cursor/rules/*.mdc`にあります。 例：`.cursor/rules/docs-lint.mdc` （lint プロセス）、`.cursor/rules/generate-release-notes.mdc` （は`help/user-guide/release-notes.md`の編集時にリリースノートのスキルを指します）。 タスクの自動化には、次のステップに従ってください。
- エージェントのスキル：タスクワークフローは`.cursor/skills/<name>/SKILL.md`の下にあります。 例：`.cursor/skills/generate-release-notes/SKILL.md` （完全なGenStudio リリースノート手順。同じフォルダーの`examples.md`と`reference.md`で使用）。
- ファイル名とfrontmatter:
   - リリースノート：`help/user-guide/release-notes.md`の既存のExperience League frontmatterを保持します（`.cursor/skills/generate-release-notes/reference.md#frontmatter`を参照）。ファイルを編集すると、シン ルール `.cursor/rules/generate-release-notes.mdc`が自動的に添付されます。
   - ルールファイルおよび`.mdc`拡張子にkebab-caseを使用します。
- フォーマット規則：ドキュメントはGitHub風のMarkdownを使用します。 見出しは一般的に、文頭の大文字と短い段落に続きます。 リリースノートのリストには`*`個、機能セクションには`###`個の箇条書きを使用します。

## ドキュメントのスタイルガイドライン
- テクニカルドキュメントのベストプラクティスについては、[Microsoftのライティングスタイルガイド &#x200B;](https://learn.microsoft.com/en-us/style-guide/)に従ってください。
   - 利用者の行動に焦点を当てた、明確で簡潔な文章を書く
   - アクティブな声と現在の緊張を使用する
   - テキストをスキャン可能な短いチャンクに分割
   - 技術的な正確性を維持しながら、暖かみのある直接的なトーンを維持したい
- Markdown オーサリング：
   - 見出しに文頭の大文字と小文字を区別する（先頭の単語のみ）
   - 段落を短くする（2～3文）
   - 見出しとリストの前後に空白行を追加する
   - UI要素、ファイルパス、コードにバックティックを使用する
   - すべての画像に代替テキストを含める
   - 説明テキストを使用して特定のセクションにリンクする

## 編集の安全性ルール（AIで実行すべき処理）
- Jira ID、内部リンク、または企業のみの参照をパブリックドキュメントに絶対に追加しない。 `.cursor/skills/generate-release-notes/SKILL.md` （セクション **禁止コンテンツ**）を参照してください。
- それを含むファイルを編集する場合は、Frontmatter YAMLを正確に保持します。 多くのテンプレートやリリースノートは、固定キー（タイトル、説明、役割、exl-id）に依存しています。
- Lint修正の場合は、`.cursor/rules/docs-lint.mdc`から自動的に同じ権限を持つ編集を優先します（末尾のスペースを削除し、最終改行を確認します）。 人間が使用するコマンドの例：

```sh
sed -i '' 's/ $//' <file>
sed -i '' '$ { /^$/d; }' <file> && echo "" >> <file>
```

## 例（何をどのように変更するか）
- 小さなコピーの修正：`help/` Markdown ファイル内のテキストを更新し、見出しとアンカーをそのまま維持します。
- 画像の更新：`help/_includes/assets/`の下の画像を参照します。 すべての参照を更新せずに画像を移動したり、名前を変更したりしないでください。

## 最初に確認すべき場所
- `help/_includes/` – 共有フラグメントと画像。
- `.cursor/rules/` – 自動化とリンティングのガイダンス。これらを書式設定とプロセスの信頼性の高いルールとして使用します。
- `markdownlint_custom.json` — ローカルのmarkdownlint オーバーライド。
- `.github/pull_request_template.md` – 期待をPRします。

## 人間に尋ねるタイミング
- 変更がDocker ベースのツールの実行または変更を必要とする場合（lint ルールはDockerに言及しています）、またはサイト構築パイプラインに影響を与える場合。
- ファイルが不明な外部設定を参照している場合（例：`markdownlint.json`が見つからない場合）、作成するか無視するかを尋ねます。

## 人間に対する最小限のコマンド

```sh
# Install linter (if not present)
npm install -g markdownlint-cli

# Run lint locally using project config
markdownlint --config markdownlint_custom.json "help/**/*.md"

# Project lint via yarn (preferred if available in environment)
yarn lint
```

&#x200B;---
必要に応じて、これをリポジトリの`.github/copilot-instructions.md`にマージできます（または文言/長さを調整できます）。 何を変更または追加すればよいですか？
