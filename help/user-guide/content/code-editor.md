---
title: テンプレートコードエディター
description: GenStudio for Performance Marketingのテンプレートコードエディターの使用方法を説明します。
level: Intermediate
role: Developer
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
source-git-commit: 8a5d15df7a347c4ee7767610fc9bb23fc7b71db4
workflow-type: tm+mt
source-wordcount: '311'
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
