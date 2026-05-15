---
title: 電子メール体験
description: 承認済みのライブラリからのキャンバスの動作やコンテンツフラグメントスワップなど、Adobe GenStudio for Performance Marketingでのメールエクスペリエンスについて説明します。
feature: Create Canvas, Media Templates
role: User
level: Beginner
exl-id: e2bddd02-914e-43a8-92b6-fdcbced94a6a
TQID: https://experienceleague.adobe.com/-lwSfvc0TnVd8byNT-5OfoEsXz7yaeIifcHOJtp-n4c
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2:
  - id: a8b28c00-da6e-4d27-8667-80f790ad8972
  - id: be495d08-ecd1-455f-951e-c22de504e667
  - id: dee4e9a9-78d1-4953-8179-f8da6117027d
  - id: ee4b6e5f-5b7a-421b-9859-0f964841a866
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: e41ca23a135e2cacfcc029c04992bbff1b515bd6
workflow-type: tm+mt
source-wordcount: 580
ht-degree: 0%

---

# 電子メール体験

Adobe GenStudio for Performance Marketingでは、生成AIを使用して、効果の高いメールエクスペリエンスの[作成を効率化できます](/help/user-guide/create/create-email-experience.md)。

[!DNL Create]を使用すると、現代のマーケターは[&#x200B; ガイドライン &#x200B;](/help/user-guide/guidelines/overview.md)、画像アセット、および[適切に作成されたプロンプト &#x200B;](/help/user-guide/effective-prompts.md)を使用して、ブランドに即したメールエクスペリエンスをすばやく[作成できます](/help/user-guide/create/create-email-experience.md)。

メール体験を生成する際には、4つのバリエーションが作成され、キャンバスに表示されます。

メールエクスペリエンスの編集可能なセクションには、次のようなものがあります。

* プリヘッダー
* Headline
* 小見出し
* 本文
* Call to action（CTA）
* 画像

[&#x200B; テンプレート要素](/help/user-guide/templates/use-templates.md#template-elements)を参照してください。

<!-- 
## Email capabilities

Content creators and marketers can produce brand-consistent email experiences in GenStudio for Performance Marketing. 
-->

## マルチセクションメール

メール体験には、さまざまなセクションが含まれているため、ブランドや目標に合わせて完全にカスタマイズすることができます。 [&#x200B; セクション &#x200B;](/help/user-guide/create/create-email-experience.md#add-parameters)ごとに [!DNL Products] とビジュアルアセットを選択し、[構造化プロンプト &#x200B;](/help/user-guide/effective-prompts.md#structured-prompts)を使用して独自のコンテンツを作成します。 各セクションは、1つのビジュアルアセットをサポートしています。

複数セクションのテンプレートを作成する方法については、[&#x200B; セクションを使用したテンプレートのカスタマイズ &#x200B;](/help/user-guide/templates/customize-template.md#sections-or-groups)を参照してください。

## プログレッシブロード

コンテンツ生成プロセスが開始されると、生成されたコンテンツの各セクションがメールのバリエーションで徐々にカンバスに読み込まれます。 エクスペリエンス、アセット、エクスペリエンス内のフィールドとセクションは、生成されるとキャンバスに個別に表示されます。

**[!UICONTROL 生成]**&#x200B;をクリックすると、生成の進行状況を更新する読み込みインジケーターがキャンバスの下部に表示されます。

メールエクスペリエンスの各フィールドとセクションは、次の順序で段階的に読み込まれます。

1. バリアント名
1. すべてのバリエーションの件名
1. プリヘッダー
1. 見出し、メール本文（単一セクションメール用）、CTA
1. 後続のセクションのメール本文（複数セクションのメール）
1. ブランド検証

   ブランドの検証とコンテンツのチェックプロセスが実行され、各バリエーションに&#x200B;[_コンテンツチェック_&#x200B;の概要](/help/user-guide/guidelines/brand-validation.md#content-check-summary)が入力されます。

## 文字数

一連のメールのバリエーションを生成すると、各セクションに表示される文字数を確認できます。 件名や本文など、生成されたセクションにカーソルを合わせるかクリックし、そのセクションのセクション名と文字数を確認します。

![文字数](/help/assets/character-count.png){width="500" zoomable="yes"}

## コンテンツフラグメントスワップ {#content-fragment-swap}

>[!NOTE]
>
>コンテンツフラグメントの入れ替えは、現在、キャンバス上の&#x200B;**電子メール**&#x200B;のエクスペリエンスで利用できます。 **Horizon** チャネルのサポートは近日提供開始予定です。

多くの場合、企業のメールコンテンツには、テンプレートに適したコンテンツとともに、新しく生成されたコピーと承認済みのモジュラーブロック（免責事項、安全言語、オファー、規制上の主張など）の両方が必要になります。 [!DNL Adobe Experience Manager]にモジュラーコンテンツを保存するチームは、[!DNL GenStudio for Performance Marketing]を離れることなく、そのコンテンツを検索してメールエクスペリエンスで使用することができます。 これは、次の場合に便利です。

* **コンプライアンス対応コンテンツ：** AIはクリエイティブスロットを埋める一方、コンプライアンス承認済みのフラグメントは注射可能なスロットを置き換えます。ロックされた領域は書き出しによって変更されません。
* **再利用可能な承認済みコンテンツコンポーネント：**&#x200B;承認済みの見出し、地域の免責事項、または製品の説明は、作成者がコピー&amp;ペーストの回避策なしでバリエーションに取り込む間、[!DNL Adobe Experience Manager]の記録システムを維持できます。

クリエイターはキャンバスでエクスペリエンスを組み立て、ブランド部門とコンプライアンス部門は承認ワークフローを[!DNL Adobe Experience Manager]に保持、IT部門と統合部門はリポジトリと組織が必要とする権限を結び付けます。

![&#x200B; コンテンツフラグメントの入れ替え](./cf-swap.png){width="500" zoomable="yes"}

組織でコンテンツフラグメントスワップを有効にすると、次のことが期待できます。

* コンテンツフラグメントフィールドには、手作業による入力やAIによる生成のみではなく、接続されているコンテンツライブラリを利用して入力できます。
* キャンペーン、ペルソナ、チャネル、言語、ブランドなどのメタデータを使用して、フラグメントを参照、検索、フィルタリングできます。
* 複数のリポジトリが設定されている場合は、リポジトリピッカーを使用できます。
* フィールドテキストを置き換える前のフラグメントのプレビュー。
* 1回のアクションで、すべてのバリエーションにフラグメント選択を反映。

![&#x200B; コンテンツフラグメント UI ペイン &#x200B;](./cf-pane.png){width="500" zoomable="yes"}

組織が、使用可能なコンテンツフラグメントソースとリポジトリを選択します。 管理者がソースを設定する方法と、作成者がCanvasから&#x200B;**[!UICONTROL Swap]**&#x200B;でコピーをスワップする方法については、[&#x200B; コンテンツフラグメント拡張機能](/help/extensibility/deploy-app.md#find-content-fragment-extension)を参照してください。
