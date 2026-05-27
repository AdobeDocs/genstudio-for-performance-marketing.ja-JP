---
title: 効果的なプロンプトの作成
description: Adobe GenStudio for Performance Marketing の効果的なプロンプトの作成方法について説明します。
role: User
level: Beginner
feature: Create Prompt, Generative AI
exl-id: 0cd4db4f-d031-4c1f-a4e7-adc220f947fc
TQID: https://experienceleague.adobe.com/ESQljlBQv9vk7Zz-SU-hMNkY2zFy6qawEfkonjXaCkQ
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2: id: be495d08-ecd1-455f-951e-c22de504e667id: de1f9646-abd3-4e21-9de2-df62ce55c8dc
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: bcc5edb5-84c3-4940-9f84-ed88b6c16274
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 758
ht-degree: 100%

---

# 効果的なプロンプトの作成

Adobe GenStudio for Performance Marketing を効果的に活用するには、生成 AI とのコミュニケーションが不可欠です。

GenStudio for Performance Marketing は、アセットを変更する機会があるたびに、生成 AI プロンプトを表示します。 効果的なプロンプトのコンポーネントには、具体的な指示文、例、設定済みのガイドラインには含まれていない情報を含める必要があります。

ベストプラクティスとして、[ガイドライン](/help/user-guide/guidelines/overview.md)を使用して GenStudio for Performance Marketing にブランド情報を提供すると、生成 AI を最大限に活用してブランドに即したコンテンツエクスペリエンスを作成できます。

## 具体的な指示文

自然言語を使用してアイデアを明確にし、エクスペリエンスを構築できます。 プロンプトは、AI がビジョンを補完するパーソナライズされたチャネルコンテンツや画像を生成するよう誘導します。 詳細な情報を提供すれば、ニーズに合った画像やエクスペリエンスを生み出す可能性が高まります。 明確かつ具体的な指示文を使って、できるだけ詳細な情報を提供してください。

- **画像**&#x200B;の場合、雰囲気、ムード、色、構図、スタイルを説明する単語を使用します。
- **コピー**&#x200B;では、オーディエンス、目的、新しい機能の説明、例、アクションを説明する単語を使用します。

