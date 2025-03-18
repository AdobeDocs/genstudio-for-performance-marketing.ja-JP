---
title: アプリの配布
description: GenStudio for Performance Marketing用のアプリまたはアドオンを配布します。
exl-id: 4935356b-08df-402c-b1a2-b89627afc188
source-git-commit: 8884f3438a0010119f578ca9a3b7158e2e01cfa3
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# アプリの配布

アドオンを配布すると、組織やその他の組織で使用できるようになります。

プライベート配布では、アドオンのデプロイメントを、アドオンを開発した IMS 組織で識別される組織に制限します。 公開配布を行うと、アドオンはAdobe Exchange上でアプリとして使用できるようになります。 配布ワークフローは、使用するアドオンがパブリックとプライベートのどちらの配布を対象としているかによって異なります。

このトピックでは、プライベート配布について説明します。 [2}App Builder](https://developer.adobe.com/app-builder/docs/guides/distribution/public/) 開発者向けドキュメントの { 公開配布 _では、任意のAdobe組織でアプリを使用できるようにする方法が説明されています。_

>[!BEGINSHADEBOX]

**前提条件**:

次の権限があることを確認します。

* 承認用にアプリを送信する組織の開発者権限

* アプリを承認するためのシステム管理者権限

App Builder アプリは、App Builder プロジェクトにデプロイする必要があります。

>[!ENDSHADEBOX]

**アプリを非公開で配布するには**:

プライベート配布では、組織のメンバーのみがアプリを使用できます。

1. [Adobe Developer Console](https://developer.adobe.com/console/) から、アプリがデプロイされている組織、プロジェクト、ワークスペースを選択します。

1. **[!UICONTROL 2}Workspaceの概要]** エリアから「_承認」を選択します。__アプリの承認_ ペインが開きます。

1. _アプリ送信の詳細_ 領域に、アドオンに関する情報の詳細を追加します。 詳細には、アプリ名、説明、連絡先のメールが含まれます。

1. すべてのフィールドへの入力が完了したら、「**[!UICONTROL 送信]**」をクリックします。

1. Developer Consoleへのログインに使用したのと同じAdobe IDを使用して ](https://exchange.adobe.com/)Adobe Exchange} にログインします。 [この組織のシステム管理者権限を持っていない場合は、組織システム管理者に承認を依頼してください。

1. **[!UICONTROL 管理]**/**[!UICONTROL App Builder アプリケーション]** を選択して、アプリをレビューするリクエストにアクセスします。

1. アプリを確認したら、「**[!UICONTROL 承認]**」を選択します。 必要に応じて、情報メモを追加します。

これで、アドオンが組織のGenStudio for Performance Marketing インスタンスに表示されるようになりました。
