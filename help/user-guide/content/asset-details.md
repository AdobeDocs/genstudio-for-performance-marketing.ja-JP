---
title: アセットの詳細
description: Adobe GenStudio for Performance Marketingでは、検索性とパフォーマンストラッキングのために、リッチなメタデータを使用して承認済みコンテンツを格納します。
feature: Attributes, Assets
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: a2c2a39a8ed69a36c7126312ac42f6e02dd0598e
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 1%

---

# アセットの詳細

Adobe GenStudio for Performance Marketingでは、検索性とパフォーマンストラッキングのために、リッチなメタデータを使用して承認済みコンテンツを格納します。

各アセット（エクスペリエンスとテンプレートを含む）には、コンテンツのパフォーマンスを識別、追跡、使用および学習するのに役立つ _詳細_ （メタデータ）が関連付けられています。

**アセットの詳細を表示するには**:

1. _[!DNL Content]_で、アセット、エクスペリエンスまたはテンプレートを選択します。 アセットをクリックすると、そのアセットのフォーカスされたビューが開きます。

1. アセット表示で、右側の _[!UICONTROL 詳細]_ セクションを確認します。

   >[!TIP]
   >
   >「_[!UICONTROL 詳細]_」セクションが表示されない場合は、「**[!UICONTROL 情報]** （i）」アイコンをクリックします。

   アセットの詳細には、作成またはアップロード処理中に適用されたメタデータが含まれます。 アセットメタデータタイプには、[ システムメタデータ ](#system-metadata) および [ ユーザー定義メタデータ ](#user-defined-metadata) が含まれます。

>[!NOTE]
>
>AEM リポジトリからのAssetsには、異なるメタデータが表示されます。 アセットの詳細を設定する方法については、[ アセットの表示の設定 ](connect-aem-repo.md#step-4-configure-asset-visibility) を参照 [!DNL AEM Assets Content Hub] てください。

## Express で編集

Adobe Expressを使用して、GenStudio for Performance Marketing内で画像アセット（JPGまたは PNG）を直接編集できます。 _[!UICONTROL Adobe Expressを利用]_ キャンバスには、GenStudio アプリケーションを離れることなく画像を強化できる便利な機能が用意されています。 背景の削除、ジェネレーティブフィルの適用、エフェクトの調整、画像の切り抜きを簡単に行うことができます。

>[!BEGINSHADEBOX]

[!DNL Edit in Adobe Express] の機能を使用して画像を強化するための条件：

- サポートされる MIME タイプには `image/png` と `image/jpeg` があります
- 画像の最小寸法は 50 x 50 ピクセルです
- 画像の最大サイズは 8000 x 8000 ピクセルです
- 最大サイズは 40 MB （40,000,000 バイト）です

>[!ENDSHADEBOX]

**Express でアセットを編集するには**:

1. _[!DNL Content]_で、画像アセットを選択します。 アセットをクリックすると、そのアセットのフォーカスされたビューが開きます。

1. アセットビューで、右上の **[!UICONTROL Adobe Expressで編集]** アイコンをクリックします。

1. _[!UICONTROL Powered by Adobe Express]_ キャンバスで、左側のパネルの Express コントロールを使用して、画像を強調します。

1. 更新された画像が気に入ったら、右上の **[!UICONTROL コピーを保存]** をクリックします。

1. ファイル形式（JPGまたは PNG）を選択し、「**[!UICONTROL コピーを保存]**」をクリックします。

1. _[!UICONTROL アセットのコピーを保存]_ ポップアップで **[!UICONTROL アセット名]** を更新します。

   - **[!UICONTROL 元のアセットと同じ詳細]** を選択して、アセットの詳細を新しい画像に引き継ぎます。

   - 「**[!UICONTROL 詳細]**」セクションを展開すると、キャンペーン、ガイドライン、その他のメタデータを更新できます。

   >[!TIP]
   >
   >提供する情報が多いほど、GenStudio for Performance Marketingの堅牢な機能を体験できます。 リストから 1 つ以上の詳細を選択するか、必要に応じて新しい詳細（キーワードを使用するなど）を入力します。 追加した各詳細は、リストの下に表示されます。 詳細を削除するには、「**`x`**」をクリックします。

1. **[!UICONTROL 保存]**&#x200B;をクリックします。

## システムメタデータ

アセットのアップロード時に、一部のアセットメタデータが自動的に収集されます。 デフォルトのシステムメタデータは編集できません。

アセットに対して保存および取得されるデフォルトのメタデータには、ファイルの名前、寸法、ソースなどがあります。

### 生成されたタグ

承認済みのアセットを [!DNL Content] に保存すると、GenStudio for Performance MarketingはAdobeの AI および機械学習機能を使用してアセットを調査し、アセット機能に基づいてタグを適用します。 例えば、猫の画像では、`pet photography` や `cat` などの属性タグや、画像内で支配的な色を識別するカラータグが生成される場合があります。 検出され、自動的に適用されたタグは編集できません。

画像、ビデオおよびテキスト機能の詳細なリストについては、[!DNL Insights] 属性カテゴリ ](/help/user-guide/insights/attribute-category.md) を参照してください [ 属性カテゴリ）。

### 生成されたコンテンツメタデータ

新しいアセットやエクスペリエンスの生成に使用する情報は、使用されたプロンプトなどのメタデータになります。 コンテンツが承認されると、プロンプトは編集できませんが、新しいコンテンツを生成するための出発点として使用できます。

## ユーザー定義のメタデータ

ユーザー定義メタデータは、アセットのコンテンツにマーケティングコンテキストを追加するので、マーケターはアセットの使用方法とエンゲージメント方法を理解できます。

[ アセットをアップロード ](/help/user-guide/content/manage-assets.md#add-assets) する際に、GenStudio for Performance Marketingにメタデータとして存在する一連のオプションのアセット詳細を定義できます。 さらに詳細を含めると、検索とフィルタリングでのアセットの識別が向上します。

### メタデータの詳細

次の表に、アセットの作成時に定義できるメタデータ（アセットの詳細）を示します。

| フィールド | 説明 |
| ------------- | ----------- |
| キャンペーン（プロジェクト名） | アセットと共にキャプチャおよび保存されるデフォルトのメタデータ |
| [!DNL Brands] | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) がGenStudio for Performance Marketingに追加され、使用するために公開されました |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md) がGenStudio for Performance Marketingに追加されて使用されるようになりました |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md) がGenStudio for Performance Marketingに追加されて使用されるようになりました |
| チャネル | メールやメタ広告など、アセットが使用されるGenStudio for Performance Marketingのコンテンツタイプ |
| 期間 | 四半期、シーズン、年など、アセットを使用する期間。 例：`Winter 2023` |
| 地域  | アセットが使用される地域。 例：`North America`, `APAC`, `Italy` |
| 言語 | アセットを使用する言語。 例：`Spanish` |
| キーワード | 資産の特性や目的の絞り込みに活用するキーワード |

<!-- ## History

Expand the _[!UICONTROL History]_ section to view a timeline of approvals and activity.

list other activity, show screenshot?
-->
