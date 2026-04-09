---
title: Marketo for GenStudio
description: GenStudio Adobe Exchange用Marketo アプリをインストールして設定し、GenStudio for Performance MarketingでMarketo Engage テンプレートを使用できるようにします。
feature: Extensibility
source-git-commit: 4118624b479905cd2f2193d542c000678daaf4b8
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# Marketo for GenStudio

同じ[!DNL IMS]組織で[!DNL Marketo Engage]と[!DNL GenStudio for Performance Marketing]を使用する組織は、[!DNL Adobe Exchange]から&#x200B;**Marketo for GenStudio** アプリをインストールできます。 システム管理者がアプリを承認してデプロイメントを完了すると、作成者は、GenStudioで電子メールエクスペリエンスを作成する際に、[!DNL Content]に直接アップロードされたテンプレートの横にMarketo テンプレートを選択できます。

このトピックは、アプリをインストールし、Marketoから資格情報を収集し、アプリをExchangeにデプロイする&#x200B;**管理者**&#x200B;を対象としています。 AJOとMarketo テンプレートの構文がGenStudioでどのように機能するかについては、[AJOとMarketoのテンプレート &#x200B;](/help/user-guide/templates/use-templates.md#templates-from-ajo-and-marketo)を参照してください。

## 前提条件

* [!DNL Marketo Engage]は、拡張機能をデプロイする組織でプロビジョニングする必要があります。
* アプリケーションをデプロイするユーザーには&#x200B;**Marketo資格情報**&#x200B;が必要です。 これらの資格情報を作成および取得するには、**Marketo Product Admin**&#x200B;のアクセス権が必要です（**[!UICONTROL Admin]**&#x200B;領域は、Marketoを開くときに使用できる必要があります）。

## Adobe Exchangeからアプリをインストールする

