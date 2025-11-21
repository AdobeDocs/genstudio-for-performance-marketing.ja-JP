---
title: Adobe GenStudio for Performance Marketingでのブランド検証
description: GenStudio for Performance Marketingでのビルトインのブランド検証システムの仕組みを説明します。
feature: Brand Personalization, Variant Generation, Compliance, Content Generation, Content Review, Generative AI
exl-id: 2e777186-3b7e-46a6-9d37-7c7b7c2aa7ae
source-git-commit: e2acf90ef5fef6af03a756882caf53ab125055c4
workflow-type: tm+mt
source-wordcount: '788'
ht-degree: 0%

---

# ブランドの検証

GenStudio for Performance Marketingでは、ブランド認証は、生成 AI 機能およびガイドライン（[[!DNL Brands]](/help/user-guide/guidelines/brands.md)、[[!DNL Products]](/help/user-guide/guidelines/products.md)、[[!DNL Personas]](/help/user-guide/guidelines/personas.md)）と連携して機能する不可欠なコンポーネントです。 すべてのコンテンツが、ブランドアイデンティティ、ADA 標準、個々のチャネルプラットフォームガイダンスに従っていることを確認します。

GenStudio for Performance Marketingは、次のような様々な側面からブランド検証やその他のコンテンツチェックを実施します。

