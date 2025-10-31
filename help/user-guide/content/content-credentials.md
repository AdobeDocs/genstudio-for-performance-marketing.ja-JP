---
title: 組織のContent Credentials
description: GenStudio for Performance MarketingでContent Credentialsを申請およびレビューする方法について説明します。
level: Intermediate
feature: Content Management, Content Attributes
source-git-commit: 488bc7d7b7447ee6e807dd91f83766844c24abb9
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 0%

---

# 組織のContent Credentials

ブランドの信頼性を証明しコンプライアンスを促進する、コンテンツの改ざん防止資格情報がマーケティングワークフローに直接組み込まれる仕組みを説明します。

>[!WARNING]
>
> この機能は現在ベータ版で、アクセス権が付与された組織のみが使用できます。 ご興味がある場合は、Adobe アカウントチームの担当者にお問い合わせいただくか、[ このリンクを使用して登録をリクエスト ](https://www.feedbackprogram.adobe.com/c/a/5aWPEOthrDv22Mf9CyekOy?source=qr) してください。


## Content Credentialsの概要

Content CredentialsがAdmin Consoleでアクティブ化されると、GenStudio for Performance Marketing ユーザーは、アプリ内のすべてのアセットに対してContent Credentialsをグローバルにオンにできます。 資格情報を適用するグローバルオプションがオフになっている場合は、個々のアセットにContent Credentialsを適用するかどうかを選択できます。

コンテンツが公開されると、Content Credentialsは、LinkedIn などの外部プラットフォームに表示されるようになります。

管理者は、Admin Console内に有効な X.509 証明書をアップロードする必要があります。 この手順により、企業のデジタル署名が適切に設定され、サポートされているAdobe DX アプリケーションで使用できるようになります。

>[!NOTE]
>
>この設定を制御することにより、今後はAdmin Consoleに移行して、アプリケーション間のContent Credentials管理を合理化し、管理監督機能を強化する可能性があります。

## Content Credentialsとは 

Content Credentialsは、コンテンツの作成方法の詳細と作成者の ID 情報を含む、耐久性のある業界標準のメタデータです。 Content Credentialsは、コンテンツがサポートプラットフォームにオンラインで公開されたとき、または [Adobeの検査ツール ](https://contentauthenticity.adobe.com/inspect)[Adobe Content Authenticity Chrome ブラウザー拡張機能 ](https://helpx.adobe.com/creative-cloud/help/cai/adobe-content-authenticity-chrome-browser-extension.html) などのツールを使用して表示できます。  

Content Credentialsを適用すると、コンテンツの作成方法の透明性を高め、ユーザーがコンテンツに慣れるのに役立ちます。

[Content Credentialsの詳細については ](https://helpx.adobe.com/jp/creative-cloud/help/content-credentials.html)Adobeを参照してください。

## ブランド署名とアセットトラッキング

ブランド署名コンテンツは、ブランドの整合性とユーザーの信頼を高める上で重要な役割を果たします。 Admin Consoleで証明書が適切に設定されている場合は、Adobe アプリケーションで一意のブランド署名を使用してコンテンツに署名できます。 この信頼性の保証は、目に見えない透かしやフィンガープリントのテクノロジーを使用して維持され、コンテンツのライフサイクルを通じて署名の耐久性を維持するのに役立ちます。

企業は、ブランド署名に加えて、アセット ID をコンテンツに直接添付できます。 これにより、特にソーシャルメディアプラットフォームで共有または投稿されるアセットを効率的に追跡できます。 アセット ID を組み込むことで、組織はコンテンツの起源と流通パスを追跡し、監視とアカウンタビリティを強化できます。

## マーケティングワークフローでのContent Credentials

Content Credentialsの適用は、読み込みとコンテンツ検出から、アクティベーションと書き出しまで、GenStudio for Performance Marketingでのマーケティングワークフロー全体を通じて直接行うことができます。 また、アプリ全体でレビューするために、コンテンツに資格情報が表示されます。

### 読み込みと検出

コンテンツギャラリーでは、読み込まれたアセットに資格情報が表示されます。

サムネールの右上隅にあるContent Credential バッジは、「ブランドが署名した」コンテンツを示します。

![ 読み込まれたアセット（資格情報を含む） ](./images/import-discovery1.png)

署名済みコンテンツを選択すると、公開されたブランド、レコーダー、使用されたツール、タイムスタンプなどの詳細なメタデータが表示されます。

コンテンツは、資格情報のステータスでフィルタリングできます。

![ アセットの資格情報データ ](./images/import-discovery2.jpg)

### 作成と選択

Content Credentialバッジは、キャンバスアセットセレクターに表示されます。

認証情報のメタデータは、編集全体を通じてプロベンションチェーンを維持するためにエクスペリエンスのアセットが選択されるたびに保持されます。

![ キャンバスアセットセレクターのContent Credential バッジ ](./images/creation-selection1.png)

### 編集と変換

ドラフトからの書き出し時に、変更されたアセットは自動的に再署名され、新しい資格情報が元の資格情報にリンクされます。

![ 書き出されたアセットの資格情報データ ](./images/edit-and-transformation1.png){width="60%"}

### レビューと承認

レビューと承認のプレビューでは、右側のパネルにアセットの資格情報ステータスが表示されます。

![ 承認済みアセットの資格情報データ ](./images/review-and-approve1.png){width="60%"}

レビュー担当者がアセットを検査すると、バリアントごとの資格情報の詳細が表示されます。 ユーザーが「**[!UICONTROL コンテンツに保存]** をクリックすると、承認済みのエクスペリエンスが再署名されます。

![ 承認済みアセットの資格情報データ ](./images/review-and-approve2.png)

### アクティベーションとエクスポート

アクティベーション時に、エクスペリエンスセレクターに資格情報ステータスが表示される。

![ アクティブ化されたアセットの資格情報データ ](./images/activate-export1.png){width="60%"}

書き出されたファイルには、C2PA 準拠の資格情報が埋め込まれます。

サポートされるすべての形式（JPEG、PNG、MP4）で資格情報の整合性が維持されます。

![ 書き出されたアセットの資格情報データ ](./images/activate-export2.png)

