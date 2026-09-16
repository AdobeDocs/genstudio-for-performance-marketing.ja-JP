---
title: ライセンス認証の管理
description: Adobe GenStudio for Performance Marketingでアクティベートされたエクスペリエンスを管理する方法をご紹介します。
feature: Ad Activation
exl-id: 7cf340d4-37ab-4906-9aad-088a26db0818
TQID: https://experienceleague.adobe.com/ird0IiW8L5Axjj2FmEjlUcD1sPaNCNfxj9XNqGfQWiI
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%
---
# アクティブ化の管理

アクティブ化テーブルが[!DNL Activate] ランディングページに表示されます。 各表には、広告とそのステータスが一覧表示されます。

| ステータス | 意味 |
|---|---|
| [!UICONTROL 要注意] | アクティベーションテーブル内の少なくとも1つの広告に、互換性のないcall to actionや重複したトラッキング IDなど、見つからないフィールドまたは無効なフィールドがあります。 |
| [!UICONTROL &#x200B; アクティベートの準備完了] | アクティベーションテーブル内のすべての広告が検証に合格し、公開する準備ができました。 |
| [!UICONTROL 保留中] | アクティブ化テーブル全体が送信され、宛先プラットフォームで処理されています。 |
| [!UICONTROL 公開済み] | アクティベーションテーブル全体が正常に公開されました。 |
| [!UICONTROL 失敗] | 宛先プラットフォームは、テーブル内の広告の少なくとも1つを拒否しました。 ステータスツールヒントにカーソルを合わせると、プラットフォームのエラーメッセージが表示されます。 |

右上の&#x200B;**[!UICONTROL 再試行]**&#x200B;をクリックすると、失敗したアクティベーションを自動的に再試行できます。

公開された行は再送信からロックされ、宛先プラットフォームのネイティブ広告マネージャーに広告へのディープリンクが含まれるため、直接移動してレビューまたはローンチできます。

## 詳細ビュー

広告行をクリックすると、そのアクティベーションの詳細に関するフォーカスされたビューが開きます。 読み取り専用の詳細ビューには、GenStudio for Performance Marketingと宛先プラットフォームの両方から得られた情報を使用して、失敗したアクティベーションを含む、アクティベートされた広告の定義に関する詳細が表示されます。

* **公開日時**：宛先プラットフォームからの公開日時
* **広告ID**：宛先プラットフォームによって割り当てられ、追跡に使用されるIDで、プラットフォームのネイティブ広告マネージャーで公開された広告へのディープリンクが含まれています
* **広告の詳細**：広告に使用される承認済みアセット、コピー、メタデータ
* **プラットフォーム設定**：広告のアクティベートに使用するアカウント、キャンペーン、その他のプラットフォーム設定フィールド

失敗したアクティベーションの詳細ビューには、失敗の理由が含まれます。
