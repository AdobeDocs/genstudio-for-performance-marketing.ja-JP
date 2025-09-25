---
title: リポジトリへ  [!DNL AEM Assets Content Hub]  接続
description: Adobe GenStudio for Performance MarketingをAdobe Experience Manager（AEM）  [!DNL Content Hub]  リポジトリに接続し、既存の承認済みコンテンツを活用する方法について説明します。
level: Experienced
role: Admin, Data Engineer
feature: Content Management
recommendations: noDisplay
exl-id: abb587fd-593c-4b9f-baad-993d92400d9b
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# [!DNL AEM Assets Content Hub] リポジトリへの接続

Adobe Experience Manager（AEM）にアセットがある場合は、次の手順に従ってGenStudio for Performance Marketingでアクセスできるようにします。

>[!BEGINSHADEBOX]

**前提条件**:

次の手順では、Admin ConsoleとAEM Assets as a Cloud Serviceへの管理者アクセス権が必要です。

>[!ENDSHADEBOX]

## 手順 1:[!DNL AEM Assets Content Hub] を有効にする

**Content Hubのデプロイ** セルフサービスプロセスに従って、Cloud Managerの既存のAEM Assetsに対して [!DNL Content Hub] を有効にします。 [3&rbrace;AEM as a Cloud Service [!DNL Content Hub]](https://experienceleague.adobe.com/ja/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub) ドキュメントの &lbrace;Deploy _を参照してください。_

[!DNL AEM Assets Content Hub] を有効にすると、Admin Consoleの `contenthub` 内に [!DNL AEM Assets as a Cloud Service] サフィックスの付いた新しいインスタンスが作成されます。

>[!IMPORTANT]
>
>管理者は、[!DNL AEM Assets Content Hub] リポジトリがGenStudio for Performance Marketingと同じ組織内にあることを確認する必要があります。

## 手順 2:GenStudio ユーザーのオンボーディング

[!DNL Admin Console] で、GenStudio for Performance Marketing ユーザーまたはユーザーグループを [!DNL AEM Assets Content Hub] 製品プロファイルに追加します。 コンテンツレビュー担当者が、[!DNL AEM Assets Content Hub] リポジトリと同じ組織へのアクセス権を持っていない場合、コンテンツのレビューと承認が難しくなることがあります。

- [Onboard [!DNL Content Hub] administrator](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-administrator)
- [Onboard [!DNL Content Hub] users](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-users)

## 手順 3：アセットの承認

[!DNL AEM Assets Content Hub] で使用するアセットを承認して、GenStudio for Performance Marketingで使用できるようにします。

[2&rbrace;AEM as a Cloud Service&rbrace; ドキュメントの ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/approve-assets)Experience Managerでのアセットの承認 _を参照してください。_

## 手順 4：アセットの表示の設定

設定オプション _[!DNL AEM Assets Content Hub]_、フィルター、アセットの詳細、検索、ブランディングの設定オプションの各セットを確認します。

[2&rbrace;AEM as a Cloud Service&rbrace; ドキュメントの ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/configure-content-hub-ui-options)Content Hub ユーザーインターフェイスの設定 _を参照してください。_

## 手順 5：接続の確認

GenStudio for Performance Marketing コンテンツでは、右側のギャラリーの上にある _[!UICONTROL 場所]_ リストを使用できます。 アクセス権がない場合や、組織が [!DNL AEM Assets Content Hub] リポジトリをデプロイおよび接続していない場合、リストは使用できません。

場所のリストとリポジトリの変更について詳しくは、[Assetsの場所 ](manage-assets.md#assets-location) を参照してください。
