---
title: Journey Optimizer for GenStudio
description: GenStudio Adobe Exchange用Journey Optimizer アプリをインストールして設定し、GenStudio for Performance MarketingでAdobe Journey Optimizer テンプレートを使用できるようにします。
feature: Extensibility
source-git-commit: e5011c95e9536d73b1f09d6bc76bb83f121573cd
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# Journey Optimizer for GenStudio

同じ[!DNL IMS]組織で[!DNL Adobe Journey Optimizer] （AJO）と[!DNL GenStudio for Performance Marketing]を使用する組織は、[!DNL Adobe Exchange]から&#x200B;**Journey Optimizer for GenStudio** アプリをインストールできます。 システム管理者がアプリを承認してデプロイメントを完了すると、作成者は、GenStudioで電子メールエクスペリエンスを作成する際に、[!DNL Content]に直接アップロードされたテンプレートの横にAJO コンテンツテンプレートを選択できます。

このトピックは、アプリをインストールし、[!DNL Adobe Developer Console]でOAuth資格情報を作成し、[!DNL Adobe Experience Platform]でテクニカルアカウントの権限をマッピングする&#x200B;**管理者と開発者**&#x200B;向けです。 AJOとMarketo テンプレートの構文がGenStudioでどのように機能するかについては、[AJOとMarketoのテンプレート &#x200B;](/help/user-guide/templates/use-templates.md#templates-from-ajo-and-marketo)を参照してください。

## 前提条件

