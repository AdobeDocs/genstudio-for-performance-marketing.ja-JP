---
title: Workfront Proofとレビューおよび承認の統合
description: Workfront ProofとAdobe GenStudio for Performance Marketingの統合。
feature: Content Review, Content Management
exl-id: 149db773-4787-4cfb-b29e-c49f13abf39a
source-git-commit: 47195c08f500e50a01db127c6badc461c10afaf9
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Workfront ProofとGenStudio for Performance Marketingの統合

とWorkfront Proofの統合は、承認テンプレート、複数ステージのワークフロー、プルーフのバージョンを比較 [ する機能などの高度な機能により、GenStudio for Performance Marketingのレビューと承認のライフサイクルを強化 ](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs) ます。 構造化されたバージョン管理により、コンテンツのレビューのライフサイクル全体を通じて、透明性、説明責任、および合理化された共同作業が確保されます。

>[!BEGINSHADEBOX]

**前提条件**:

[Adobe Workfront Web ビューア拡張機能のインストール ](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/review-proofs-in-workfront/review-a-proof/review-proof-in-web-viewer-extension)

>[!ENDSHADEBOX]

Workfront Proof [!DNL Proofing Viewer] は、プルーフの表示、コメント、比較を行うための機能豊富なワークスペースです。 [!DNL Proofing Viewer] から、次のことができます

* 様々なバージョンのコンテンツの比較
* プルーフにコメントと図面マークアップを追加する
* プルーフを承認

承認依頼メールまたは製品内通知のプルーフ URL をクリックすると、[!DNL Proofing Viewer] が読み込まれます。 [!DNL Proofing Viewer] 新規 _承認_ ビューが開きます。 この表示から、コア [!DNL Proofing Viewer] 注釈ツールを使用して、コンテンツをレビューし、コメントを提供できます。

[!DNL Proofing Viewer] を終了するには、「**[!UICONTROL GenStudioに戻る]** をクリックします。

## Genstudio for Performance Marketing とWorkfront Proof：機能の比較

次の表では、GenStudio for Performance Marketingの標準的なレビューおよび承認機能と、Workfront Proofの統合で利用できるより高度な機能を比較しています。

| 機能        | GenStudio for Performance Marketing                                                                 | Workfront Proof                                                                 |
|-------------------------------|------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| **ドラフト/プルーフのライフサイクル**        | ドラフトコンテンツは公開時に有効期限が切れます。 | タイムスタンプ付きの永続的なログを含む、複数ステージの役割ベースの承認チェーン。<br> すべてのバージョンが無期限に保持されます。 |
| **コメント**                | コメントはドラフト ID に結び付けられ、公開後に破棄されます。                                           | 永続的なコメントと注釈は、監査とコンプライアンスのために保持されます。     |
| **バージョン**           | ドラフトは一意のインスタンスとして扱われます。<br> 横に並べて比較することはできません。                                      | 並列およびオーバーレイ比較ツールによる完全なバージョン管理。        |
| **プロジェクト管理** | 基本的なキャンペーン管理。 | カスタマイズ、テンプレート、レポート、詳細な監査を含む、完全なキャンペーンライフサイクル管理。 |

### ライセンスとユーザーの役割

ライセンスは、製品内の一連のユーザー使用権限を識別します。 Workfront Proofには、GenStudio for Performance Marketingよりも多くのライセンスタイプまたはユーザーの役割が用意されています。 [ プルーフの役割の概要 ](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles) では、Workfront Proofのレビューと承認のワークフローに関連付けられたユーザーの役割について説明します。

