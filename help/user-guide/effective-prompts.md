---
title: 有効なプロンプトの記述
description: Adobe GenStudio for Performance Marketingの効果的なプロンプトを記述する方法を説明します。
role: User
level: Beginner
feature: Create Prompt, Generative AI
exl-id: 0cd4db4f-d031-4c1f-a4e7-adc220f947fc
TQID: https://experienceleague.adobe.com/ESQljlBQv9vk7Zz-SU-hMNkY2zFy6qawEfkonjXaCkQ
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2:
  - id: be495d08-ecd1-455f-951e-c22de504e667
  - id: de1f9646-abd3-4e21-9de2-df62ce55c8dc
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: bcc5edb5-84c3-4940-9f84-ed88b6c16274
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 758
ht-degree: 0%

---

# 有効なプロンプトの記述

Adobe GenStudio for Performance Marketingで効果的に作業するには、生成 AI とのコミュニケーションが不可欠です。

GenStudio for Performance Marketingでは、アセットを変更する機会があるたびに生成 AI プロンプトが表示されます。 効果的なプロンプトのコンポーネントには、説明的な言語、例、設定済みのガイドラインでは提供されない情報を含める必要があります。

ベストプラクティスとしては、[&#x200B; ガイドライン &#x200B;](/help/user-guide/guidelines/overview.md) を使用してGenStudio for Performance Marketingにブランド情報を提供すると、生成 AI を最大限に活用して、ブランドに合わせたコンテンツエクスペリエンスを作成できます。

## 記述言語

自然言語を使用して、アイデアを明確に表現し、エクスペリエンスを作成できます。 プロンプトは、パーソナライズされたチャネルコンテンツやビジョンを補完する画像を生成するために AI をガイドします。 提供する詳細情報が多いほど、ニーズを満たす画像やエクスペリエンスを作成する可能性が高くなります。 明確で説明的な言語を使用して、可能な限り詳細な情報を提供します。

- **画像** には、雰囲気、気分、色、構成、スタイルを説明する単語を使用します。
- **コピー** については、オーディエンス、目的、新機能の説明、例およびアクションを説明する単語を使用します。

インテント、ターゲットオーディエンスおよびスタイルに関する情報を明確にするサンプルプロンプトを次に示します。

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.
```

+++サンプル結果を参照

![&#x200B; 生成された 3 通のメール &#x200B;](/help/assets/sample-email.png)

+++

## プロンプト条件

GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) では、プロンプトドロワーで **[!UICONTROL プロンプト条件]** （[_パラメーター_](/help/user-guide/create/overview.md#parameters) とプロンプト）を使用して、選択を通じて詳細を追加し、AI の解釈を改善できます。

[&#x200B; メール &#x200B;](/help/user-guide/create/email-experiences.md) の場合、プロンプト条件には [&#x200B; パラメーター &#x200B;](/help/user-guide/guidelines/overview.md) に _ガイドライン_ を追加すること、メールのバリエーションで使用するアセットをアップロードすること、説明プロンプトを含めることができます。 [Meta広告 &#x200B;](/help/user-guide/create/create-meta-ad.md) の場合、プロンプトの条件には、_パラメーター_ でのブランドガイドライン、既存アセットの選択またはアップロード、画像またはアセットに関連する設定（縦横比など）、プロンプトなどが含まれます。 真のパワーは、[&#x200B; ガイドラインの設定 &#x200B;](/help/user-guide/guidelines/add-guidelines.md) から始まります。

>[!NOTE]
>
>プロンプトのドロワーの _パラメーター_ にガイドラインが追加されている場合は、プロンプトにガイドラインへの参照を含める必要はありません。 GenStudio for Performance Marketingでは、これらをコンテンツの生成に自動的に活用します。

### ガイドライン

GenStudio for Performance Marketingのガイドラインは、生成 AI がアセット構成をパーソナライズするのに役立ちます。 プロンプト条件が表示されたら、設定済みのガイドラインから [[!DNL Brand]](/help/user-guide/guidelines/brands.md)、[[!DNL Persona]](/help/user-guide/guidelines/personas.md)、[[!DNL Product]](/help/user-guide/guidelines/products.md) を選択できます。

>[!TIP]
>
>GenStudio for Performance Marketingで [!DNL Brand] ガイドラインを使用する方法とタイミングを制御します。 ブランドガイドラインの設定および管理方法については、[&#x200B; ガイドライン &#x200B;](/help/user-guide/guidelines/overview.md) を参照してください。

### 構造化されたプロンプト

複数セクションのメールの場合、メール内のセクションごとに様々なコンテンツを生成するための、セクション固有の手順を提供するように促す構造を作成できます。 構造化プロンプトは、生成されたコンテンツを対応するコンテンツプレースホルダーに挿入できるように [&#128279;](/help/user-guide/templates/customize-template.md#sections-or-groups) メールテンプレート内のセクション名  を直接参照する必要があります。

例えば、最初のセクションでは新製品のプロモーションをおこない、2 番目のセクションではコスト削減のメリットを詳しく説明するメールのコンテンツを生成するよう、GenStudio for Performance Marketingに指示できます。

構造化されたプロンプトでは、次の操作を行う必要があります。

- メールテンプレートのセクション名に、次のいずれかの参照を使用します。
   - ポッド
   - グループ
   - セクション
   - モジュール

  例えば、テンプレートでセクション名として `moduleA` または `Group-3` を使用している場合、プロンプトでこれらのセクション名を参照できます。

- 推奨されるルール/構造に従います。 プロンプト構造が指定された形式に準拠していない場合、プロンプトは *すべて* のメールセクションに適用され、引き続きコンテンツの生成を容易にします。
- メールテンプレートで定義したセクション名を使用します。 プロンプト参照は、メールテンプレートにコーディングされたセクション名と一致する必要があります。
- 大文字と小文字を区別しない。 例えば、メールテンプレートと構造化プロンプトで `Pod` または `pod` を使用できます。
- 最初に汎用のユーザープロンプトを参照し、次にセクション固有のディレクティブを参照します。
- セクション名の参照とディレクティブの間の区切りとして、コロン、ハイフン、コンマ、その他の区切り文字（`,:;#$!~|@=-%&*^_`）を使用します。 例えば、次をセクション固有のプロンプトディレクティブとして使用できます。`Pod1; Describe how to easily edit text and swap images.`

以下は、推奨されるプロンプト構造を明確にし、`Pod1`、`Pod2`、`Pod3` などの識別用語 `Pod` を使用するメールテンプレートを活用するプロンプトのサンプルです。

```properties
Create an exciting multi-pod email focusing on Creative Cloud and its powerful generative AI capabilities.

Encourage customers to convert to Photoshop or use a free Photoshop trial. We want to better educate them about app features.

Pod1: Focus on Adobe Photoshop and its new generative AI tools that enable creators to bring images to life in minutes.

Pod2: Focus on Adobe Illustrator and its new generative AI tools, such as Generative Shape Fill, which allows you to quickly fill your vector outline and explore a variety of options that match the look and feel of your own artwork.

Pod3: Focus on Adobe Acrobat Pro. Make users aware that with Acrobat Pro they can edit images and text inside a PDF.
```

[&#x200B; テンプレート使用のベストプラクティス &#x200B;](/help/user-guide/templates/best-practices-for-templates.md) を参照してください。

## 再試行

プロンプトは反復的なプロセスです。 結果が期待どおりでない場合は、プロンプトを確認し、変更を加えるか、詳細を追加します。 または、キャンペーン概要のセクションにペーストすることもできます。 特定の単語、要素またはテーマを避けるようにGenStudio for Performance Marketingにリクエストすることもできます。

## ベストプラクティス

効果的なプロンプトを作成するためのシンプルなベストプラクティス：

- 具体的に説明し、実行する操作と実行しない操作の詳細を指定します。
- 外部参照を使用してコンテキストを提供する
- GenStudio for Performance Marketingのガイドラインを活用します。
- ガイドラインを定期的に確認し、調整します。
- 繰り返して調整します。
- 実験を通じて学ぶ。

{{in-academy}}