* AJOは、拡張機能をデプロイする組織でプロビジョニングする必要があります。
* AJOでテンプレートを作成するユーザーは、組織の定義に従って、Journey Optimizerで&#x200B;**コンテンツテンプレートを作成および編集**&#x200B;する権限が必要です。
* AJOのメールテンプレートには、生成されたコンテンツを表示するフィールドプレースホルダー（ハンドルバー）を含める必要があります。 これらのフィールドを使用せずにテンプレートを選択できますが、[!DNL GenStudio for Performance Marketing]が想定するプレースホルダーが見つからない場合、**エクスペリエンスの生成が失敗します**。 [&#x200B; テンプレートのカスタマイズ &#x200B;](/help/user-guide/templates/customize-template.md)および[認識済みフィールド名](/help/user-guide/templates/customize-template.md#recognized-field-names)を参照してください。

## Adobe Exchangeからアプリをインストールする

>[!VIDEO](https://video.tv.adobe.com/v/3483300?captions=jpn&learn=on)

1. [Adobe Exchange](https://exchange.adobe.com)を開き、**[!UICONTROL CX Enterprise]**&#x200B;に移動します。
1. GenStudio[&#128279;](https://exchange.adobe.com/apps/ec/abpopqqr1q/journey-optimizer-for-genstudio)のJourney Optimizer リストを開きます。
   要件と無料インストール ![&#128279;](/help/extensibility/ajo-adobe-exchange.png){width="75%"}を含むAdobe Exchange上のGenStudio用Journey Optimizerの一覧
1. **[!UICONTROL 無料]**&#x200B;を選択して、組織のアプリをリクエストします。
1. 組織&#x200B;**がリクエストをレビューして承認**&#x200B;したら、[Adobe Developer ConsoleでOAuth資格情報を作成](#create-oauth-credentials-in-adobe-developer-console)し、[Exchange](#deploy-the-application-from-exchange)からアプリケーションをデプロイします。

## Adobe Developer ConsoleでのOAuth資格情報の作成

Journey Optimizer APIのOAuth資格情報を提供する[Adobe Developer Console](https://developer.adobe.com/console/)に&#x200B;**プロジェクト**&#x200B;を作成します。 Exchangeでアプリを設定する際には、**クライアント ID**、**クライアント シークレット**、**組織ID**、**スコープ**&#x200B;などの値が必要です。

1. Adobe Developer Consoleにログインし、**新しいプロジェクト**&#x200B;を作成します。
1. **[!UICONTROL Add API]**&#x200B;をクリックし、**[!DNL CX Enterprise]**&#x200B;製品API リストから&#x200B;**[!UICONTROL Adobe Journey Optimizer]**&#x200B;を選択して、**Adobe Journey Optimizer （AJO） API**&#x200B;をプロジェクトに追加します。
1. プロジェクト ワークスペースで資格情報を生成し、**クライアント ID**、**クライアント シークレット**、**組織ID**、**スコープ**&#x200B;およびその他のデプロイメントフローが要求する値をコピーします。 次のセクションのために安全に保存しましょう。

>[!NOTE]
>
>Exchangeからインストールする場合、OAuth クライアント IDとテクニカルアカウント IDの両方が表示されている場合は、**OAuth クライアント ID**&#x200B;を使用します。

## Exchangeからのアプリケーションのデプロイ

### 管理でアプリを開き、環境を追加します

1. [Adobe Exchange](https://exchange.adobe.com)に戻ります。
1. **[!UICONTROL 管理]**&#x200B;を選択し、**[!UICONTROL App Builder アプリケーション]**&#x200B;を開きます（または組織の管理対象アプリケーションへのパス）。
1. GenStudio **の** Journey Optimizerを選択し、アプリが&#x200B;**Approved**&#x200B;であることを確認します。
1. **[!UICONTROL 環境]**&#x200B;で、**環境：** ドロップダウンから既存の環境を選択するか、**[!UICONTROL 環境を追加]**&#x200B;を選択して環境を作成します。
   ![承認済みステータスと環境の追加を含むアプリケーションの詳細](/help/extensibility/ajo-config-002.png){width="50%"}
1. 選択した環境で、**[!UICONTROL 設定]**&#x200B;を選択します。
1. 「**[!UICONTROL Configuration]**」タブで、**[!UICONTROL AJO資格情報]**&#x200B;を検索します。
   ![&#x200B; デプロイ前のAJO資格情報による設定（ドラフト） &#x200B;](/help/extensibility/ajo-config-004.png){width="80%"}
1. Journey Optimizer APIが追加されたDeveloper Console プロジェクトの資格情報（例：**[!UICONTROL AJO クライアント ID]**、**[!UICONTROL AJO クライアントシークレット]**、**[!UICONTROL AJO トークン エンドポイント]**&#x200B;およびその他の必須フィールド）を入力します。
1. すべての小文字&#x200B;**に** サンドボックス名を入力します（例：`prod`）。
1. 「**[!UICONTROL デプロイ]**」をクリックします。デプロイメントが完了すると、ステータスは「デプロイ済み」と表示されます。ボタンのテキストが&#x200B;**[!UICONTROL デプロイ解除]**&#x200B;に変更されます。
   ![&#x200B; デプロイ済みアプリとアンデプロイ済みアプリは、App Builderのアプリケーションビュー](/help/extensibility/ajo-config-005.png){width="80%"}で利用できます

デプロイメント後、Adobe Developer Consoleには、AJOおよびAdobe Runtime APIを使用したGenStudio &lt;Your_Environment_Name>**用の**&#x200B;Journey Optimizerという名前の新しい自動生成プロジェクトが含まれます。このプロジェクトは読み取り専用で、編集または削除できません。
![&#x200B; デプロイメント後に読み取り専用の自動生成されたDeveloper Console プロジェクト &#x200B;](/help/extensibility/ajo-auto-project.png){width="100%"}

### 設定を更新

環境の設定変数を変更するには、まず&#x200B;**[!UICONTROL 展開を解除]**&#x200B;し、値を更新してから&#x200B;**[!UICONTROL 展開]**&#x200B;をもう一度します。これにより、変更が有効になります。

Exchangeで&#x200B;**複数の環境**&#x200B;を作成できます（例えば、サンドボックスごとに1つ）。 複数のサンドボックスを使用している場合、デプロイメントごとにGenStudioの個別のエクスペリエンスとして表示できます。

## テクニカルアカウントの権限のマッピング

GenStudioでAJO拡張機能を表示できます。完全な[!DNL Adobe Experience Platform] アクセス権はありません。 API呼び出し（テンプレートの読み込みなど）の場合、OAuth資格情報に関連付けられたテクニカルアカウントには、**[!DNL Adobe Experience Platform]** > **[!UICONTROL 権限]**&#x200B;でJourney Optimizer権限を付与する必要があります。 役割の正確な名前と権限セットは、組織によって異なります。

AJO **[!UICONTROL 権限]** > **[!UICONTROL ロール]**&#x200B;の&#x200B;**[!UICONTROL ジャーニー管理者]**&#x200B;の下にある拡張機能を表示し、Developer Console プロジェクトから&#x200B;**API資格情報**&#x200B;を追加します。これは、Exchangeからのデプロイ時に使用したのと同じ資格情報です。

![Adobe Experience Platform権限でAJO Architect ロールに割り当てられたAPI資格情報](/help/extensibility/ajo-map-permissions.png){width="80%"}

**関連項目** （Journey Optimizer アクセス制御）:

* [アクセス制御](https://experienceleague.adobe.com/ja/docs/journey-optimizer/using/access-control/access-control-landing-page)
* [Journey Optimizerでの権限](https://experienceleague.adobe.com/ja/docs/journey-optimizer/using/access-control/permissions)
* [システム管理者向けの基本を学ぶ](https://experienceleague.adobe.com/ja/docs/journey-optimizer/using/get-started/quick-start/administrator)

## GenStudioでのAJO テンプレートへのアクセス

デプロイメントと権限のマッピング後：
1. GenStudio for Performance Marketingで&#x200B;**[!UICONTROL Create]**&#x200B;を開き、**電子メール**&#x200B;のエクスペリエンスを開始します。
1. **[!UICONTROL テンプレートを選択]**&#x200B;で、**[!UICONTROL アップロードしたテンプレート]**&#x200B;の横にある&#x200B;**[!UICONTROL AJO テンプレート]** タブを開き、Journey Optimizerからテンプレートを参照します。

![AJO テンプレート タブとテンプレートギャラリーを使用してテンプレートを選択](/help/extensibility/ajo-template-tab.png){width="80%"}

## トラブルシューティング

### 「AJO テンプレート」タブが表示されない

* Exchange **[!UICONTROL 設定]**&#x200B;で入力された値が正しいことを確認します。これには、**クライアント ID**、**クライアントシークレット**、**スコープ**、**サンドボックス**&#x200B;が含まれます。
* **サンドボックス名が小文字**&#x200B;であることを確認します（例：`prod`）。
* Exchangeからインストールする場合は、[OAuth資格情報の作成](#create-oauth-credentials-in-adobe-developer-console)の説明に従って、**クライアント ID**&#x200B;を使用してください。

### 「AJO テンプレート」タブは表示されますが、テンプレートは表示されません

* ページを再読み込みするか、「**[!UICONTROL AJO テンプレート]**」タブを再度開きます。
* ブラウザー&#x200B;**[!UICONTROL ネットワーク]** ツールで、**`get-templates`** リクエストを調べます。 **403 Forbidden**&#x200B;が返された場合、テクニカルアカウントは、必要なJourney Optimizer権限を持つロールまたはグループに割り当てられていません。 [!DNL Adobe Experience Platform] **[!UICONTROL 権限]**&#x200B;およびAJO **[!UICONTROL 権限]**&#x200B;のマッピングを、組織が必要に応じて更新します。
