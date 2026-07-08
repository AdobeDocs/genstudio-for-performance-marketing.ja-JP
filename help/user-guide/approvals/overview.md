---
title: Adobe GenStudio for Performance Marketing のレビューと承認
description: GenStudio for Performance Marketing のレビューおよび承認プロセスについて説明します。
level: Beginner
feature: Content Review, Content Management
exl-id: c83f47c0-e8ae-4c54-84b3-c50f67d6b3c2
TQID: https://experienceleague.adobe.com/2oFwfqVPlW24irHth-mkEx-ciO5tQgNv2hwAYmkfi-g
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: e5011c95e9536d73b1f09d6bc76bb83f121573cd
workflow-type: ht
source-wordcount: 890
ht-degree: 100%

---

# Adobe GenStudio for Performance Marketing のレビューと承認

レビューと承認のワークフローにより、クリエイティブチームから法務のエキスパートに至るまで、すべての関係者が、生成 AI で作成されたブランドアセットを含むキャンペーン用のアセットやエクスペリエンスを、効率的にレビューおよび承認できます。

>[!NOTE]
>
> この機能は、[Adobe Workfront Proof との統合](/help/user-guide/approvals/proof-integration.md)としても使用できます。この統合により、GenStudio for Performance Marketing のキャンバスに対してプルーフ機能が提供されます。Workfront Proof との統合により、GenStudio for Performance Marketing は、より構造化され、透明性の高い、共同作業に適したレビュープロセスを実現します。これにより、チームは信頼性と明確性を持って、ドラフトから最終版へと作業を進めることができます。

## レビューと承認ワークフローの利点

* **堅牢で反復的な生成 AI コンテンツ制作のサポート**。組織内でブランドに一致したコンテンツを作成してデプロイすることは、高度に反復的なプロセスです。GenStudio for Performance Marketing の生成 AI 機能は、数百ものアセットバリアントの迅速な作成をサポートします。各レビュアーは、アセットのドラフトを承認する前に、複数の変更をリクエストする可能性があります。レビュアーの数が増えるほど、すべての関係者が最終なバリアントに合意する前に可能性のある反復の回数も増加します。

* **クリエイティブの整合性のサポート**。承認プロセスにコンテンツ制作者を関与させることで、ブランドアセットのクリエイティブな整合性が保護されます。クリエイティブ関係者（例：コンテンツ作成者やクリエイティブディレクター）をレビューと承認のプロセスに関与させることで、最終的な出力がビジョンやブランドアイデンティティと一致します。

* **キャンペーン目標と法的要件の遵守**。承認プロセスは、コンテンツがキャンペーン目標をサポートしているかどうかを確認するのに役立ちます。これにより、すべてのマーケティング資料が法的および規制上の標準に適合することを確保し、リスクや潜在的な法的問題を最小限に抑えます。

* **Adobe Workfront Proof との統合**。ユーザーは、GenStudio for Performance Marketing 内から、Workfront Proof の堅牢なレビューと承認機能にアクセスできます。GenStudio for Performance Marketing でレビューされたコンテンツは Workfront Proof に同期され、レビューコメントとステータスは保持されます。[統合のハイライト](/help/user-guide/approvals/proof-integration.md)では、Proof が GenStudio for Performance Marketing の承認ワークフローを拡張する仕組みについて説明します。

## レビューと承認のライフサイクル

レビューと承認のワークフローの主なフェーズは次のとおりです。

* [作成したコンテンツのレビューと承認をリクエストします](/help/user-guide/approvals/request-review.md)。GenStudio for Performance Marketing は、承認リクエストや承認者の管理といったプロセスを効率化します。Workfront Proof の承認テンプレートを使用すると、このタスクをさらに簡素化できます。

* [コンテンツをレビューおよび編集します](/help/user-guide/approvals/review-and-edit.md)。変更リクエストや承認状況に関する通知が届くので、コンテンツ作成者は常に最新の状況を把握できます。コンテンツを修正すると、新しい承認サイクルが自動的に開始されます。

