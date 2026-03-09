---
title: アセットの詳細
description: Adobe GenStudio for Performance Marketingでは、検索性とパフォーマンストラッキングのために、リッチなメタデータを使用して承認済みコンテンツを格納します。
feature: Generative AI, Content Attributes, Content Management
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
TQID: https://experienceleague.adobe.com/Hm7qcrP6VcXf6IqZ2pYybduNyjjV8kdWj571gcRpglI
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: c95c94c1-727b-457a-9184-a4dda4c95ab2id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f321b88b-6bb7-49cc-a16a-ae2b665ebd32id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2: id: a8b28c00-da6e-4d27-8667-80f790ad8972id: a98e0185-3180-4e8c-8f31-f72af4cc21a2id: b03d2162-d906-40a0-9cbd-001391e22d4aid: dd48f9df-f2e2-49fe-a918-332a8e240ffeid: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eb30f47f-d87a-400f-8f78-63ce7979ff56
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 732
ht-degree: 1%

---

# アセットの詳細

Adobe GenStudio for Performance Marketingでは、検索性とパフォーマンストラッキングのために、リッチなメタデータを使用して承認済みコンテンツを格納します。

各アセット（エクスペリエンスとテンプレートを含む）には、コンテンツのパフォーマンスを識別、追跡、使用および学習するのに役立つ _詳細_ （メタデータ）が関連付けられています。

**アセットの詳細を表示するには**:

1. _[!DNL Content]_で、アセット、エクスペリエンスまたはテンプレートを選択します。 アセットをクリックすると、そのアセットのフォーカスされたビューが開きます。

1. アセット表示で、右側の _[!UICONTROL 詳細]_ セクションを確認します。

1. 「_[!UICONTROL 詳細]_」セクションが表示されない場合は、「**[!UICONTROL 情報]** （i）」アイコンをクリックします。

アセットの詳細には、作成またはアップロード処理中に適用されたメタデータが含まれます。 アセットメタデータタイプには、[ システムメタデータ ](#system-metadata) および [ ユーザー定義メタデータ ](#user-defined-metadata) が含まれます。

次の画像アセットには、ファイルタイプ、サイズ、その他の特性、1 つのユーザー定義キーワード、AI によって検出された複数の属性と色を記述したシステムメタデータが含まれています。

![ 複数のタグを持つアセットの詳細 ](/help/assets/content-asset-details.png)

>[!NOTE]
>
AEM リポジトリからのAssetsには、異なるメタデータが表示されます。 アセットの詳細を設定する方法については、[ アセットの表示の設定 ](connect-aem-repo.md#step-4-configure-asset-visibility) を参照 [!DNL AEM Assets Content Hub] てください。

## システムメタデータ

ファイルタイプ、サイズ、サイズ、サイズ、ソースなど、アセットがアップロードされると、一部のアセットメタデータが自動的に収集されます。 ファイル名以外は、デフォルトのシステムメタデータを編集できません。

### 生成されたタグ

承認済みのアセットを [!DNL Content] に保存すると、GenStudio for Performance MarketingはAdobeの AI と機械学習機能を使用してアセットを調査し、アセットの機能に基づいてタグを適用します。 例えば、猫の画像では、`pet photography` や `cat` などの属性タグや、画像内で支配的な色を識別するカラータグが生成される場合があります。 検出され、自動的に適用されたタグは編集できません。

画像、ビデオおよびテキスト機能の詳細なリストについては、[!DNL Insights] 属性カテゴリ ](/help/user-guide/insights/attributes.md#categories) を参照してください [ 属性カテゴリ）。

### 生成されたコンテンツメタデータ

新しいアセットやエクスペリエンスの生成に使用する情報は、使用されたプロンプトなどのメタデータになります。 コンテンツが承認されると、プロンプトは編集できませんが、新しいコンテンツを生成するための出発点として使用できます。

## ユーザー定義のメタデータ

ユーザー定義メタデータは、アセットのコンテンツにマーケティングコンテキストを追加するので、マーケターはアセットの使用方法とエンゲージメント方法を理解できます。

[ アセットをアップロード ](/help/user-guide/content/manage-assets.md#add-assets) する際に、GenStudio for Performance Marketingにメタデータとして存在する一連のオプションのアセット詳細を定義できます。 さらに詳細を含めると、検索とフィルタリングでのアセットの識別が向上します。

**ユーザー定義のメタデータを編集するには**:

1. _[!DNL Content]_で、アセット、エクスペリエンスまたはテンプレートを選択します。 アセットをクリックすると、そのアセットのフォーカスされたビューが開きます。

1. アセット表示で、右側の _[!UICONTROL 詳細]_ セクションを確認します。

1. **[!UICONTROL 詳細を編集]** （鉛筆）をクリックして、アセット、エクスペリエンスまたはテンプレートのメタデータを編集します。

   提供する情報が多いほど、GenStudio for Performance Marketingの堅牢な機能を体験できます。 リストから 1 つ以上の詳細を選択するか、必要に応じて新しい詳細（キーワードを使用するなど）を入力します。 追加した各詳細は、リストの下に表示されます。 詳細を削除するには、「**`x`**」をクリックします。

### メタデータの詳細

次の表に、アセット作成時に定義できるメタデータ（アセットの詳細）を示します。

| フィールド | 説明 |
| -------------- | ----------- |
| タイトル | アセットの名前。デフォルトのタイトルは元のファイル名にすることができます |
| [!DNL Campaigns] | ビジネス目標を達成 [[!DNL Campaigns]](/help/user-guide/campaigns/overview.md) るために、一貫したメッセージを含んだプロモーションコンテンツを含めます <br> キャンペーンリンクをクリックすると、キャンペーンの概要ページに移動します |
| [!DNL Brands] | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) がGenStudio for Performance Marketingに追加され、使用するために公開されました |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md) がGenStudio for Performance Marketingに追加されて使用されるようになりました |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md) がGenStudio for Performance Marketingに追加されて使用されるようになりました |
| チャネル | メール、バナー、ディスプレイ広告など、特定のコンテンツタイプを配信するプラットフォーム |
| [!UICONTROL  期間 ] | 四半期、シーズン、年など、アセットを使用する時間枠。例：`Winter 2023` |
| 地域 | アセットが使用される地域。 例：`North America`, `APAC`, `Italy` |
| 言語 | アセットを使用する言語。 例：`Spanish` |
| キーワード | ユーザー定義のキーワードは、アセットの特徴や目的をさらに特定するために使用されます |

>[!TIP]
>
**[!UICONTROL 詳細を編集]** （鉛筆）をクリックして、アセットのメタデータを編集します。 例えば、アセット名を変更したり、キーワードを追加または削除したりできます。

## 生成コンテキスト

[!UICONTROL  生成コンテキスト ] セクションには、エクスペリエンスプロセス中に使用された `Prompt` など、エクスペリエンスの生成に使用された情報が表示 [!DNL Create] れます。 このinsightは、より成功したバリアントを作成するのに役立つ場合があります。

情報には次が含まれる場合があります。

- [!DNL Create] のプロセス中に選択された `Brand`、`Product`、および `Persona` のパラメーター
- メールエクスペリエンスの `Subject line` と `Preheader`
- Meta広告の `Headline` と `Body`

## 履歴

エクスペリエンスの _[!UICONTROL 履歴]_ セクションを展開すると、承認とアクティビティのタイムラインが表示されます。 例えば、承認されたエクスペリエンスには、承認日、時刻、承認者が表示されます。

```
Approved

December 10, 2024 at 6:00 PM by Username
```
