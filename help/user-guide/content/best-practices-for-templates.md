---
title: テンプレートのベストプラクティス
description: Adobe GenStudio for Performance Marketingでテンプレートを使用する際は、ベストプラクティスに従ってください。
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '384'
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

明確なチャネルガイドラインの定義は、生成されたコンテンツがブランドの要件や目標に確実に合致するようにするために不可欠です。 チャネルガイドラインでは、テンプレートで使用するトーン、長さ、スタイルなどの要素に関するルールを指定できます。 例えば、本文の最大文字数を設定したり、特定のcall-to-action スタイルを要求したりできます。 これらのガイドラインを事前に設定することで、各 AI プロンプトで詳細な手順を書き出す必要性を減らし、コンテンツ生成プロセスを合理化し、メール間の一貫性を確保します。

テンプレート内のすべての主要なフィールドについて、ブランドの [ チャネルガイドライン ](/help/user-guide/guidelines/brands.md#channel-guidelines) を確認して定義します。 ガイドラインを定義しない場合は、[ デフォルトのチャネルガイドライン ](/help/user-guide/guidelines/brands.md#default-channel-guidelines) が適用されますが、ブランド要件が完全に反映されていない可能性があります。

![ ボディ仕様 ](/help/assets/channel-email-body.png)

[ ブランド、製品、ペルソナのガイドライン ](/help/user-guide/guidelines/overview.md) が生成されたコンテンツにどのように影響し、マーケティング目標に合わせてそれらを調整するかについて説明します。

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