| GenStudio for Performance Marketing ライセンス       | Workfront ライセンス                 | 説明                                                                                                                                                      |
|---------------------------------------------------|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| GenStudio System Manager                          | Workfront管理者/パワーユーザー | ブランド、ペルソナ、商品管理など、GenStudioのパフォーマンスマーケティング機能へのフルアクセス。 ワークフローと設定を管理します。 承認テンプレートを作成します。 |
| コンテンツの作成者と編集者（パワーユーザーライセンス）   | プルーフの作成者（標準ライセンス）  | コンテンツドラフトを生成して送信します。 プルーフビューアでは、がアセットをアップロードし、プルーフを開始します。 Workfront Proof ライセンスが必要です。                              |
| レビュアー/承認者（Collaborator ライセンス）        | レビュアー/承認者                 | 複数ステージのレビューに参加し、コメントを追加し、コンテンツを承認または却下します。                                                                             |

Adobe システム管理者は、Adobe Admin Consoleで両方の製品のユーザープロビジョニングと使用権限を管理します。

>[!NOTE]
>
> Workfront Proofには [ 追加のユーザーの役割 ](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles) が用意されています。 パフォーマンスマーケティング内にすべての役割が表示されるわけではありません。 ただし、Workfront Proofテンプレート内に設定されたすべてのロールが適用されます。

### ドラフトと配達確認

Workfront [!DNL Proofing Viewer] は、GenStudio for Performance Marketingの基本的な確認および承認プロセスを、より構造化された確認および承認機能で拡張します。 この統合で確認されるプルーフは、GenStudio for Performance Marketingでサポートされる形式に制限されます。

### バージョン管理

GenStudio for Performance Marketingは承認テンプレートをサポートしていませんが、Workfront Proofはサポートしています。 プルーフのバージョン管理機能により、GenStudioのコンテンツのレビューと承認のプロセスが大幅に強化されます。 プルーフワークフロー内の各送信は、コンテンツのドラフトまたは _プルーフ_ の個別のバージョンとして扱われます。 配達確認は自動的に保存され、以前のイテレーションと並べて比較できます。 関係者は、変更を追跡し、正確なフィードバックを提供し、レビューサイクルを通じて調整を維持できます。 Proof は、監査の準備とコンプライアンスの要件をサポートするために、すべてのコメント、決定、バージョンの完全な履歴を保持します。 また、各バージョンは、承認、却下、コメントなどのすべてのアクションが明確にログに記録され、タイムスタンプが付けられた、複数ステージの役割ベースの承認ワークフローもサポートします。

### 承認テンプレート

Workfront Proof承認テンプレートには、プルーフ承認ワークフローを効率化できる形式設定済みの手順が用意されています。 これらのテンプレートには、選択したレビュー担当者と承認者、プルーフの役割、期限が含まれるので、一貫性と効率が確保されます。 レビューを開始するコンテンツ作成者は、単相承認ワークフローと多相承認ワークフローの両方について、事前定義済みのテンプレートのセットから選択できます。

ワークフローテンプレートの各ステージは、割り当てられたレビュー担当者を識別します。 Workfront Proof ワークフローからのすべてのステータス更新とコメントはプルーフビューアに表示されるため、透明性と共同作業が向上します。

承認テンプレートは複数のステージの承認をサポートしており、様々な関係者グループからのレビューの調整をサポートします。

### コメント

レビュー担当者は、プルーフの特定の領域を直接クリックして、コンテキストに沿った正確なコメントを残すことができます。 すべてのコメントにはタイムスタンプが付き、プルーフのバージョン履歴の一部として保存されます。 コメント履歴は、GenStudio for Performance Marketingでは使用できません。

[2 つのバージョンのプルーフを比較 ](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs) して、レビューのコメントとコンテンツを評価できます。

## 通知とリマインダー

レビュー担当者と承認者は、新しいプルーフがレビュー可能になった場合、または進行中のレビューのステータスが変更された場合に、メール通知を受け取ります。
[ プルーフ通知とリマインダー ](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/proof-notifications-and-reminders/proof-notifications-and-reminders/proof-notifications-and-reminders) には、プルーフへのパーソナライズされたリンク、プルーフの詳細と承認プロセスを通じたその進行状況、バージョン情報が含まれます。
