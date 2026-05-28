---
title: レビューと承認を含むWorkfront Proofとの統合
description: Workfront ProofとAdobe GenStudio for Performance Marketingの連携：
feature: Content Review, Content Management
exl-id: 149db773-4787-4cfb-b29e-c49f13abf39a
TQID: https://experienceleague.adobe.com/G9e9Ft0l9OmSX1lCJY8syzP2-pIswt0MkCpOYlox-Zk
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: ad3738c7-91ac-48ed-a914-fd0b03f89396id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 911
ht-degree: 1%

---

# Workfront ProofとGenStudio for Performance Marketingの統合

Workfront Proofとの統合により、承認テンプレート、多段階のワークフロー、[ プルーフのバージョンを比較](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs)する機能など、高度な機能により、GenStudio for Performance Marketingのレビューと承認のライフサイクルが強化されます。 この構造化されたバージョン管理により、コンテンツレビューのライフサイクル全体を通じて、透明性、説明責任、コラボレーションの合理化を実現できます。

>[!BEGINSHADEBOX]

**前提条件**:

[Adobe Workfront Web Viewer拡張機能](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/review-proofs-in-workfront/review-a-proof/review-proof-in-web-viewer-extension)をインストールします

>[!ENDSHADEBOX]

Workfront Proofの[!DNL Proofing Viewer]は、プルーフを表示、コメント、比較するための豊富なワークスペースです。 [!DNL Proofing Viewer]から、次のことができます

* コンテンツの様々なバージョンの比較
* プルーフにコメントと描画マークアップを追加する
* プルーフを承認

[!DNL Proofing Viewer]は、承認リクエスト電子メールまたは製品内通知でプルーフ URLをクリックすると読み込まれます。 [!DNL Proofing Viewer] _新しい承認_ ビューが開きます。 このビューから、コア [!DNL Proofing Viewer]注釈ツールを使用してコンテンツを確認し、コメントを入力できます。

[!DNL Proofing Viewer]を終了するには、**[!UICONTROL GenStudioに戻る]**&#x200B;をクリックします。

## Genstudio for Performance MarketingとWorkfront Proof：機能の比較

次の表では、GenStudio for Performance Marketingの標準的なレビューと承認の機能と、Workfront Proof統合を通じて利用できる高度な機能を比較しています。

| 機能        | GenStudio for Performance Marketing                                                                 | Workfront Proof                                                                 |
|-------------------------------|------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| **ドラフト/プルーフのライフサイクル**        | ドラフトコンテンツは公開時に期限切れになります。 | タイムスタンプ付きの永続的なログを備えた、多段階の役割ベースの承認チェーン。<br>すべてのバージョンは無期限に保持されます。 |
| **コメント**                | コメントはドラフト IDに関連付けられ、公開後に破棄されます。                                           | 永続的なコメントと注釈は、監査とコンプライアンスのために保持されます。     |
| **バージョン**           | ドラフトは一意のインスタンスとして扱われます。<br>並べて比較することはできません。                                      | 横並びおよびオーバーレイの比較ツールによる完全なバージョン管理。        |
| **プロジェクト管理** | 基本的なキャンペーン管理： | カスタマイズ、テンプレート、レポート、詳細監査など、キャンペーンのライフサイクル全体を管理。 |

### ライセンスとユーザーの役割

ライセンスは、製品内のユーザーエンタイトルメントのセットを識別します。 Workfront Proofは、GenStudio for Performance Marketingよりも多くのライセンスタイプやユーザーロールを提供しています。 [ プルーフの役割の概要](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles)では、Workfront Proofのレビューと承認のワークフローに関連付けられたユーザーの役割が導入されています。

