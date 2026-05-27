---
title: アセットの詳細
description: Adobe GenStudio for Performance Marketingは、検索性とパフォーマンスを追跡するために、承認済みコンテンツと豊富なメタデータを保存します。
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

Adobe GenStudio for Performance Marketingは、見つけやすさとパフォーマンス追跡のために、承認済みコンテンツと豊富なメタデータを保存します。

各アセット（エクスペリエンスとテンプレートを含む）には、コンテンツのパフォーマンスを識別、追跡、使用、学習するのに役立つ&#x200B;_詳細_ （メタデータ）が関連付けられています。

**アセットの詳細を表示するには**:

1. _[!DNL Content]_で、アセット、エクスペリエンスまたはテンプレートを選択します。 アセットをクリックすると、アセットの全体像が表示されます。

1. アセットビューで、右側の&#x200B;_[!UICONTROL 詳細]_ セクションを確認します。

1. _[!UICONTROL 詳細]_ セクションが表示されない場合は、**[!UICONTROL 情報]** （i） アイコンをクリックします。

アセットの詳細には、作成またはアップロードプロセス中に適用されたメタデータが含まれます。 アセットのメタデータタイプには、[ システムのメタデータ ](#system-metadata)と[ ユーザー定義のメタデータ ](#user-defined-metadata)が含まれます。

次の画像アセットには、ファイルタイプ、サイズ、その他の特性、1つのユーザー定義キーワード、およびAIが検出したいくつかの属性と色を示すシステムメタデータが含まれています。

![複数のタグを持つアセットの詳細](/help/assets/content-asset-details.png)

>[!NOTE]
>
AEM リポジトリのAssetsには、様々なメタデータが表示されます。 [!DNL AEM Assets Content Hub] アセットの詳細を設定する方法については、[ アセットの表示の設定](connect-aem-repo.md#step-4-configure-asset-visibility)を参照してください。

## システムメタデータ

ファイルの種類、サイズ、ディメンション、ソースなど、アセットをアップロードすると、一部のアセットメタデータが自動的に収集されます。 ファイル名を除き、デフォルトのシステムメタデータを編集することはできません。

### 生成されたタグ

[!DNL Content]に承認済みのアセットを保存する場合、GenStudio for Performance MarketingはAdobeのAIとマシンラーニング機能を使用してアセットを調査し、アセットの機能に基づいてタグを適用します。 例えば、猫の画像では、`pet photography`や`cat`などの属性タグや、画像内の主要な色を識別するカラータグが生成される場合があります。 検出され、自動的に適用されるタグは編集できません。

画像、ビデオ、テキスト機能の詳細なリストについては、[!DNL Insights] [属性カテゴリ ](/help/user-guide/insights/attributes.md#categories)を参照してください。

### 生成されたコンテンツメタデータ

新しいアセットやエクスペリエンスの生成に使用された情報は、使用されたプロンプトなどのメタデータになります。 コンテンツが承認されると、プロンプトを編集することはできませんが、新しいコンテンツを生成するための出発点として使用できます。

## ユーザー定義メタデータ

ユーザー定義のメタデータは、マーケティングコンテキストをアセットのコンテンツに追加し、マーケターがアセットの使用方法を理解してエンゲージできるようにします。

アセットを[ アップロード ](/help/user-guide/content/manage-assets.md#add-assets)すると、GenStudio for Performance Marketingにメタデータとして存在するオプションのアセットの詳細のセットを定義できます。 詳細を含めることで、検索とフィルタリングでアセット識別を向上させることができます。

**ユーザー定義メタデータを編集するには**:

1. _[!DNL Content]_で、アセット、エクスペリエンスまたはテンプレートを選択します。 アセットをクリックすると、アセットの全体像が表示されます。

1. アセットビューで、右側の&#x200B;_[!UICONTROL 詳細]_ セクションを確認します。

1. **[!UICONTROL 詳細を編集]** （鉛筆）をクリックして、アセット、エクスペリエンス、またはテンプレートのメタデータを編集します。

   詳細を確認すればするほど、GenStudio for Performance Marketingの優れた機能をより実感できます。 リストから1つ以上の詳細を選択するか、キーワードなど、該当する場合は新しい詳細を入力します。 追加した各詳細は、リストの下に表示されます。 **`x`**&#x200B;をクリックして詳細を削除します。

### メタデータの詳細

次の表は、アセットの作成時に定義できるメタデータ（アセットの詳細）の詳細です。

| フィールド | 説明 |
| -------------- | ----------- |
| タイトル | アセットの名前。デフォルトのタイトルは元のファイル名です |
| [!DNL Campaigns] | [[!DNL Campaigns]](/help/user-guide/campaigns/overview.md)には、ビジネス目標を達成するための一貫したメッセージを含むプロモーションコンテンツが含まれています<br> キャンペーンリンクをクリックすると、キャンペーンの概要ページに移動します |
| [!DNL Brands] | [[!DNL Brands]](/help/user-guide/guidelines/brands.md)がGenStudio for Performance Marketingに追加され、使用のために公開されました |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md)がGenStudio for Performance Marketingに追加されました |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md)がGenStudio for Performance Marketingに追加されました |
| チャネル | メール、バナー、ディスプレイ広告など、特定のコンテンツタイプを配信するためのプラットフォーム |
| [!UICONTROL  タイムフレーム ] | 四半期、季節、年など、アセットが使用される時間枠。例：`Winter 2023` |
| 地域 | アセットが使用されるリージョン。 例：`North America`, `APAC`, `Italy` |
| 言語 | アセットの使用言語。 例：`Spanish` |
| キーワード | ユーザー定義キーワードは、アセットの特性と目的をさらに特定するために使用します |

>[!TIP]
>
**[!UICONTROL 詳細を編集]** （鉛筆）をクリックして、アセットメタデータを編集します。 例えば、アセット名を変更したり、キーワードを追加または削除したりできます。

## 生成コンテキスト

[!UICONTROL 生成コンテキスト ] セクションには、[!DNL Create] プロセス中に使用された`Prompt`など、エクスペリエンスの生成に使用された情報が表示されます。 このinsightは、さらに効果的なバリエーションを構築するのに役立ちます。

情報には以下が含まれる場合があります。

- [!DNL Create] プロセス中に`Brand`、`Product`および`Persona` パラメーターが選択されました
- `Subject line`および`Preheader`の電子メールエクスペリエンス
- Meta広告の`Headline`および`Body`

## 履歴

エクスペリエンスの「_[!UICONTROL 履歴]_」セクションを展開して、承認とアクティビティのタイムラインを表示します。 たとえば、承認済みのエクスペリエンスでは、承認日、時間、承認者が表示されます。

```
Approved

December 10, 2024 at 6:00 PM by Username
```
