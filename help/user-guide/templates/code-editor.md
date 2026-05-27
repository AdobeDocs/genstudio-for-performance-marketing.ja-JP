---
title: テンプレートコードエディタ
description: GenStudio for Performance Marketingのテンプレートコードエディターの使用方法を説明します。
level: Intermediate
role: Developer
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
TQID: https://experienceleague.adobe.com/QtGu-GaR4LMNGa4IrtYKzk1EjL1g9y08hF-kAm4rLJM
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 787
ht-degree: 1%

---

# テンプレートコードエディタ

テンプレートコードエディターは、GenStudio for Performance Marketingを使用して新しいエクスペリエンスを生成する際に、最適な使用のためにテンプレートを検証および調整できるように設計されています。 このエディターでは、テンプレート内のプレースホルダーを使用して、GenStudio for Performance Marketingでコンテンツを生成する場所を示すHandlebars構文をサポートしています。

>[!TIP]
>
>テンプレート HTML コードを[!DNL Content] _テンプレート_ ビューにアップロードする前に、[ テンプレートのカスタマイズ ](customize-template.md) ガイダンスで定義されたコンテンツ プレースホルダーを挿入して、テンプレートを準備します。

## 検出されたフィールドの確認

_[!UICONTROL 検出されたフィールドの確認]_ ペインには、GenStudio for Performance Marketingがテンプレートで認識するフィールドのリストが表示されます。 リストを確認すると、HTML コードをスクロールして、テンプレートのフォーメーションを確認できます。

![ コードエディタービュー](/help/assets/template-detected-fields.png "検出されたフィールドを確認"){width="600"}

リストにフィールドが見つからない場合は、テンプレートコードを検索して、見つからないフィールドの場所を見つけます。 Handlebars構文と[認識済みのフィールド名](/help/user-guide/templates/customize-template.md#recognized-field-names)を使用して、正しいプレースホルダーを挿入します。 コードエディターの下部に表示される「検索と置換」フォームを使用して、コード内の特定の文字列を検索します。 （Windows `CTRL`+`F`またはmacOS `CMD`+`F`）

## 変数の役割の調整

テンプレート構造のチェック中に、ドロップダウンを使用して、テキストベースのフィールドロール（例：`headline`、`sub_headline`、`body`、`cta`、`on_image_text`、`custom`）のフィールドロールを選択および変更できます。 フィールドの役割の選択は、テンプレートの編集中も保持されるため、カスタマイズが失われることなく、ワークフローの効率が向上します。

>[!NOTE]
>
>画像変数は、役割を調整できません。

![複数役割フィールドの選択](/help/assets/multirole-dropdown-field.png "複数役割フィールドの選択"){width="600"}

変数に役割を割り当てるには、次の手順に従います。

1. _[!UICONTROL 検出されたフィールドを確認]_ ペインで変数を検索します。 これらの変数は自動的に検出されます。
2. 各変数に割り当てられた役割を確認します。 役割は自動的に割り当てられますが、テンプレート内の任意の変数のドロップダウンを使用して調整できます。
3. ドロップダウンから新しい役割を選択して、役割を調整します。
4. 「**[!UICONTROL 次へ]**」をクリックして次に進みます。

## 修正する

テンプレートにエラーがある場合は、問題の簡単な説明を含む`Template is invalid` メッセージが表示される場合があります。 次の例では、メッセージは、`_image` フィールドがマルチポッドテンプレートで確立されたフィールド命名規則に準拠していないことを示しています。 このメッセージでは、正しい接頭辞を使用してフィールド名を更新する必要があることをさらにアドバイスします。 テンプレートコードエディターで「`_image`」フィールドを見つけ、必要に応じて名前を更新します。

![無効なテンプレートを修正](/help/assets/animation/template-code-editor.gif){width="600"}

_[!UICONTROL チェックで検出されたフィールド]_&#x200B;のペインが更新され、変更が反映されます。 フィールドが正しく入力されていることを確認したら、**[!UICONTROL 次へ]**&#x200B;をクリックして、テンプレートのアップロードを続行します[3}。](/help/user-guide/templates/use-templates.md#add-a-template)

## テンプレートの一般的な問題と解決策

| **エラー** | **説明** | **ソリューション** |
|-----------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| 解析できませんでした | テンプレートコンテンツを有効なHandlebarsとして解析できませんでした。 | テンプレートにHTMLとHandlebarsの構文エラーがないか確認し、それらを修正して、[ コンテンツプレースホルダー](/help/user-guide/templates/customize-template.md#content-placeholders)の有効な書式設定を確認します。 |
| グループが割り当てられていません | マルチグループメールテンプレートの画像フィールドは、どのグループにも割り当てられていません。 | セクション接頭辞の一貫した使用を確認します。 各[ セクション ](/help/user-guide/templates/customize-template.md#sections-or-groups)では、各フィールドタイプ （`headline`、`body`、`image`、`cta`）のうち1つのみを使用できます。 テンプレート内の有効なグループに`image` フィールドを割り当てます。 |
| 画像がありません | 必須の画像フィールドがありません。 | Meta、ディスプレイ、バナー広告などの特定のテンプレートタイプには、1つの`image` フィールドが必要です。 必要な`image` フィールドをテンプレートに追加します。 |
| 無効な単一グループ | メールテンプレートに1つのグループが含まれていますが、これは無効です。 | 基本的なメールテンプレートには、テンプレート要素のセットが1つ含まれており、[ セクションまたはグループ ](/help/user-guide/templates/customize-template.md#sections-or-groups)で定義されているグループ命名規則は必要ありません。 グループ命名構文を削除して、テンプレートを調整してセクションがゼロになるように設定します。 |
| フィールドなし | テンプレートにフィールドが含まれていません。 | 特定の種類のコンテンツを生成するためにGenStudio for Performance Marketingが必要なテンプレートに、Handlebars構文を使用して[認識されたフィールド名](/help/user-guide/templates/customize-template.md#recognized-field-names)を追加します。 |
| 必須プロパティがありません | 必要なメタデータプロパティの一部が見つかりません。 | 各テンプレートタイプには、チャネルガイドラインにもとづく要件と制約があります。 たとえば、Metaではアスペクト比が必要であり、ディスプレイ広告ではディメンションが必要です。 [ チャネル固有のテンプレートガイドラインに従う](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines)。 |
| 予約済みの名前が使用されました | 禁止または予約済みのフィールド名が使用されています。 | `subject`や`introductory_text`など、特定の[ フィールド名](/help/user-guide/templates/customize-template.md#recognized-field-names)は予約されています。 予約名または禁止名を使用するフィールドの名前を変更します。 |
| フィールドが多すぎます | フィールド数がグローバル制限の20を超えています。 | 不要なフィールドを削除して、合計が20を超えないようにします。 |
| グループが多すぎます | グループの数が、チャネルで許可されている最大数を超えています。 | Meta、ディスプレイ、LinkedInのテンプレートでは、複数のセクションを使用できません。 2つまたは3つのセクションを定義する場合、メールにはグループ名が必要です。 テンプレート内のグループの数を減らして、[ チャネルの要件](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines)を満たします。 |
| サポートされていないフィールド | テンプレートは、チャネルがサポートしていないフィールドを使用しています。 | [認識されたフィールド名](/help/user-guide/templates/customize-template.md#recognized-field-names)に従って、サポートされていないフィールドを置き換えるか削除します。 |