| GenStudio for Performance Marketing ライセンス       | Workfront ライセンス                 | 説明                                                                                                                                                      |
|---------------------------------------------------|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| GenStudio System Manager                          | Workfront Administrator/Power User | ブランド、ペルソナ、製品管理など、GenStudio Performance Marketingの機能に完全にアクセスできます。 ワークフローと設定を管理します。 承認テンプレートを作成します。 |
| コンテンツ作成者とエディター（パワーユーザーライセンス）   | プルーフクリエイター（標準ライセンス）  | コンテンツのドラフトを生成して送信します。 プルーフビューアで、アセットをアップロードしてプルーフを開始します。 Workfront Proof ライセンスが必要です。                              |
| 審査担当者/承認者（共同作業者ライセンス）        | レビュアー/承認者                 | 多段階のレビューに参加し、コメントを追加し、コンテンツを承認または却下します。                                                                             |

Adobe system administratorsは、Adobe Admin Consoleの両方の製品のユーザープロビジョニングと使用権限を管理します。

>[!NOTE]
>
Workfront Proofには[追加のユーザーロール ](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles)が用意されています。 すべての役割がPerformance Marketing内に表示されるわけではありません。 ただし、Workfront Proof テンプレート内で設定されたすべてのロールが尊重されます。

### ドラフトとプルーフ

Workfront [!DNL Proofing Viewer]は、より構造化されたレビューと承認の機能を使用して、GenStudio for Performance Marketingの基本レビューと承認のプロセスを拡張します。 この統合でレビューされたプルーフは、GenStudio for Performance Marketingでサポートされているフォーマットに限定されます。

### バージョン管理

GenStudio for Performance Marketingは承認テンプレートをサポートしていませんが、Workfront Proofはサポートしています。 Proofのバージョン管理機能は、GenStudioのコンテンツのレビューと承認のプロセスを大幅に強化します。 プルーフワークフローの各送信は、コンテンツドラフトまたは&#x200B;_プルーフ_&#x200B;の個別のバージョンとして扱われます。 プルーフは自動的に保存され、以前のイテレーションと並べて比較できます。 関係者は、レビューサイクル全体を通じて、変更を追跡し、正確なフィードバックを提供して、連携を維持できます。 「プルーフ」では、すべてのコメント、決定、バージョンの履歴が完全に保持され、監査の準備状況とコンプライアンス要件に対応します。 各バージョンは、承認、却下、コメントなど、あらゆるアクションが明確にログに記録され、タイムスタンプが付いた、多段階の役割ベースの承認ワークフローもサポートしています。

### 承認テンプレート

Workfront Proofの承認テンプレートには、プルーフの承認ワークフローを効率化するための、事前にフォーマットされた手順が用意されています。 これらのテンプレートには、選択したレビュー担当者と承認者、プルーフの役割、期限が含まれており、一貫性と効率性を確保します。 レビューを開始するコンテンツ作成者は、単一フェーズと複数フェーズの両方の承認ワークフロー用に、事前に定義された一連のテンプレートから選択できます。

ワークフローテンプレートの各段階で、割り当てられたレビュー担当者が割り当てられます。 Workfront Proof ワークフローのすべてのステータス更新とコメントは、プルーフビューア内に表示され、透明性と共同作業が強化されます。

承認テンプレートは、様々な段階の承認をサポートします。これにより、様々な関係者グループによるレビューの調整が可能になります。

### コメント

レビュー担当者は、プルーフの特定の領域を直接クリックして、正確なコンテキストにもとづくコメントを残すことができます。 すべてのコメントはタイムスタンプ付きで、プルーフのバージョン履歴の一部として保存されます。 コメント履歴はGenStudio for Performance Marketingでは使用できません。

プルーフの2つのバージョンを[比較](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs)して、レビューコメントとコンテンツを評価できます。

## 通知とリマインダー

新しいプルーフがレビュー可能になった場合、または進行中のレビューのステータスが変更された場合、レビュー担当者と承認者にメール通知が送信されます。
[ プルーフの通知とリマインダー](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/proof-notifications-and-reminders/proof-notifications-and-reminders/proof-notifications-and-reminders)には、プルーフへのパーソナライズされたリンク、プルーフと承認プロセスの進捗状況に関する詳細、バージョン情報が含まれます。
