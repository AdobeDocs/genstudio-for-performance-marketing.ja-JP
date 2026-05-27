---
title: コンテンツのレビューと編集
description: Adobe GenStudio for Performance Marketingを使用して、コンテンツを反復的にレビューおよび編集する方法について説明します。
feature: Content Review, Content Management
exl-id: 9a3a15aa-355f-439e-9417-850704402f39
TQID: https://experienceleague.adobe.com/YAUeZkKC0UzOt1fCKgFfXLxGEi2896IpcRTdfwG8KXA
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: e4bd5f48-22a4-465d-a046-5ffb52e27856
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 694
ht-degree: 0%

---

# コンテンツのレビューと編集

レビューと承認の段階では、多くの場合、複数の関係者と反復的なフィードバックが関与するため、コンテンツ制作が遅れる可能性があります。 GenStudio for Performance Marketingの生成AIを利用すれば、コンテンツの修正を迅速化し、このプロセスを合理化できます。これにより、クリエイターは、プロンプトベースの編集を使用して、フィードバックに迅速に対応できるようになります。 レビューサイクルが複雑になればなるほど、GenStudioがもたらす時間の節約というメリットが大きくなります。

## 反復的なドラフト編集

コンテンツエディターは、レビューコメントに応じてコンテンツをプロセス内で編集できます。 ドラフトが変更中の場合、承認者はレビューコメントを追加し続けることができますが、承認ステータスを変更することはできません。 コンテンツエディターは、承認者がレビューを続ける間、キャンバス上のコンテンツの編集を続行できます。

変更が実質的な場合は、すべての関係者に対して[新しいレビューを依頼](/help/user-guide/approvals/request-review.md#request-new-approval)できます。

## 承認要求の表示

指定された承認者は、複数の方法でコンテンツにレビュー用にアクセスできます。

* **承認リクエストの下書きリンクから、レビュー用の下書きに直接アクセスします**。 承認リクエストメールまたは製品内通知の下書きリンクをクリックします。 カンバスが開き、アセットまたはエクスペリエンスが表示されます。 _承認_ パネルが右側に表示されます。

* **承認要求のリストからレビュー用ドラフトにアクセス**。 複数のコンテンツの下書きを確認するように求められた場合、通知メールには「**[!UICONTROL すべての通知を表示]**」ボタンが含まれています。 このボタンをクリックすると、他のAdobe Experience Cloud製品から有効にした承認リクエストや通知など、受信したすべての通知を表示するページに移動します。

## レビュー用コンテンツへのアクセス

アセットやエクスペリエンスのレビューと承認を求める電子メールを受信した場合、コンテンツを承認できます。 このメールには、レビューを依頼された読み取り専用のドラフトへのリンクが含まれています。 このURLは、ドラフトがレビュー中の場合のみ有効です。

**コンテンツをレビューするには**:

1. 実稼動中の通知または電子メールのリンクを使用して、レビュー用のコンテンツに移動します。

   カンバスが開き、レビュー用のコンテンツが表示されます。

1. 右上の「**[!UICONTROL レビューと承認]**」ボタンをクリックします。

   このアセットの&#x200B;_承認_ パネルが開きます。

## リクエストの変更

_承認_ パネルから、提案された変更を一覧表示したり、ドラフトについて質問したりできます。 **作業が必要** ドラフトのステータスは、変更が要求されたことをコンテンツ作成者に通知します。

コンテンツ作成者に対してレビューを行い、編集を提案し、コンテンツを修正し、必要に応じて`@mention`件のコメントを介して追加の入力を求めるこのプロセスは、非常に反復的です。

**変更を要求するには**:

1. ドラフトステータスを&#x200B;**作業が必要**&#x200B;に設定します。

1. 「**コメント**」フィールドにコメントと推奨される変更を入力し、**[!UICONTROL 送信]**&#x200B;をクリックします。

   すべてのレビュー担当者とコンテンツ作成者は、これらのコメントを表示できます。

1. 「**[!UICONTROL レビューと承認]**」をクリックして、**必要な作業**&#x200B;を割り当てます。

   これにより、コンテンツ制作者に電子メールや製品内での通知がトリガーされます。

コンテンツ作成者は、レビューコメントを受信して応答しながら、編集を続行できます。

## Workfront Proofでコンテンツをレビューする

[!DNL Proofing Viewer]には、プルーフに注釈を付けたり、変更を追跡したりするための[堅牢なマークアップツール &#x200B;](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/review-proofs-in-workfront/comment-on-a-proof/comment-on-proof-1)が用意されています。 また、2つのバージョンのプルーフを比較することもできます。

**コンテンツをレビューするには**:

1. メールまたは製品内通知のレビューURLをクリックします。

   GenStudio for Performance Marketingは[!DNL Proofing Viewer] _新しい承認_ ビューを読み込み、レビュー用のプルーフを表示します。

1. ビューアの上部にある「**[!UICONTROL コメントを追加]**」をクリックします。

   「_コメントを追加_」ポップアップが開きます。

1. 「**[!UICONTROL コメントを追加]**」フィールドにコメントを入力します。

1. 「**[!UICONTROL 投稿]**」をクリックします。

   コンテンツ作成者にコメントが通知されます。

### プルーフの比較

[!DNL Proofing Viewer]から、[&#x200B; プルーフのバージョンを比較](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs)できます。

**プルーフを比較**:

1. [!DNL Proofing Viewer]の左上隅にあるプルーフの名前をクリックします。

1. プルーフバージョンの横にある「_比較_」アイコンをクリックします。

   プルーフは横に並べて表示され、左側には新しいバージョンが表示されます。

Workfront Proofには、自動比較ツールなど、プルーフを比較するためのツールがいくつか用意されています。 [比較ツールの使用](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs#use-the-compare-tools)を参照してください。
