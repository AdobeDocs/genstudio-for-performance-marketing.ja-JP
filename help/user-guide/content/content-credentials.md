---
title: Content Credentials法人版
description: GenStudio for Performance MarketingでContent Credentialsを適用してレビューする方法について説明します。
level: Intermediate
feature: Content Management, Content Attributes
exl-id: 9fc1e428-7fa7-4f00-84ba-51c9318766f4
TQID: https://experienceleague.adobe.com/ATpH1AXBAhr5tJDVkgx0ZaK20YYBmP7NQF0BUCtGiGw
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: ad3738c7-91ac-48ed-a914-fd0b03f89396id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f321b88b-6bb7-49cc-a16a-ae2b665ebd32
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 5fe8dccdcf24d26706b7d3621acc1715fd9eb164
workflow-type: tm+mt
source-wordcount: 750
ht-degree: 5%

---

# Content Credentials法人版

ブランドの信頼性を証明し、コンプライアンスを促進するコンテンツの改ざん防止のための資格情報が、マーケティングワークフローに直接組み込まれる方法をご確認ください。

## Content Credentials の基本を学ぶ {#content-credentials}

>[!CONTEXTUALHELP]
>id="gspm_content_credentials"
>title="[!DNL GenStudio for Performance Marketing] の Content Credentials"
>abstract="ブランドの信頼性を証明し、コンプライアンスを推進するコンテンツの改ざん防止資格情報を、マーケティングワークフローに直接埋め込むことができます。"

GenStudio for Performance Marketingは、Content Credentialsをあらゆるアセットに自動的にグローバルに適用します。 有効にする設定手順やアセットごとの設定はありません。マーケティングワークフロー全体を通じて、資格情報が埋め込まれ、保存され、更新されます。

コンテンツが公開されると、LinkedInなどの外部プラットフォームにContent Credentialsが表示されます。

C2PAに準拠したContent Credentialsでは、証明書を設定する必要はありません。 ブランドの署名は例外です。組織独自の署名でコンテンツに署名するには、管理者がAdmin Console内に有効なX.509証明書をアップロードする必要があります。 この手順により、企業のデジタル署名が適切に設定され、サポートされているAdobe DX アプリケーションで使用できる状態になります。

## Content Credentialsとは？ 

Content Credentialsは、業界標準の耐久性のあるメタデータであり、コンテンツの制作方法やクリエイターのID情報が記載されています。 Content Credentialsは、コンテンツがサポートするプラットフォームにオンラインで公開されている場合、または[Adobeの検査ツール ](https://contentauthenticity.adobe.com/inspect)や[Adobe Content Authenticity Chrome ブラウザー拡張機能](https://helpx.adobe.com/creative-cloud/help/cai/adobe-content-authenticity-chrome-browser-extension.html)などのツールを使用して表示できます。  

Content Credentialsを導入すれば、コンテンツの制作方法の透明性を高め、オーディエンスがコンテンツを活用できるようになります。

[AdobeでContent Credentials](https://helpx.adobe.com/jp/creative-cloud/help/content-credentials.html)の詳細を確認します。

## ブランド署名とアセット追跡

ブランド署名コンテンツは、ブランドの整合性とユーザーの信頼を促進する上で重要な役割を果たします。 組織は、Admin Consoleで証明書が適切に設定されている場合、Adobe アプリケーションで一意のブランド署名を使用してコンテンツに署名できます。 この信頼性の保証は、目に見えない透かしとフィンガープリント技術を使用して維持され、コンテンツのライフサイクル全体を通じて署名の耐久性を維持するのに役立ちます。

企業は、ブランドへの署名に加えて、アセット IDをコンテンツに直接添付できます。 これにより、特にソーシャルメディアプラットフォームで共有または投稿されたアセットを効率的に追跡できます。 アセット IDを組み込むことで、コンテンツの由来と配信パスを追跡し、管理と説明責任を強化することができます。

## マーケティングワークフローにおけるContent Credentials

Content Credentialsの導入は、インポートやコンテンツの発見からアクティベーション、エクスポートに至るまで、マーケティングワークフロー全体を通じて、GenStudio for Performance Marketingで直接実行できます。 また、アプリ全体でレビュー用にコンテンツに表示される資格情報もあります。

### 読み込みと検出

コンテンツギャラリーでは、読み込んだアセットに認証情報が表示されます。

サムネールの右上隅にあるContent Credential バッジは、[!UICONTROL  ブランド署名済み] コンテンツを示します。

![資格情報を含むインポートされたアセット ](./images/import-discovery1.png)

署名済みコンテンツを選択すると、公開されたブランド、レコーダー、使用されたツール、タイムスタンプなどの詳細なメタデータが表示されます。

コンテンツは、資格情報のステータスでフィルタリングできます。

![ アセットの資格情報データ ](./images/import-discovery2.jpg)

### コンテンツの制作と選択

Content Credentialのバッジは、Canvas Asset セレクターに表示されます。

エクスペリエンスでアセットを選択すると、編集中に来歴チェーンを維持するために資格情報のメタデータが保持されます。

![Canvas アセットセレクターのContent Credential バッジ ](./images/creation-selection1.png)

### 編集と変換

ドラフトからの書き出し中に、変更されたアセットは自動的に再署名され、新しい資格情報は元のアセットにリンクされます。

![書き出し形式オプションを含むダウンロードダイアログ ](./images/edit-and-transformation2.png){width="60%"}

### レビューと承認

レビューと承認プレビューでは、右側のパネルにアセットの資格情報ステータスが表示されます。

![承認済みアセットの資格情報データ ](./images/review-and-approve1.png){width="60%"}

レビュー担当者がアセットを調査すると、バリエーションごとの資格情報の詳細が表示されます。 ユーザーが「**[!UICONTROL コンテンツに保存]**」をクリックすると、承認済みエクスペリエンスが再署名されます。

![承認済みコンテンツの詳細を確認ダイアログ。コンテンツに保存ボタン ](./images/review-and-approve3.png)

### アクティベーションとエクスポート

アクティベーション中、資格情報のステータスがエクスペリエンスセレクターに表示されます。

アクティブ化されたアセットの![資格情報データ ](./images/activate-export1.png){width="60%"}

書き出されたファイルには、C2PA準拠の資格情報が埋め込まれます。

書き出されたアセットも系統を維持します。 埋め込まれた資格情報には、書き出しの派生元のアセットが記録されるため、書き出されたエクスペリエンスは、元の読み込まれたアセットの編集を通じて遡ることができます。 リネージュはファイル内を移動するため、アセットがGenStudio for Performance Marketingを離れた後も検査できます。

資格情報の一貫性は、サポートされているすべてのフォーマット（JPEG、PNG、MP4）で維持されます。

![書き出されたアセットの資格情報データ ](./images/activate-export2.png)

## 関連情報

* [コンテンツの透明性](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/overview/content-transparency)
* Adobeの[Content Credentials](https://helpx.adobe.com/jp/creative-cloud/help/content-credentials.html)
