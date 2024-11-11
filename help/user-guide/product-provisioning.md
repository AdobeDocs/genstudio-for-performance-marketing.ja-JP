---
title: Adobe GenStudio for Performance Marketingのプロビジョニング
description: GenStudio for Performance Marketing製品のプロビジョニングについて説明します。
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: 7a9f8de1-79e7-455c-ae0f-e7646febc483
source-git-commit: 0998362a50c63958e331796fd1deebd61f170d2e
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# Adobe GenStudio for Performance Marketingのプロビジョニング

Adobeシステム管理者は、[Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html#Overview) で初期プロビジョニングタスクを実行します。 Admin Consoleから、Adobeシステム管理者はGenStudio製品プロファイルにアクセスし、使用可能な製品ライセンスをユーザーに割り当てることができます。

>[!NOTE]
>
>Adobe Admin Console アクセスを必要とするイネーブルメントタスクを実装できるのは、Adobeシステム管理者のみです。

## 手順 1:Adobe Admin Consoleで製品プロファイルにアクセスする

Admin Console内で、製品プロファイルは、GenStudio for Performance Marketing内でのブランドおよびキャンペーンの作成と管理に固有のルールとユーザープロファイルを定義します。

**GenStudio製品プロファイルにアクセスするには**

1. お知らせメールの **使用を開始** リンクをクリックして、[Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html#Overview) に移動します。

1. Adobe IDを使用してAdmin Consoleにログインします。

   ログインに成功すると、Adobe Admin Consoleの「_概要_」タブが表示されます。

1. 「_製品_ タブに移動します。 このタブには、組織が購入したすべてのAdobe製品が表示されます。

1. 商品のリストから ]**0}GenStudio} を選択します。**[!UICONTROL &#x200B;コンソールには、GenStudio製品プロファイルが表示されます。このプロファイルには、組織が購入した製品ライセンスに関する主要な情報が表示されます。 また、これらのライセンスを管理するオプションも提供されます。

これで、GenStudio for Performance Marketingのユーザーにライセンスを割り当てる（プロビジョニングする）準備が整いました。 誤った組織にログインした場合は、正しい組織に切り替えてから、ユーザーに使用権限を割り当てようとします。 組織を変更するには、右上隅の組織名をクリックし、**GenStudio** 組織を選択します。

## 手順 2：ユーザーをプロビジョニングする

Admin Consoleでのユーザーのプロビジョニングは、ユーザーに製品ライセンスを割り当てるプロセスです。 これらのユーザーは、製品プロファイルで指定されている IMS 組織に属している必要があります。 ユーザーを他のAdobe製品にプロビジョニングするのと同じ方法で、GenStudio for Performance Marketing組織にユーザーをプロビジョニングできます。 ユーザーを手動で追加することも、ユーザーを一括で読み込むこともできます。

>[!TIP]
>
>GenStudio for Performance Marketingでシステム管理タスクを実行するには、自分自身にGenStudio システムマネージャーの権限を割り当てます。

**前提条件**:

プロビジョニングの準備を行うには、まず基本情報を特定します。

* 姓と名
* 会社のメールアドレス
* ユーザーを割り当てる使用権限のタイプ

GenStudio for Performance Marketing ユーザーの役割を割り当てる方法については、[ ユーザーの役割と権限 ](user-roles.md) を参照してください。

ユーザーを個別に追加することも、複数のユーザーのアカウント情報を読み込むこともできます。

* [ ユーザーを個別に管理 ](https://helpx.adobe.com/enterprise/using/manage-users-individually.html#add-users)

* [ 複数のユーザーの管理/CSV の一括アップロード ](https://helpx.adobe.com/jp/enterprise/using/bulk-upload-users.html)

組織のGenStudio for Performance Marketingにユーザーをオンボーディングしたら、Genstudio システムマネージャーは [ 組織のブランドとメディアのガイドラインを設定 ](get-started.md) できます。