* [コンテンツを承認します](/help/user-guide/approvals/approve-content.md)。指定された承認者が、コンテンツを「承認済み」または「公開準備完了」としてマークします。

* [コンテンツを公開します](/help/user-guide/approvals/publish-content.md)。承認済みコンテンツを [!DNL Content] に公開すると、組織内の他のメンバーがそのコンテンツを使用または参照できます。

## コンテンツドラフトについて

_ドラフト_&#x200B;とは、レビューと承認のプロセスが完了していないアセットやエクスペリエンスの暫定バージョンのことです。ドラフトのステータスは、そのドラフトがレビューと承認プロセスのどの段階にあるかを示します。各ドラフトは、一意のドラフト ID によって識別されます。この ID は、ドラフトが承認され、[!DNL Content] として公開されるまで有効です。ドラフトに対するレビューコメントや承認は、この個別のドラフト ID に関連付けられます。GenStudio コンテンツドラフトには、バージョン管理はありません。

ドラフトがレビューと承認のプロセスを完了し、[!DNL Content] として公開されると、そのドラフト ID は有効期限が切れます。GenStudio for Performance Marketing は、関連するコメントや承認ステータスを保存しません。ドラフト URL は有効ではなくなりました。

ドラフトのステータスは、レビューと承認のプロセスを通じてコンテンツドラフトの状態を表します。レビュー中のコンテンツを作成した GenStudio for Performance Marketing コンテンツ編集者には、ドラフトに対する変更リクエストや承認の通知が届きます。承認者は、ドラフトにさらなる修正が必要か、承認可能かを示すために、ドラフトのステータスを変更します。アセットやエクスペリエンスを公開する前に、指定されたすべての承認者による承認が必要です。

使用可能なドラフトのステータス：

**通知**：コンテンツ編集者は、レビュー用のドラフトが準備完了したことを承認者に通知し、レビューと承認のプロセスを開始しました。
**作業が必要**：1 人以上の承認者がコンテンツのドラフトに対する変更をリクエストしたことを示します。このステータスのコンテンツは、[!DNL Content] に保存できません。
**承認済み**：指定されたすべての承認者が、アセットまたはエクスペリエンスを承認しました。コンテンツ編集者は、アセットやエクスペリエンスにメタデータを追加し、[!DNL Content] に保存できるようになりました。

>[!NOTE]
>
> Workfront Proof 統合のユーザーにとって、ドラフトは&#x200B;_プルーフ_&#x200B;に相当します。[ドラフトとプルーフ](/help/user-guide/approvals/proof-integration.md#drafts-and-proofs)は、永続性とバージョン管理の点で異なります。

## 承認の役割

_レビュアー_&#x200B;はコメントを追加できますが、コンテンツを承認できません。レビュアーの参加は役に立ちますが、必須ではありません。コンテンツが承認プロセスを進むには、_承認者_&#x200B;がそのコンテンツを承認する必要があります。Workfront Proof の統合は、より幅広いユーザーの役割をサポートしています。

## 通知

GenStudio for Performance Marketing の製品内通知では、アセットのステータス変更や `@mention` コメントについて、承認者やコンテンツ編集者にリアルタイムで通知します。通知では、複数のレビュー、編集、承認サイクルを通じて、迅速な反復をサポートします。

コンテンツの編集者や承認者は、Slack でこれらの通知を受信するように新規登録できます。[CX Enterprise のサービスへの登録](https://experienceleague.adobe.com/ja/docs/core-services/interface/services/customer-attributes/subscription)を参照してください。

承認参加者が実行したアクションは、製品内での通知やメール通知を自動的にトリガーします。承認プロセスを開始すると、指定された承認者は、メールと製品内通知の両方を受信します。承認者が `@mention` コメントを追加したり、決定したりするたびに、製品内通知やメール通知で最新状況が随時共有されます。通知には、コンテンツのドラフトへのリンクが含まれます。

コンテンツのレビューと承認プロセスを開始した場合、すべての承認とレビューのコメントについて通知を受信します。ただし、承認者に通知されるのは、`@mention` を含む自身が含まれたコメントのみです。
