---
title: Adobe GenStudio for Performance Marketingのプロビジョニング
description: GenStudio for Performance Marketing製品のプロビジョニングについて説明します。
level: Beginner
feature: Generative AI
role: Admin
exl-id: 7a9f8de1-79e7-455c-ae0f-e7646febc483
TQID: https://experienceleague.adobe.com/cAOdJx0J4GtlITBp0dd-gJqDwM55ynoZNfN2eYWd5SI
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 473
ht-degree: 1%

---

# Adobe GenStudio for Performance Marketingのプロビジョニング

Adobe システム管理者は、[Adobe Admin Console](https://helpx.adobe.com/jp/enterprise/using/admin-console.html#Overview)で初期プロビジョニング タスクを実行します。 Admin Consoleから、Adobe システム管理者はGenStudio製品プロファイルにアクセスし、使用可能な製品ライセンスをユーザーに割り当てることができます。

>[!NOTE]
>
>Adobe Admin Consoleへのアクセスを必要とするイネーブルメントタスクを実装できるのは、Adobe システム管理者のみです。

>[!IMPORTANT]
>
>既存の製品プロファイルを新規に追加したり、編集または削除したりしないでください。 デフォルトの製品プロファイルを変更すると、GenStudio for Performance Marketingのデプロイメントが大幅に中断される可能性があります。

## 手順1:Adobe Admin Consoleで製品プロファイルにアクセスする

Admin Consoleでは、商品プロファイルは、GenStudio for Performance Marketing内でのブランドおよびキャンペーンの作成と管理に固有のルールとユーザープロファイルを定義します。

**GenStudio製品プロファイルにアクセスするには**

1. ウェルカムメールの&#x200B;**開始** リンクをクリックして、[Adobe Admin Console](https://helpx.adobe.com/jp/enterprise/using/admin-console.html#Overview)に移動します。

1. Adobe IDを使用してAdmin Consoleにログインします。

   ログインが成功すると、Adobe Admin Consoleの「_概要_」タブが表示されます。

1. 「_製品_」タブに移動します。 このタブには、組織が購入したすべてのAdobe製品が表示されます。

1. 商品リストから「**[!UICONTROL GenStudio]**」を選択します。 コンソールにはGenStudio製品プロファイルが表示され、組織が購入した製品ライセンスに関する重要な情報が表示されます。 また、これらのライセンスを管理するオプションも用意されています。

これで、GenStudio for Performance Marketingにユーザーを（プロビジョニング）にライセンスを割り当てる準備が整いました。 間違った組織にログインした場合は、ユーザーに使用権限を割り当てる前に、正しい組織に切り替えてください。 組織を変更するには、右上隅にある組織名をクリックし、**GenStudio**&#x200B;組織を選択します。

## 手順2：ユーザーのプロビジョニング

Admin Consoleでのユーザーのプロビジョニングは、ユーザーに製品ライセンスを割り当てるプロセスです。 これらのユーザーは、製品プロファイルで指定されたIMS組織に属している必要があります。 他のAdobe製品にユーザーをプロビジョニングする場合と同様に、GenStudio for Performance Marketing組織にユーザーをプロビジョニングできます。 ユーザーを手動で追加することも、ユーザーを一括で読み込むこともできます。

>[!TIP]
>
>GenStudio for Performance Marketingでシステム管理タスクを実行するために、GenStudio system managerの使用権限を割り当てます。

**前提条件**:

最初に基本的な情報を特定して、プロビジョニングの準備を行います。

* 氏名（名）
* 企業のメールアドレス
* ユーザーを割り当てる使用権限のタイプ

GenStudio for Performance Marketing ユーザーロールの割り当てについて詳しくは、[&#x200B; ユーザーロールと権限](user-roles.md)を参照してください。

ユーザーを個別に追加することも、複数のユーザーのアカウント情報をインポートすることもできます。

* [ユーザーを個別に管理](https://helpx.adobe.com/jp/enterprise/using/manage-users-individually.html#add-users)

* [複数ユーザーの管理/CSVの一括アップロード](https://helpx.adobe.com/jp/enterprise/using/bulk-upload-users.html)

組織のGenStudio for Performance Marketingにユーザーをオンボーディングすると、GenStudio system managerは[組織のブランドガイドラインとメディアガイドラインを設定できます](get-started.md)。