* 定義済みまたはデフォルトの [!DNL Brand] ガイドライン
* Platform のガイドライン
* [&#x200B; 米国障害者法（ADA）基準 &#x200B;](/help/user-guide/guidelines/brand-validation.md#american-with-disabilities-act-ada-validation)
<!-- * Ethical considerations related to gender, ethnicity, race, disability status, and age in AI-generated content -->


## コンテンツチェックの概要

生成されたコンテンツの各項目に対するブランド検証の概要およびその他のコンテンツチェック情報には、キャンバスの各バリアントの _コンテンツチェック_ 概要アイコンからアクセスできます。

_コンテンツチェック_ 概要には、次の項目が表示されます。

* 検証に合格した [[!DNL Brand]](brands.md) ガイドライン [&#x200B; の数とテストしたガイドラインの数から計算した、](overview.md) ールへの準拠の割合
* Metaや LinkedIn など、プラットフォームガイドラインの `Pass` または `Fail` の結果
* ADA アクセシビリティ標準規格に対する `Pass` または `Fail` の結果

![&#x200B; コンテンツチェックの概要 &#x200B;](/help/assets/content-check-summary.png){width="400" zoomable="yes"}

パーセンテージをクリックして、バリアントの準拠を確認します。 バリアントや他のコンテンツを編集すると、スコアが自動更新されます。 _問題を表示および修正_ をクリックして、さらに準拠することができます。

[&#x200B; ブランドの整合性の向上 &#x200B;](#improve-brand-alignment) を参照してください。

## コンテンツチェックパネル

右側のアクションバーからクリックすると _コンテンツチェック_ パネルがキャンバスの右側に開きます _または_ コンテンツチェック [_概要アイコンからクリック_](#content-check-summary)。 このパネルは、詳細なブランド検証、プラットフォームガイドライン、アクセシビリティ標準情報を提供し、改善の機会を明らかにします。

![&#x200B; コンテンツチェックパネル &#x200B;](/help/assets/content-check-panel.png){width="400" zoomable="yes"}

_コンテンツチェック_ パネルには、画像セクションとバリデーションセクションの検証と [&#x200B; コンプライアンス情報 &#x200B;](/help/user-guide/guidelines/overview.md#compliance) が表示されます。

* コンテン _、プラットフォームガイドラインおよびアクセシビリティ標準の_ コンテンツチェック [!DNL Brand] 概要情報の表現
* _レビューが必要_ 節で、失敗したガイドラインの数と、修正が必要な各ガイドラインの詳細情報を表示します
* _合格_ 合格したガイドラインの数と、各合格ガイドラインの詳細情報を表示する節

[&#x200B; コンテンツチェック &#x200B;](#improve-brand-alignment) パネルスコアを改善する方法については、_ブランドの関連付けの向上_ を参照してください。

### コンテンツタイプ

_コンテンツチェック_ パネルでは、実行するガイドラインおよびアクセシビリティ標準チェックを切り替えることができます。 パネルの上部にある _コンテンツタイプ_ アイコン（レベルアイコン）をクリックして、オンとオフを切り替えます。

* **[!DNL Brand]** - ガイドラインに関連するチェック [!DNL Brand] 実行します
* **Platform ガイドライン** - Metaなど、チャネル固有のプラットフォームに関連付けられているチェックを実行します。
* **アクセシビリティ** - ADA アクセシビリティ標準に関連するチェックを実行します

**コンテンツタイプを設定** するには、実行するチェックをオンまたはオフに切り替えるをクリックし、「**適用**」をクリックします。

## ブランドの整合性の向上

生成されるコンテンツの効果を最大限に高め、一貫したブランドアイデンティティを維持するには、[_コンテンツチェック_ 概要 &#x200B;](#content-check-summary) および [_コンテンツチェック_ パネル &#x200B;](#content-check-panel) を使用します。 [[!DNL Brand]  ガイドライン &#x200B;](brands.md)、Platform のガイドラインチェック、アクセシビリティ標準のチェックに合わせて、特定のセクションを手動で変更できます。

**生成されたバリアントのブランドの整合性を向上させるには**:

1. 右側のアクションバーにある _コンテンツチェック_ パネルアイコンをクリックして、検証とアクセシビリティに関する情報を確認します。

   _レビューが必要_ チェックと _合格_ チェックの概要を確認して、改善が必要な項目を確認できます。

   >[!NOTE]
   >
   > _コンテンツチェック_ パネルに記載されている _ブランドの声_ のガイドラインは、個々のセクションではなくバリアント全体に適用されます。 改善案として、コンテンツバリアント全体がハイライト表示されています。

1. 現在準拠していないガイドラインを修正する場合にクリックします。
1. _ヘッドライン_、_カラー_、_ブランドボイス_ などの利用可能なセクションで、レビューが必要な各チェックを展開および検査します。

   各チェックに対して示された推論を使用して、画像とバリアントの変更に関するガイドを示します。

1. 必要な修正を加えたら、「**[!UICONTROL スコアを再確認]**」をクリックして変更を再確認および検証し、ブランド ID、プラットフォームガイドライン、アクセシビリティ標準に合致していることを確認します。

   コンテンツチェックプロセスが再び実行されます。 改訂された項目が検証に合格すると、キャンバスの下部に緑色のバナーが表示され、スコアが更新されたことを確認できます。 再確認の後、変更がなかった場合、バナーはスコアに変更がなかったことを確認します。 改訂されたバリアントの _コンテンツチェック_ 概要アイコンのパーセンテージにも、進捗が表示されます。

1. バリアント全体が検証とアクセシビリティチェックに合格するように、節の改訂を続行します。 キャンバス内の個々のバリアントの横にある矢印を使用して、各バリアントを移動します。

## 米国障害者法（ADA）の検証

これらのアクセシビリティチェックは、Americans with Disabilities Act （ADA）の法的遵守のために含まれています。

[WCAG 1.1.1 非テキストコンテンツ &#x200B;](https://www.w3.org/WAI/WCAG21/Understanding/non-text-content.html) – 画像が `<alt>` 属性を提供することを確認します。
[WCAG 1.4.3 コントラスト（最低限） &#x200B;](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum.html) – 生成されたテキストの背景に対するコントラストが 4.5:1 になるようにします。
[WCAG 3.1.3 珍しい単語 &#x200B;](https://www.w3.org/WAI/WCAG21/Understanding/unusual-words.html) – 慣用句や専門用語を含め、珍しい方法または制限された方法で使用される単語やフレーズを識別します。
[WCAG 3.1.4 略語 &#x200B;](https://www.w3.org/WAI/WCAG21/Understanding/abbreviations.html) – 略語の展開された形式または意味を識別するためのメカニズム。
[WCAG 3.1.5 読み取りレベル &#x200B;](https://www.w3.org/WAI/WCAG21/Understanding/reading-level.html) – より低い中等教育レベルでコンテンツが確実に読み取れるようにします。

