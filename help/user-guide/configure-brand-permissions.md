---
title: 割り当て  [!DNL Brand]  権限
description: GenStudio for Performance Marketingの作成者と編集者に権限を割り当てる方法  [!DNL Brand]  ついて説明します。
level: Intermediate
feature: Brands Service, Generative AI
source-git-commit: 3c391753ebd0d19ad7dcb17870915eeccc55cc05
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 1%

---

# [!DNL Brand] 権限の割り当て

デフォルトでは、GenStudio システム管理者が [!DNL Brands] を作成および編集できます。 コンテンツ編集者および共同作業者の役割には、編集権限と作成権限がありますが、システム管理権限は必要ない場合があります。 コンテンツエディターと共同作業者にこれらの [!DNL Brand] 関連の権限を付与するには、Adobeシステム管理者がAdobe Admin Consoleで追加の設定タスクを実行する必要があります。 _Enterprise and Teams 管理ガイド_ の [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html#Overview) を参照してください。

ユーザーとユーザーグループの追加は、すべてのAdobe製品に共通する基本的なタスクであり、Admin Consoleを通じて管理される資格を持っています。 ユーザー管理の概要とユーザーおよびユーザーグループを追加する手順については、{Enterprise and Teams 管理ガイド _の_ 0}Adobe Admin Console ユーザー ](https://helpx.adobe.com/jp/enterprise/using/users.html) を参照してください。[

## 手順 1：ユーザーグループの作成

**ユーザーグループを作成するには**:

1. Admin Consoleーにログインし、**[!UICONTROL ユーザー]**/**[!UICONTROL ユーザーグループ]** に移動します。

1. **[!UICONTROL 新規ユーザーグループ]** をクリックします。 _新規ユーザーグループを作成_ ポップアップが開きます。

1. 「**[!UICONTROL ユーザーグループ名]**」フィールドに情報のユーザーグループ名を追加して、新しいグループの目的を識別します。 例えば、「ブランドマネージャー」と入力します。

1. オプションで、グループとその目的の説明を追加します。

1. 「**[!UICONTROL 保存]**」をクリックします。Admin Consoleを実行すると、_新規グループ_ ポップアップが開き、新しく作成したグループの名前が表示されます。

[ エンタープライズおよびチーム管理ガイド ](https://helpx.adobe.com/jp/enterprise/using/user-groups.html) の _ユーザーグループの管理_ を参照してください。

## 手順 2：ユーザーグループへのGenStudio System Manager プロファイルの割り当て

新しいユーザーグループを作成してユーザーを追加したら、**Adobe GenStudioシステムマネージャー** プロファイルをこのグループに割り当てることができます。 割り当てられたプロファイルに関連付けられた使用権限は、このグループ内のすべてのユーザーにGenStudio [!DNL Brands] 権限（ブランドの作成、更新、削除）を付与します。

**プロファイルをユーザーグループに割り当てるには**:

1. 新しく作成されたユーザーグループに移動し、「_割り当てられた製品プロファイル_」タブをクリックします。

1. 「_割り当てられた製品プロファイル_」タブで、「**[!UICONTROL プロファイルを割り当て]**」をクリックします。 _製品とプロファイルを割り当て_ ポップアップが開きます。

1. _製品を選択_ リストから「`Adobe GenStudio`」を選択します。

1. **[!UICONTROL 適用]** をクリックします。 _製品プロファイルを選択_ ポップアップが開き、Adobe GenStudioに関連付けられた製品プロファイルが表示されます。

1. 「`Adobe GenStudio system manager`」を選択します。

1. **[!UICONTROL 適用]** をクリックします。 _製品とプロファイルを割り当て_ ポップアップが開き、新しく作成したユーザーグループの製品プロファイルが表示されます。

1. **[!UICONTROL 保存]**&#x200B;をクリックします。

[ エンタープライズおよびチーム管理ガイド ](https://helpx.adobe.com/jp/enterprise/using/user-groups.html) の _ユーザーグループへの製品プロファイルの割り当て_ を参照してください。

## 手順 3:[!DNL Brands] プロジェクトの作成

_プロジェクト_ は、選択したユーザーがアセット（この場合はアセット）を保存できるストレージの場所 [!DNL Brands] 提供します。

**「_ストレージ_」タブから [!DNL Brands] プロジェクトを作成するには**:

1. Admin Consoleの「_ストレージ_」タブに移動します。

1. サイドナビゲーションで **[!UICONTROL プロジェクト]** をクリックします。 「_プロジェクト_」タブが開きます。

1. **[!UICONTROL プロジェクトを作成]** をクリックします。 _新規プロジェクト_ ポップアップが開きます。

1. 「プロジェクト名」フィールドに「`Adobe GenStudio Brands`」と入力します。 ここに表示されているとおりに、このプロジェクト名を入力してください。 余分なスペースを含めたり、大文字と小文字を変更したりしないでください。

1. 「**[!UICONTROL 作成]**」をクリックします。_プロジェクトに招待_ ポップアップが開きます。

[ エンタープライズおよびチーム管理ガイド ](https://helpx.adobe.com/enterprise/using/projects-in-business-storage.html) の _プロジェクトの管理_ を参照してください。

## 手順 4：ユーザーグループをプロジェクトに招待

これで、作成したユーザーグループを `Adobe GenStudio [!DNL Brands]` プロジェクトに追加する準備が整いました。

**新しく作成したプロジェクトにユーザーグループを招待するには**:

1. _プロジェクトに招待_ ポップアップから、作成したユーザーグループをこのプロジェクトに追加します。

1. 「**編集可能** 権限オプションを選択します。

1. **[!UICONTROL 招待]** をクリックします。

## 手順 5：ユーザーグループへのユーザーの追加

ユーザーにア [!DNL Brands] ットの作成、編集、公開の権限を割り当てるには、新しく作成したユーザーグループにユーザーを追加します。

**ユーザーグループにユーザーを追加するには**:

1. _Admin Console_ から、**[!UICONTROL ユーザー]**/**[!UICONTROL ユーザーグループ]** に移動します。

1. 前に作成したユーザーグループの名前を選択します。 _このユーザーグループにユーザーを追加_ ポップアップが開きます。

1. ユーザー名またはメールアドレスで、新規または既存のユーザーを追加します。 ユーザーグループの管理については、[ エンタープライズおよびチーム管理ガイド ](https://helpx.adobe.com/jp/enterprise/using/user-groups.html) の _ユーザーグループの管理_ を参照してください。

ユーザーは、グループに追加されると、Adobe GenStudioシステム管理者の [!DNL Brand] の作成、編集、公開権限を付与されます。 また、Adobe GenStudio for Performance Marketing [!DNL Brands] プロジェクトを編集するための招待メールも自動送信されます。