---
source-git-commit: 8ed1e6853c9f844c72431dc692b556ece9c215a8
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---
## 目的

AI コーディングアシスタントがGenStudio for Performance Marketing ドキュメントリポジトリを小さく安全に編集するのに役立ちます。

## アーキテクチャの概要（簡単）- このリポジトリーは、`help/` の下の Markdown と、`help/_includes/` の下の共有されたインクルードおよびキュレーションされた画像で構成されるドキュメントサイトです `help/_includes/assets/`- リリースノート、ユーザーガイドおよび拡張機能コンテンツは、`help/` に公開されています。 コンテンツを大幅に変更した場合でも、一番前の項目と既存の見出し構造が維持されます。- このサイトは Jekyll を使用して構築され、GitHub ページでホストされています。 ビルドプロセスでは、一部のカスタムプラグインで標準の Jekyll 規則を使用します。

## プロジェクト固有の規則- カーソルルール：カスタム自動化とガイダンスは `.cursor/rules/*.mdc` に存在します。 例：`.cursor/rules/docs-lint.mdc` （lint プロセス）、`.cursor/rules/generate-release-notes.mdc` （リリースノート形式）。 自動タスクについては、次の手順に従います。- ファイル名とフロントマター：   - リリースノートには、特定の最前線が必要です（`.cursor/rules/generate-release-notes.mdc` を参照）。   - ルールファイルと `.mdc` の拡張子には kebab-case を使用します。- 書式設定規則：ドキュメントでは GitHub 固有の Markdown を使用します。 見出しは通常、文の大文字と小文字を区別し、短い段落の後に続きます。 リリースノートのリストと機能セクションのリストには、`*` の箇条書きを `###` 用します。

## ドキュメントのスタイルガイドライン- 技術ドキュメントのベストプラクティスについては、[Microsoft ライティングスタイルガイド ](https://learn.microsoft.com/en-us/style-guide/) に従ってください。   - ユーザーの行動に重点を置いた、明確で簡潔な文を記述する   - 能動態と現在時制を用いる   - テキストをスキャン可能な短いチャンクに分割します   - 技術的な精度を維持しながら、温かみのある直接的なトーンを維持します- Markdown オーサリング :   - 見出しに文の大文字/小文字を使用（最初の単語は大文字にする）   - 読みやすくするために段落を短くする（2 ～ 3 文）   - 見出しおよびリストの前後に空白行を追加   - UI 要素、ファイルパス、コードにバッククォートを使用する   - すべての画像に代替テキストを含める   - 説明テキストを使用して特定のセクションにリンクする

## 編集の安全ルール（AI ですべきこと）- Jira ID、内部リンク、または企業のみの参照を公開ドキュメントに追加しないでください。 「問題 `generate-release-notes.mdc` トラッキング」の節を参照してください。- フロントマターの YAML を含むファイルを編集する際に、YAML を正確に保持します。 多くのテンプレートとリリースノートは、固定キー（タイトル、説明、役割、exl-id）に依存しています。- lint 修正の場合は、`.cursor/rules/docs-lint.mdc` から自動のべき等モード編集を推奨します（末尾のスペースを削除し、最終的な改行を確保します）。 人間が使用するコマンドの例：

```sh
sed -i '' 's/ $//' <file>
sed -i '' '$ { /^$/d; }' <file> && echo "" >> <file>
```

## 例（変更点と変更方法）- 小さなコピー修正：Markdown ファイル内のテキスト `help/` 更新し、見出しとアンカーをそのままにします。- 画像の更新：`help/_includes/assets/` の下の画像を参照します。 すべての参照を更新せずに、画像を移動したり、名前を変更したりしないでください。

## 最初に見る場所- `help/_includes/` – 共有されたフラグメントと画像。- `.cursor/rules/` – 自動化とリンティングガイダンス。書式設定とプロセスに関する権限のあるルールとして使用します。- `markdownlint_custom.json` - ローカル markdownlint がオーバーライドします。- `.github/pull_request_template.md` — PR の期待。

## いつ人間に尋ねるか- 変更で Docker ベースのツールの実行や変更が必要な場合（リントルールでは Docker が言及されています）、またはサイトビルドパイプラインに影響を与える場合。- ファイルが不明な外部設定を参照している場合（例えば、`markdownlint.json` が見つからない場合） – 作成するか無視するかを尋ねます。

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
必要に応じて、これをリポジトリの `.github/copilot-instructions.md` に結合します（または、表現や長さを調整します）。 何を変更または追加すればよいですか？
