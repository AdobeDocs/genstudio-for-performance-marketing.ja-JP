---
title: テンプレートのベストプラクティス
description: Adobe GenStudio for Performance Marketingでテンプレートを使用する際は、ベストプラクティスに従ってください。
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: 3fe6e235b774cf5a99627d981230f96d5e51ac02
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 0%

---

# テンプレート使用のベストプラクティス

テンプレートは、事前設定済みのレイアウトとデザイン要素を含む出発点を提供することで、新しいコンテンツの生成に必要な時間と労力を大幅に削減します。

GenStudio for Performance Marketingでテンプレートを使用する場合は、次の推奨事項を使用します。

1. [&#x200B; テンプレート要素 &#x200B;](#know-about-template-elements) について
1. コンテンツを効果的にパーソナライゼーションするための [&#x200B; チャネルガイドライン &#x200B;](#configure-channel-guidelines) の設定
1. 最適なエクスペリエンスを実現するために [&#x200B; アクセシビリティ標準 &#x200B;](accessibility-for-templates.md) を使用したデザイン
1. [&#x200B; チャネル固有のテンプレートガイドライン &#x200B;](#follow-channel-specific-template-guidelines) に従う

>[!TIP]
>
>基本的なテンプレートの要素と手順について詳しくは、[&#x200B; テンプレートの操作 &#x200B;](use-templates.md) を参照してください。 次のキャンペーンで使用する [&#x200B; テンプレートのカスタマイズ &#x200B;](customize-template.md) について詳しく説明します。

## テンプレート要素について

ベストプラクティスとして、テンプレートの各部分をよく理解しておいてください。 テンプレートタイプごとに異なる要素を使用して、チャネル固有のコンテンツ作成用構造を作成します。 テンプレートをカスタマイズするには、GenStudio for Performance Marketingでコンテンツを生成する必要がある場所で、これらの要素の代わりにフィールド名を使用します。

[&#x200B; テンプレート要素 &#x200B;](use-templates.md#template-elements) を参照してください。

## チャネルガイドラインの設定

明確なチャネルガイドラインの定義は、生成されたコンテンツがブランドの要件や目標に確実に合致するようにするために不可欠です。 チャネルガイドラインでは、テンプレートで使用するトーン、長さ、スタイルなどの要素に関するルールを指定できます。 例えば、本文の最大文字数を設定したり、特定のcall-to-action スタイルを要求したりできます。 これらのガイドラインを事前に設定することで、各 AI プロンプトで詳細な手順を書き出す必要性を減らし、コンテンツ生成プロセスを合理化し、メール間の一貫性を確保します。

テンプレート内のすべての主要なフィールドについて、ブランドの [&#x200B; チャネルガイドライン &#x200B;](/help/user-guide/guidelines/brands.md#channel-guidelines) を確認して定義します。 ガイドラインを定義しない場合は、[&#x200B; デフォルトのチャネルガイドライン &#x200B;](/help/user-guide/guidelines/brands.md#default-channel-guidelines) が適用されますが、ブランド要件が完全に反映されていない可能性があります。

![&#x200B; ボディ仕様 &#x200B;](/help/assets/channel-email-body.png)

[&#x200B; ブランド、製品、ペルソナのガイドライン &#x200B;](/help/user-guide/guidelines/overview.md) が生成されたコンテンツにどのように影響し、マーケティング目標に合わせてそれらを調整するかについて説明します。

## テンプレート用の画像のアップロード

テンプレートで使用する画像は、コンテンツリポジトリから取得し、正しくアップロードして、画像が正確に表示されるようにする必要があります。

テンプレートにエッジ間（フルブリード）画像が含まれている場合、選択した画像は、テンプレートの全寸法に合わせて自動的にサイズ変更されます。 ただし、画像がテンプレートの縦横比に一致しない場合は、テンプレートの寸法に合わせて画像が切り抜かれ、期待どおりに表示されないことがあります。

テンプレートに含まれる画像に対しては、「自動調整」機能はありません。

画像の切り抜きを解決するには、ユーザーは、コンテンツリポジトリにアップロードする際に、テンプレートで使用される画像の縦横比を定義する必要があります。 承認済みテンプレートをアップロードする場合：

1. [&#x200B; 詳細を追加 &#x200B;](/help/user-guide/content/use-templates.md#add-a-template) ページが表示されるまで **[!UICONTROL テンプレートのアップロードプロセスを続行]** ます。

2. テンプレートで使用する画像の縦横比を **[!UICONTROL 広告の幅（px）]**&#x200B;**[!UICONTROL 広告の高さ（px）]** で定義します。 これにより、画像を表示するテンプレートのセクションに対する画像ウィンドウが定義されます。

3. 「**[!UICONTROL 詳細]**」セクションで、「**[!UICONTROL 画像サイズ]**」ドロップダウンを選択し、「_固定サイズに切り抜き_」を選択します。
   ![&#x200B; 固定サイズに切り抜き &#x200B;](./images/crop-to-fixed-size.png " 固定サイズに切り抜き "){width="80%"}

ブラウザーで画像のサイズと縦横比を決定するには：

1. 画像を検査します。
   - Windows/Linux:
      - F12 キーを押します。
   - macOS:
      - Command + Option + I を押します。

1. 画像の上にマウスポインターを置きます。

1. アスペクト比に注意してください。 テンプレート内の画像の縦横比を定義する場合に使用します。

アップロード時にこれらの詳細が適用されない場合、画像はテンプレートの全縦横比と見なされ、その縦横比に完全に一致しない画像は切り抜いて表示されます。

![&#x200B; ディスプレイでの画像の切り抜き ad](./images/cropped-display.png "Image cropping"){width="60%"}

ディ **❌プレイ広告テンプレートの切り抜き画像**

![&#x200B; ディスプレイ広告に表示される画像 &#x200B;](./images/full-fit.png " ディスプレイ広告に表示される画像 "){width="60%"}

画像 **✅完全に表示されました**

## チャネル固有のテンプレートガイドラインに従う

テンプレートを作成する場合は、目的のチャネルの特定の要件を満たしていることを確認します。 各チャネルのレイアウトと視覚要件に対応するテンプレートを作成します。 すべてのテンプレートに適用される一般的なガイドラインを以下に示します。

- クリーンでレスポンシブなHTMLとインライン CSS の使用
- AdobeまたはGoogle フォントの使用
- JavaScript **使用しない**

{{note-css-effects}}

最適なパフォーマンスを確保するために、各テンプレートタイプを操作する際のヒントと制約について詳しくは、以下を参照してください。

- [メール](/help/user-guide/templates/email-template.md)
- [ディスプレイ広告とバナー広告](/help/user-guide/templates/display-template.md)
- [LinkedIn](/help/user-guide/templates/linkedin-template.md)
- [Meta広告](/help/user-guide/templates/meta-template.md)
