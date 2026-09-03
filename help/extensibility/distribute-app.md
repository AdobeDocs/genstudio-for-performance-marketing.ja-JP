---
title: アプリを配布
description: GenStudio for Performance Marketing用にアプリまたはアドオンを配布します。
feature: Extensibility
exl-id: 4935356b-08df-402c-b1a2-b89627afc188
TQID: https://experienceleague.adobe.com/6SHsqsafwqCWS3dspM65BTVAqZ09WwW2IxF-PIecINE
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 303
ht-degree: 1%

---

# アプリの配布

アドオンを配布することで、組織や他の人がアドオンを利用できるようになります。 配布のワークフローは、このアドオンがパブリック配布とプライベート配布のどちらを対象としているかによって異なります。

このトピックでは、プライベート配布について説明します。 プライベート配布では、アドオンのデプロイメントを、IMS組織によって特定された、アドオンが開発された組織に制限します。

一般公開により、このアドオンはAdobe Exchange上でアプリとして利用可能となります。 _Adobe_&#x200B;開発者向けドキュメントの[ パブリックディストリビューション ](https://developer.adobe.com/app-builder/docs/guides/distribution/public/)では、任意のApp Builder組織でアプリを利用できるようにする方法について説明しています。

>[!BEGINSHADEBOX]

**前提条件**:

次の権限を確認します。

* 承認用にアプリを送信する組織の開発者権限

* アプリを承認するためのシステム管理者の権限

App Builder アプリは、App Builder プロジェクトにデプロイする必要があります。

>[!ENDSHADEBOX]

**アプリをプライベートに配布するには**:

プライベート配信は、あなたのアプリを組織内のメンバーのみが利用できるようにします。

1. [Adobe Developer Console](https://developer.adobe.com/console/)から、アプリがデプロイされている組織、プロジェクト、ワークスペースを選択します。

1. 「_Workspaceの概要_」エリアから「**[!UICONTROL Approval]**」を選択します。 _アプリの承認_ ペインが開きます。

1. _アプリ提出の詳細_ エリアで、アドオンに関する有益な詳細を追加してください。 詳細には、アプリ名、説明、連絡先のメールが含まれます。

1. すべてのフィールドを完了したら、**[!UICONTROL 送信]**&#x200B;をクリックします。

1. Developer Consoleへのログインに使用したのと同じAdobe IDを使用して、[Adobe Exchange](https://exchange.adobe.com/)にログインします。 この組織にシステム管理者権限がない場合は、組織システム管理者に承認を依頼してください。

1. **[!UICONTROL Manage]** > **[!UICONTROL App Builder applications]**&#x200B;を選択して、アプリをレビューするリクエストにアクセスします。

1. アプリを確認したら、「**[!UICONTROL 承認]**」を選択します。 また、情報メモを追加することもできます。

これで、アドオンが組織のGenStudio for Performance Marketing インスタンスに表示されます。
