---
title: ブランド権限の設定
description: GenStudio for Performance Marketing [!DNL Brand] の作成者と編集者に対する使用権限の割り当てについて説明します。
level: Intermediate
feature: Brand Personalization, Generative AI
exl-id: fc33ecd3-4403-4045-87af-012a0377226c
TQID: https://experienceleague.adobe.com/13RaDoLWSm8KjpzgsMkxAUOULez15KTUj6xF3QSb3vE
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 742
ht-degree: 4%

---

# [!DNL Brand]権限の割り当て

デフォルトでは、GenStudio システム管理者は[!DNL Brands]を作成および編集できます。 コンテンツエディターと共同作業者の役割には編集と作成の権限がありますが、システム管理の権限は必要ありません。

これらの[!DNL Brand]関連の使用権限をコンテンツエディターおよび共同作業者に付与するには、Adobe システム管理者がAdobe Admin Consoleでさらに設定タスクを実行する必要があります。 _Enterprise and Teams管理ガイド_&#x200B;の[Adobe Admin Console](https://helpx.adobe.com/jp/enterprise/using/admin-console.html#Overview)を参照してください。

ユーザーとユーザーグループの追加は、Admin Consoleを通じて管理される使用権限を持つすべてのAdobe製品に共通する基本的な作業です。 ユーザー管理の概要とユーザーとユーザーグループを追加する手順については、_Enterprise and Teams管理ガイド_&#x200B;の[Adobe Admin Console ユーザー](https://helpx.adobe.com/jp/enterprise/using/users.html)を参照してください。

このビデオのチュートリアルを見るか、以下の手順に従います。

>[!VIDEO](https://video.tv.adobe.com/v/3474998?captions=jpn&learn=on&enablevpops)

## 手順1：ユーザーグループの作成

**ユーザーグループを作成するには**:

1. Admin Consoleにログインし、**[!UICONTROL Users]** > **[!UICONTROL Users Groups]**&#x200B;に移動します。

1. **[!UICONTROL 新規ユーザーグループ]**&#x200B;をクリックします。 _新しいユーザーグループを作成_ ポップアップが開きます。

1. 新しいグループの目的を特定するために、**[!UICONTROL ユーザーグループ名]** フィールドに有益なユーザーグループ名を追加します。 例えば、「ブランドマネージャー」と入力します。

1. 必要に応じて、グループとその目的の説明を追加します。

1. 「**[!UICONTROL 保存]**」をクリックします。 Admin Consoleは、新しく作成されたグループの名前が付いた&#x200B;_新しいグループ_ ポップアップを開きます。

_エンタープライズおよびTeams管理ガイド_&#x200B;の「[&#x200B; ユーザーグループの管理](https://helpx.adobe.com/jp/enterprise/using/user-groups.html)」を参照してください。

## 手順2:GenStudio system manager プロファイルをユーザーグループに割り当てる

新しいユーザーグループを作成してユーザーを追加したら、このグループに&#x200B;**Adobe GenStudio system manager** プロファイルを割り当てることができます。 割り当てられたプロファイルに関連付けられている権限は、このグループ GenStudio [!DNL Brands]のすべてのユーザーに権限を与えます（ブランドの作成、更新、削除）。

**ユーザーグループにプロファイルを割り当てるには**:

1. 新しく作成したユーザーグループに移動し、「_割り当てられた製品プロファイル_」タブをクリックします。

1. 「_割り当てられた製品プロファイル_」タブで、「**[!UICONTROL プロファイルを割り当て]**」をクリックします。 _製品とプロファイルを割り当て_ ポップアップが開きます。

1. 「_製品を選択_」リストから「`Adobe GenStudio`」を選択します。

1. 「**[!UICONTROL 適用]**」をクリックします。 _製品プロファイルを選択_ ポップアップが開き、Adobe GenStudioに関連付けられた製品プロファイルが表示されます。

1. 「`Adobe GenStudio system manager`」を選択します。

1. 「**[!UICONTROL 適用]**」をクリックします。 _製品とプロファイルを割り当て_ ポップアップが開き、新しく作成されたユーザーグループの製品プロファイルが表示されます。

1. 「**[!UICONTROL 保存]**」をクリックします。

_エンタープライズおよびTeams管理ガイド_&#x200B;の「[製品プロファイルをユーザーグループに割り当てる](https://helpx.adobe.com/jp/enterprise/using/user-groups.html)」を参照してください。

## 手順3：ユーザーグループにユーザーを追加する

[!DNL Brands]を作成、編集、公開する権限をユーザーに割り当てるには、新しく作成したユーザーグループにユーザーを追加します。

>[!NOTE]
>
>プロジェクトにグループを追加する前に、少なくとも1人のユーザーをこのユーザーグループに追加する必要があります。

**ユーザーグループにユーザーを追加するには**:

1. _Admin Console_&#x200B;から、**[!UICONTROL Users]** > **[!UICONTROL User Groups]**&#x200B;に移動します。

1. 前に作成したユーザーグループの名前を選択します。 _このユーザーグループにユーザーを追加_ ポップアップが開きます。

1. ユーザー名または電子メールアドレスを使用して、新規または既存のユーザーを追加します。 既存のユーザーの名前またはメールアドレスを入力すると、このIMS組織に属する既知のユーザーの名前に一致する名前がこのフィールドに自動的に入力されます。 ユーザーグループの管理について詳しくは、_エンタープライズおよびTeams管理ガイド_&#x200B;の[&#x200B; ユーザーグループの管理](https://helpx.adobe.com/jp/enterprise/using/user-groups.html)を参照してください。

グループに追加されると、Adobe GenStudio システムマネージャーの[!DNL Brand]の作成、編集、公開権限が付与されます。 また、Adobe GenStudio for Performance Marketing [!DNL Brands] プロジェクトを編集するための招待メールが自動的に送信されます。

## 手順4: [!DNL Brands] プロジェクトの作成

_プロジェクト_&#x200B;は、選択したユーザーがアセットを保存できるストレージの場所（この場合は[!DNL Brands] アセット）を提供します。

**「_ストレージ_」タブ**&#x200B;から[!DNL Brands] プロジェクトを作成するには：

1. Admin Consoleの「_ストレージ_」タブに移動します。

1. サイドナビゲーションの「**[!UICONTROL プロジェクト]**」をクリックします。 「_プロジェクト_」タブが開きます。

1. 「**[!UICONTROL プロジェクトを作成]**」をクリックします。 _新規プロジェクト_ ポップアップが開きます。

1. プロジェクト名フィールドに`Adobe GenStudio Brands`と入力します。 ここに表示されているとおりに、このプロジェクト名を正確に入力します。 余分なスペースを含めたり、大文字と小文字を変更したりしないでください。

1. 「**[!UICONTROL 作成]**」をクリックします。 「_プロジェクトに招待_」ポップアップが開きます。

_エンタープライズおよびチーム管理ガイド_&#x200B;の「[&#x200B; プロジェクトの管理](https://helpx.adobe.com/jp/enterprise/using/projects-in-business-storage.html)」を参照してください。

## 手順5：ユーザーグループをプロジェクトに招待する

これで、作成したばかりのユーザーグループを`Adobe GenStudio [!DNL Brands]` プロジェクトに追加する準備が整いました。

**新しく作成したプロジェクトにユーザーグループを招待するには**:

1. _プロジェクトに招待_ ポップアップから、作成したばかりのユーザーグループをこのプロジェクトに追加します。

1. 「**編集可能**&#x200B;権限」オプションを選択します。

1. **[!UICONTROL 招待]**&#x200B;をクリックします。
