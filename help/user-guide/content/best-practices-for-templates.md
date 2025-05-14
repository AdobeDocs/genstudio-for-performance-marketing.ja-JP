---
title: テンプレートのベストプラクティス
description: Adobe GenStudio for Performance Marketingでテンプレートを使用する際は、ベストプラクティスに従ってください。
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: 5666fbf3bae23181232d806b12f520dbc8bc38cf
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# テンプレート使用のベストプラクティス

テンプレートは、事前設定済みのレイアウトとデザイン要素を含む出発点を提供することで、新しいコンテンツの生成に必要な時間と労力を大幅に削減します。

GenStudio for Performance Marketingでテンプレートを使用する場合は、次の推奨事項を使用します。

1. [ テンプレート要素 ](#know-about-template-elements) について
1. コンテンツを効果的にパーソナライゼーションするための [ チャネルガイドライン ](#configure-channel-guidelines) の設定
1. 最適なエクスペリエンスを実現するために [ アクセシビリティ標準 ](accessibility-for-templates.md) を使用したデザイン
1. [ チャネル固有のテンプレートガイドライン ](#follow-channel-specific-template-guidelines) に従う

>[!TIP]
>
>基本的なテンプレートの要素と手順について詳しくは、[ テンプレートの操作 ](use-templates.md) を参照してください。 次のキャンペーンで使用する [ テンプレートのカスタマイズ ](customize-template.md) について詳しく説明します。

## テンプレート要素について

ベストプラクティスとして、テンプレートの各部分をよく理解しておいてください。 テンプレートタイプごとに異なる要素を使用して、チャネル固有のコンテンツ作成用構造を作成します。 テンプレートをカスタマイズするには、GenStudio for Performance Marketingでコンテンツを生成する必要がある場所で、これらの要素の代わりにフィールド名を使用します。

[ テンプレート要素 ](use-templates.md#template-elements) を参照してください。

## チャネルガイドラインの設定

GenStudio for Performance Marketingでテンプレートを使用する前に、各ブランドのチャネルガイドラインを設定してください。 チャネルガイドラインは、テンプレートの使用時に生成されるコンテンツのタイプに直接影響します。 例えば、メールの本文に文字制限を設定できます。

![ ボディ仕様 ](/help/assets/channel-email-body.png)

[ チャネルガイドライン ](/help/user-guide/guidelines/brands.md#channel-guidelines) を参照してください。

## チャネル固有のテンプレートガイドラインに従う

テンプレートを作成する場合は、目的のチャネルの特定の要件を満たしていることを確認します。 各チャネルのレイアウトと視覚要件に対応するテンプレートを作成します。 すべてのテンプレートに適用される一般的なガイドラインを以下に示します。

- クリーンでレスポンシブなHTMLとインライン CSS の使用
- AdobeまたはGoogle フォントの使用
- JavaScript **使用しない**

{{note-css-effects}}

最適なパフォーマンスと互換性を確保するために、各テンプレートタイプを使用する際には次のヒントと制約を考慮してください。

>[!BEGINTABS]

>[!TAB メール]

GenStudio for Performance Marketingと連携するようにメールテンプレートをカスタマイズする場合は、次のデザインのベストプラクティスに従います。

- AdobeまたはGoogle フォントの使用
- クリーンでレスポンシブなHTMLとインライン CSS の使用
- JavaScript **使用しない**
- 本文 **コンテナ** は固定幅を使用しないでください
- 画像には base64 エンコーディングを使用しないでください **使用すると** テンプレートサイズが大幅に増加する可能性があります

**制約**:

- [ セクション ](customize-template.md#sections-or-groups) の使用：
   - 基本テンプレート（1 つのセクションのみ）は、単一のテンプレート要素のセットを生成できます。
   - 複雑なテンプレート（複数のセクション）では、最大 3 つのテンプレート要素セットを生成できます。
- テンプレートで許可される最大フィールド数は 20 です
- HTMLの最大ファイルサイズは 102 KB です

**認識されたフィールド名**:

メールの場合、「`subject`」フィールドが自動的に含まれます。 次のフィールドには、コンテンツプレースホルダーを使用します。

- `pre_header`
- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` （Content JPEG、PNG、GIFから選択）

テンプレートでのフィールド名の使用について詳しくは、[ コンテンツプレースホルダー ](customize-template.md#content-placeholders) を参照してください。

>[!TAB  メタ広告 ]

GenStudio for Performance Marketingと連携するようにメタ広告テンプレートをカスタマイズする場合は、次のデザインのベストプラクティスに従います。

- 列レイアウトには 360 ピクセルの幅を使用
- 画像には 1080 x 1080 ピクセルの最小解像度を使用します
- 相対的 **フォントサイズを使用しない**
- ビューポートを定義し **い** でください
- JavaScript **使用しない**
- CSS **HTML要素を上書きし** い
- `background-image` の代わりに `<img>` タグを使用します
- マスクを使用して、背景画像のテキスト読みやすさを向上させます

**制約**:

- [ セクション ](customize-template.md#sections-or-groups) の使用：
   - 使用できるセクションは 1 つだけで、単一のテンプレート要素セットが生成されます。

**サポートされる縦横比**:

- 正方形 1:1 （1080 x 1080 ピクセル）
- 縦 4:5 （1080 x 1350 ピクセル）
- ストーリー 9:16 （1080 x 1920 ピクセル）
- カスタム画像サイズ：（最小画像幅 50 x 50 ピクセル）

**認識されたフィールド名**:

メタ広告の場合、「`headline`」、「`body`」および「`CTA`」フィールドが自動的に生成されます。 次のフィールドには、コンテンツプレースホルダーを使用します。

- `image` （Content JPEG、PNG、GIFから選択）
- `on_image_text`

テンプレートでのフィールド名の使用について詳しくは、[ コンテンツプレースホルダー ](customize-template.md#content-placeholders) を参照してください。

>[!TAB  バナーとディスプレイ広告 ]

GenStudio for Performance Marketingと連携するようにバナーとディスプレイ広告のテンプレートをカスタマイズする場合は、次のデザインのベストプラクティスに従ってください。

- AdobeまたはGoogle フォントの使用
- スリムなサイズで適切に表示されるアセットの準備
- 埋め込み画像またはエンコードされた背景画像は使用し **い**
- GenStudio for Performance Marketing コンテンツリポジトリにアップロードされた背景画像（`image` フィールド）を使用
- JavaScript **使用しない**

**制約**:

- [ セクション ](customize-template.md#sections-or-groups) の使用：
   - 使用できるセクションは 1 つだけで、単一のテンプレート要素セットが生成されます。

**サポートされるディメンション**:

- 垂直方向：（ピクセル）
   - 300 x 600
   - 160 x 600&#x200B;
- 水平方向：（ピクセル）
   - 300 x 250
   - 728 x 90
   - 336 x 280
   - 320 x 50
   - 970 x 250&#x200B;
- カスタム：（ピクセル）
   - 50 x 50 ～ 2000 x 2000

**認識されたフィールド名**:

バナー広告とディスプレイ広告の場合は、「`CTA`」フィールドが自動的に生成されます。 次のフィールドには、コンテンツプレースホルダーを使用します。

- `headline`
- `sub_headline`
- `body`
- `image` （Content JPEG、PNG、GIFから選択）

テンプレートでのフィールド名の使用について詳しくは、[ コンテンツプレースホルダー ](customize-template.md#content-placeholders) を参照してください。

>[!TAB LinkedIn 広告 ]

[!BADGE Beta]{type=Informative tooltip="この機能は現在Betaにあるので、一部の機能が制限されるか、変更される可能性があります。"}

LinkedIn 広告テンプレートをカスタマイズしてGenStudio for Performance Marketingと連携させる場合は、次のデザインのベストプラクティスに従います。

**制約**:

- [ セクション ](customize-template.md#sections-or-groups) の使用：
   - 使用できるセクションは 1 つだけで、単一のテンプレート要素セットが生成されます。
- 最大画像サイズは 5 MB
- 最大見出し 70 文字
- 150 文字以内の紹介文

**サポートされる縦横比**:

- 正方形 1:1
   - デスクトップまたはモバイル
   - 最小：360 x 360 ピクセル
   - 最大：4320 x 4320 ピクセル
- 水平 1.91:1
   - デスクトップ
   - 最小：640 x 360 ピクセル
   - 最大：7680 x 4320 ピクセル
- 縦 1:1.91
   - mobile
   - 最小：360 x 640 ピクセル
   - 最大：2430 x 4320 ピクセル
- 垂直 2.3
   - mobile
   - 最小：360 x 640 ピクセル
   - 最大：2430 x 4320 ピクセル
- 縦 4.5 （推奨）
   - mobile
   - 最小：360 x 640 ピクセル
   - 最大：2430 x 4320 ピクセル

**認識されたフィールド名**:

LinkedIn 広告の場合、「`headline`」、「`introductory_text`」および「`CTA`」フィールドが自動的に生成されます。 次のフィールドには、コンテンツプレースホルダーを使用します。

- `image` （Content JPEG、PNG、GIFから選択）
- `on_image_text`

テンプレートでのフィールド名の使用について詳しくは、[ コンテンツプレースホルダー ](customize-template.md#content-placeholders) を参照してください。

>[!ENDTABS]