次に、インテント、ターゲットオーディエンス、スタイルに関する情報を示すサンプルプロンプトを示します。

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.
```

+++サンプル結果を表示

![生成された 3 通のメール](/help/assets/sample-email.png)

+++

## プロンプトの条件

GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md)では、プロンプトドロワーで&#x200B;**[!UICONTROL プロンプト条件]** ([_パラメーター_](/help/user-guide/create/overview.md#parameters)&#x200B;とプロンプト) を使用し、選択操作を通じて詳細を追加し、AI の解釈精度を高めることができます。

[メール](/help/user-guide/create/email-experiences.md)の場合、プロンプト条件には、_パラメーター_&#x200B;に[ガイドライン](/help/user-guide/guidelines/overview.md)を追加すること、メールのバリアントで使用するアセットのアップロード、説明的なプロンプトを含めることができます。 [Meta 広告](/help/user-guide/create/create-meta-ad.md)の場合、プロンプトの条件には、_パラメーター_&#x200B;のブランドガイドライン、既存のアセットの選択またはアップロード、画像またはアセットに関連する設定 (縦横比など)、プロンプトなどを含めることができます。 本当の力は、[ガイドラインの設定](/help/user-guide/guidelines/add-guidelines.md)を行うことから始まります。

>[!NOTE]
>
プロンプトドロワーの&#x200B;_パラメーター_&#x200B;にガイドラインが追加されている場合、プロンプトでそれらを参照する必要はありません。 GenStudio for Performance Marketing では、それらをコンテンツ生成に自動的に活用できます。

### ガイドライン

GenStudio for Performance Marketing のガイドラインは、生成 AI がアセット構成をパーソナライズするのをサポートします。 プロンプト条件が表示されたら、設定済みのガイドラインから [[!DNL Brand]](/help/user-guide/guidelines/brands.md)、[[!DNL Persona]](/help/user-guide/guidelines/personas.md) および [[!DNL Product]](/help/user-guide/guidelines/products.md) を選択できます。

>[!TIP]
>
GenStudio for Performance Marketing で [!DNL Brand] ガイドラインをいつどのように使用するかは、ユーザーが制御します。 ブランドガイドラインを設定および管理する方法については、[ガイドライン](/help/user-guide/guidelines/overview.md)を参照してください。

### 構造化プロンプト

複数セクションから成るメールの場合は、セクション固有の指示を提供するプロンプトを作成して、メールの各セクションに応じて異なるコンテンツを生成できます。 構造化プロンプトでは、生成されたコンテンツを対応するコンテンツプレースホルダーに挿入できるように、[メールテンプレートのセクション名を直接](/help/user-guide/templates/customize-template.md#sections-or-groups)参照する必要があります。

たとえば、最初のセクションでは新製品を宣伝し、2 番目のセクションではコスト削減のメリットを詳しく説明しているメールのコンテンツを生成するように、GenStudio for Performance Marketing に指示できます。

構造化プロンプトは次のようになります。

- メールテンプレートのセクション名には、次のいずれかの参照を使用します。
   - ポッド
   - グループ
   - セクション
   - モジュール

  例えば、テンプレートでセクション名に `moduleA` または `Group-3` を使用している場合、プロンプトでこれらのセクション名を参照できます。

- 推奨されるルール / 構造に従います。 プロンプト構造が指定された形式に従っていない場合、プロンプトは&#x200B;*すべての*&#x200B;メールセクションに適用され、引き続きコンテンツ生成が促進されます。
- メールテンプレートで定義されたセクション名を使用します。 プロンプト参照は、メールテンプレートでコード化されたセクション名と一致する必要があります。
- 大文字と小文字は区別しません。 例えば、メールテンプレートと構造化プロンプトで `Pod` または `pod` を使用できます。
- 最初に汎用ユーザープロンプト、次にセクション固有のディレクティブを参照します。
- セクション名の参照とディレクティブの間は、コロン、ハイフン、コンマ、またはその他の区切り記号 (`,:;#$!~|@=-%&*^_`) を使用して区切ります。 例えば、セクション固有のプロンプトディレクティブとして次を使用できます。`Pod1; Describe how to easily edit text and swap images.`

以下は、推奨されるプロンプト構造を明確にし、識別用の単語 `Pod` を使用するメールテンプレート（`Pod1`、`Pod2`、`Pod3` など）を活用するサンプルプロンプトです。

```properties
Create an exciting multi-pod email focusing on Creative Cloud and its powerful generative AI capabilities.

Encourage customers to convert to Photoshop or use a free Photoshop trial. We want to better educate them about app features.

Pod1: Focus on Adobe Photoshop and its new generative AI tools that enable creators to bring images to life in minutes.

Pod2: Focus on Adobe Illustrator and its new generative AI tools, such as Generative Shape Fill, which allows you to quickly fill your vector outline and explore a variety of options that match the look and feel of your own artwork.

Pod3: Focus on Adobe Acrobat Pro. Make users aware that with Acrobat Pro they can edit images and text inside a PDF.
```

[テンプレート使用のベストプラクティス](/help/user-guide/templates/best-practices-for-templates.md)を参照してください。

## 再試行

プロンプトは反復的なプロセスです。 結果が期待に応えていない場合は、プロンプトを見直して変更を加えるか、詳細を追加してください。 または、キャンペーンの概要から、セクションにペーストすることもできます。 また、GenStudio for Performance Marketing に対して、特定の単語、要素、テーマの使用を避けるようにリクエストすることもできます。

## ベストプラクティス

効果的なプロンプトを作成するための簡単なベストプラクティスをいくつか紹介します。

- 具体的に、すべきこととすべきでないことの詳細を説明する。
- 外部参照を使用してコンテキストを提供する。
- GenStudio for Performance Marketingのガイドラインを活用する。
- ガイドラインのレビューと調整を定期的に行う。
- 反復し改善する。
- 実験を通じて学ぶ。

{{in-academy}}
