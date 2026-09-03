---
title: ' [!DNL AEM Assets Content Hub]  リポジトリに接続'
description: Adobe GenStudio for Performance MarketingをAdobe Experience Manager （AEM）  [!DNL Content Hub]  リポジトリに接続し、既存の承認済みコンテンツを活用する方法について説明します。
level: Experienced
role: Admin, Developer
feature: Content Management
recommendations: noDisplay
exl-id: abb587fd-593c-4b9f-baad-993d92400d9b
TQID: https://experienceleague.adobe.com/FJ6G7qlBlkrsGk1H7SHhlkqHUHYYGKkTqklTeGDxJho
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 387
ht-degree: 3%

---

# [!DNL AEM Assets Content Hub] リポジトリへの接続

Adobe Experience Manager（AEM）にアセットがある場合は、次の手順に従って、GenStudio for Performance Marketingでアセットにアクセスできるようにします。

>[!BEGINSHADEBOX]

**前提条件**:

次の手順では、Admin ConsoleおよびAEM Assets as a Cloud Serviceへの管理アクセスが必要です。

>[!ENDSHADEBOX]

## 手順1: [!DNL AEM Assets Content Hub]を有効にする

**Content Hubのデプロイ** セルフサービスプロセスに従って、Cloud Managerの既存のAEM Assetsで[!DNL Content Hub]を有効にします。 _AEM as a Cloud Service_ ドキュメントの[&#x200B; デプロイ  [!DNL Content Hub]](https://experienceleague.adobe.com/ja/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub)を参照してください。

[!DNL AEM Assets Content Hub]を有効にすると、Admin Consoleで[!DNL AEM Assets as a Cloud Service]内に`contenthub`接尾辞を持つ新しいインスタンスが作成されます。

>[!IMPORTANT]
>
>管理者は、[!DNL AEM Assets Content Hub] リポジトリがGenStudio for Performance Marketingと同じ組織内にあることを確認する必要があります。

## 手順2:GenStudio ユーザーのオンボーディング

[!DNL Admin Console]で、GenStudio for Performance Marketing ユーザーまたはユーザーグループを[!DNL AEM Assets Content Hub]製品プロファイルに追加します。 コンテンツレビュアーが[!DNL AEM Assets Content Hub] リポジトリと同じ組織にアクセスできない場合、コンテンツのレビューと承認が困難になる可能性があります。

- [&#x200B; オンボード  [!DNL Content Hub] 管理者](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-administrator)
- [&#x200B; オンボード  [!DNL Content Hub]  ユーザー](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-users)

## ステップ 3：アセットの承認

[!DNL AEM Assets Content Hub]で使用するアセットを承認すると、GenStudio for Performance Marketingで使用できるようになります。

_AEM as a Cloud Service_ ドキュメントの「[Experience Manager](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/approve-assets) アセットの承認」を参照してください。

## 手順4：アセットの表示の設定

_[!DNL AEM Assets Content Hub]_&#x200B;設定オプションで、フィルター、アセットの詳細、検索、ブランディングの各設定オプションのセットを確認します。

_Content Hub_ ドキュメントの[AEM as a Cloud Service ユーザーインターフェイスの設定](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/configure-content-hub-ui-options)を参照してください。

## 手順5：接続の確認

GenStudio for Performance Marketing コンテンツでは、右側のギャラリーの上に「_[!UICONTROL 場所]_」リストが表示されます。 アクセス権がない場合、または組織が[!DNL AEM Assets Content Hub] リポジトリをデプロイして接続していない場合、リストは使用できません。

場所リストとリポジトリの変更については、[Assetsの場所](manage-assets.md#assets-location)を参照してください。