>[!VIDEO](https://video.tv.adobe.com/v/3483299?learn=on)

1. [Adobe Exchange](https://exchange.adobe.com)を開き、**[!UICONTROL Experience Cloud]**&#x200B;に移動します。
1. GenStudio[&#128279;](https://exchange.adobe.com/apps/ec/ab6p21vo8r/marketo-for-genstudio)のMarketo リストを開きます。
   ![Adobe ExchangeのGenStudio用Marketoのリスト &#x200B;](/help/extensibility/marketo-adobe-exchange.png){width="75%"}
1. **[!UICONTROL 無料]**&#x200B;を選択して、組織のアプリをリクエストします。
1. 組織&#x200B;**がリクエストをレビューして承認**&#x200B;したら、[Marketo資格情報を取得](#get-marketo-credentials)および[Exchange](#deploy-the-application-from-exchange)からアプリケーションをデプロイします。

## Marketo資格情報の取得

**Marketo** インスタンスの資格情報を使用します（Adobe Developer Consoleではありません）。 Exchangeにデプロイする前に、次の情報を収集してください。

### APIのみのユーザーを作成します（既存のAPI ユーザーを再利用する場合はオプション）

1. Marketoで、**[!UICONTROL Admin]**&#x200B;に移動します。
1. **[!UICONTROL セキュリティ]**&#x200B;で、**[!UICONTROL ユーザーと役割]**&#x200B;を開きます。
1. 新しいAPI ユーザーの場合は、**[!UICONTROL APIのみのユーザーを作成]**&#x200B;をクリックします（API ユーザーごとに一意の電子メールを使用）。 **[!UICONTROL API ロール（すべてのワークスペース）]**&#x200B;の役割（または組織が必要とする役割）を割り当てます。 使用するAPI ユーザーが既にある場合は、[LaunchPoint サービスの作成または選択](#create-or-select-a-launchpoint-service)にスキップします。

![&#x200B; ユーザーと役割（APIのみ） ユーザーとAPI役割](/help/extensibility/marketo-users-roles-api-user.png){width="80%"}

### LaunchPoint サービスの作成または選択

1. **[!UICONTROL 管理者]**&#x200B;の&#x200B;**[!UICONTROL 統合]**&#x200B;で、**[!UICONTROL LaunchPoint]**&#x200B;を開きます。
1. **[!UICONTROL 作成]**&#x200B;をクリックして、新しいサービスを作成します（または既存のカスタムサービスを使用します）。
   ![LaunchPoint カスタムサービス &#x200B;](/help/extensibility/marketo-launchpoint-custom-service.png){width="80%"}
1. サービスの場合、**[!UICONTROL 詳細を表示]**&#x200B;をクリックし、**[!UICONTROL クライアント ID]**&#x200B;と&#x200B;**[!UICONTROL クライアントシークレット]**&#x200B;をコピーします。 これらはAdobe Exchange **[!UICONTROL Configuration]**&#x200B;で入力します。

### Marketo REST APIのベース URLをメモします

1. **[!UICONTROL 管理者]**&#x200B;の&#x200B;**[!UICONTROL 統合]**&#x200B;で、**[!UICONTROL Web サービス]**&#x200B;を開きます。
1. **[!UICONTROL REST API]** エンドポイントを見つけます。 フォーム `https://###-XXX-###.mktorest.com`の&#x200B;**ベース URL** （ホスト）のみをコピーします。 **not**&#x200B;には、`/rest`や`/identity`などのパスセグメントを含めないでください。 この値は、Marketo インスタンスごとに一意です。

![Web サービス REST API エンドポイント ベース URL](/help/extensibility/marketo-web-services-rest-endpoint.png){width="80%"}

また、Exchange デプロイメント画面がリクエストする&#x200B;**[!UICONTROL Marketo Engage ID URL]**&#x200B;と、そのREST ベース URL、およびLaunchPointからのクライアント IDとクライアント シークレットも必要です。

## Exchangeからのアプリケーションのデプロイ

拡張機能をGenStudioで使用できるようにするには、Adobe Exchangeからアプリをデプロイします。

1. [Adobe Exchange](https://exchange.adobe.com)に戻ります。
1. **[!UICONTROL 管理]**&#x200B;を選択し、**Marketo for GenStudio** アプリを開きます（例：**[!UICONTROL App Builder アプリケーション]**&#x200B;または組織の管理アプリ）。
1. **[!UICONTROL 環境]**&#x200B;で、ドロップダウンから既存の環境を選択するか、**[!UICONTROL 環境を追加]**&#x200B;を選択して環境を作成します。
1. 選択した環境の&#x200B;**[!UICONTROL 設定]**&#x200B;を開きます。
1. [LaunchPoint](#create-or-select-a-launchpoint-service)の&#x200B;**[!UICONTROL クライアント ID]**&#x200B;と&#x200B;**[!UICONTROL クライアントシークレット]**、Marketo Engage ID URL **、および**&#x200B;[!UICONTROL &#x200B; Marketo Engage REST API ベース URL &#x200B;]&#x200B;**（[Web サービス &#x200B;](#note-your-marketo-rest-api-base-url)のベースホスト）を入力します。**
1. 「**[!UICONTROL デプロイ]**」をクリックします。 デプロイメントが成功すると、アクションは&#x200B;**[!UICONTROL デプロイ解除]**&#x200B;に変わります。

### 設定を更新

環境の設定値を変更するには、まず&#x200B;**[!UICONTROL デプロイ解除]**&#x200B;し、フィールドを更新してから&#x200B;**[!UICONTROL デプロイ]**&#x200B;を再度実行します。

## GenStudioでのMarketo テンプレートへのアクセス

GenStudio用Marketoをインストールして設定した後、GenStudioで&#x200B;**電子メール**&#x200B;のエクスペリエンスを作成すると、**[!UICONTROL Marketo テンプレート]** タブが表示されます。 Marketo Engageからテンプレートを参照するには、このタブを使用します。

>[!IMPORTANT]
>
>GenStudio for Performance Marketingの&#x200B;**標準メール** エクスペリエンスフローでメールを作成します。 この統合では、新しいメールエディターエクスペリエンスで作成されたメールはサポートされていません。

![Marketo資格情報を使用したExchange設定](/help/extensibility/marketo-exchange-configuration.png){width="80%"}

## トラブルシューティング

### 「Marketo テンプレート」タブが表示されない

* アプリがExchangeで&#x200B;**Approved**&#x200B;であり、有効なクライアント ID、クライアントシークレット、Marketo ベース URLを使用して環境が&#x200B;**デプロイ**&#x200B;であることを確認してください。
* 資格情報の作成時に&#x200B;**Marketo Product Admin** アクセスが使用されたことを管理者に確認してもらいます。

### テンプレートが読み込まれない

* ページを再読み込みするか、ログアウトしてGenStudioに再度ログインします。
* ブラウザー開発者ツール **[!UICONTROL Network]** パネルで、Marketo インスタンスへのAPI呼び出しに失敗したことを確認し、Marketoの&#x200B;**[!UICONTROL Web サービス]**&#x200B;に一致するREST ベース URLを確認します（ホストの後に追加パスはありません）。
