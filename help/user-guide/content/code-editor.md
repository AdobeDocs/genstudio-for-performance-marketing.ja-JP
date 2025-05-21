---
title: テンプレートコードエディター
description: GenStudio for Performance Marketingのテンプレートコードエディターの使用方法を説明します。
level: Intermediate
role: Developer
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
source-git-commit: 3739a218ce67749d0038059e3504ab9a4df8f065
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 0%

---

# テンプレートコードエディター

テンプレートコードエディターは、GenStudio for Performance Marketingで新しいエクスペリエンスを生成する際に最適に使用できるよう、テンプレートの検証と調整に役立つように設計されています。 このエディターでは、Handlebars 構文をサポートしています。この構文では、テンプレート内のプレースホルダーを使用して、GenStudio for Performance Marketingでコンテンツを生成する場所を指定します。

>[!TIP]
>
>[!DNL Content] の _テンプレート ](customize-template.md) ビューにテンプレートHTMLコードをアップロードする前に、[ テンプレートのカスタマイズ_ ガイダンスで定義されているコンテンツプレースホルダーを挿入してテンプレートを準備します。

## 検出されたフィールドを確認

_[!UICONTROL 検出されたフィールドの確認]_ ウィンドウには、GenStudio for Performance Marketingがテンプレートで認識するフィールドのリストが表示されます。 リストを確認すると、HTML コードをスクロールしてテンプレートの作成を確認できます。

![ コードエディタービュー ](/help/assets/template-detected-fields.png " 検出されたフィールドの確認 "){width="600" zoomable="yes"}

リストにフィールドがないことに気付いた場合は、テンプレートコードを検索し、見つからないフィールドの場所を見つけます。 Handlebars 構文と [ 認識されたフィールド名 ](/help/user-guide/content/customize-template.md#recognized-field-names) を使用して、正しいプレースホルダーを挿入します。 コードエディターの下部に表示される「検索と置換」フォームを使用して、コード内の特定の文字列を検索します。 （Windows `CTRL`+`F` またはmacOS `CMD`+`F`）

### 修正を行う

テンプレートにエラーがある場合は、問題の簡単な説明を含む `Template is invalid` メッセージが表示される場合があります。 次の例では、`_image` フィールドが複数ポッドテンプレートで確立されたフィールド命名規則に準拠していないことを示すメッセージが表示されます。 また、フィールド名を正しいプレフィックスで更新する必要があることをお知らせします。 テンプレートコードエディターで「`_image`」フィールドを見つけ、指示に従って名前を更新します。

![ 無効なテンプレートを修正 ](/help/assets/animation/template-code-editor.gif){width="600" zoomable="yes"}

_[!UICONTROL 検出されたフィールドをチェック]_ パネルが更新され、変更が反映されます。 フィールドが正しく、完全であることを確認したら、「**[!UICONTROL 次へ]**」をクリックして続行 [ テンプレートのアップロード ](/help/user-guide/content/use-templates.md#add-a-template) します。

## テンプレートの一般的な問題と解決策

| **エラー** | **説明** | **ソリューション** |
|-----------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| の解析に失敗しました | テンプレートのコンテンツを有効な Handlebars として解析できませんでした。 | テンプレートでHTMLおよび Handlebars 構文エラーがないか確認し、それらのエラーを修正して [ コンテンツのプレースホルダー ](/help/user-guide/content/customize-template.md#content-placeholders) の形式が有効であることを確認します。 |
| グループが割り当てられていません | 複数グループのメールテンプレートの画像フィールドがグループに割り当てられていない。 | セクション接頭辞が一貫して使用されているかどうかをチェックします。 各 [ セクション ](/help/user-guide/content/customize-template.md#sections-or-groups) は、各フィールドタイプ（`headline`、`body`、`cta`）の 1 つのみ `image` 使用できます。 `image` フィールドをテンプレート内の有効なグループに割り当てます。 |
| 画像がありません | 必須の画像フィールドがありません。 | メタ、ディスプレイ、バナー広告など、特定のテンプレートタイプには 1 つの `image` フィールドのみが必要です。 必須の `image` フィールドをテンプレートに追加します。 |
| 無効な単一グループ | メールテンプレートには、1 つのグループのみが含まれていますが、これは無効です。 | 基本のメールテンプレートには、テンプレート要素のセットが 1 つ含まれます。これらのテンプレート要素は、「[ セクションまたはグループ ](/help/user-guide/content/customize-template.md#sections-or-groups) で定義されているグループ命名規則を必要としません。 グループの命名構文を削除して、テンプレートにセクションがゼロになるように調整します。 |
| フィールドなし | テンプレートにフィールドが含まれていません。 | GenStudio for Performance Marketingで特定のタイプのコンテンツを生成する必要がある場合は、Handlebars 構文を使用して [ 認識されたフィールド名 ](/help/user-guide/content/customize-template.md#recognized-field-names) をテンプレートに追加します。 |
| 必要なプロパティがありません | 必要なメタデータプロパティの一部が欠落しています。 | 各テンプレートタイプには、チャネルガイドラインに基づく要件と制約があります。 例えば、Meta には縦横比が必要で、ディスプレイ広告にはディメンションが必要です。 [ チャネル固有のテンプレートガイドラインに従う ](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines)。 |
| 使用された予約名 | 禁止されたまたは予約済みのフィールド名が使用されています。 | `subject` や `introductory_text` などの特定の [ フィールド名 ](/help/user-guide/content/customize-template.md#recognized-field-names) は予約されています。 予約済みの名前または禁止された名前を使用するフィールドの名前を変更します。 |
| フィールドが多すぎます | フィールド数がグローバル制限の 20 を超えています。 | 不要なフィールドを削除して、合計が 20 を超えないようにします。 |
| グループが多すぎます | グループの数がチャネルの許可されている上限を超えています。 | Meta、display、および LinkedIn テンプレートでは、複数のセクションを使用できません。 メールでは、2 つまたは 3 つのセクションを定義する際に、グループの名前が必要です。 [ チャネルの要件 ](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) を満たすように、テンプレート内のグループの数を減らします。 |
| サポートされていないフィールド | チャネルがサポートしないフィールドをテンプレートが使用しています。 | [ 認識されたフィールド名 ](/help/user-guide/content/customize-template.md#recognized-field-names) に従って、サポートされていないフィールドを置き換えるか、削除します。 |
