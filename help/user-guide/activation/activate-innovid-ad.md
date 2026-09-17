---
title: Innovid広告をアクティベートする
description: Innovid エクスペリエンスをアクティブ化する方法について説明します。
feature: Ad Activation
exl-id: ebb2aa9e-8efb-45b0-9ba2-7b27b8888708
TQID: https://experienceleague.adobe.com/VTzk2CDlTqawM1ckdHPVzs2ES-y0Ui0mkOLnVD88bJk
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%
---
# Innovid広告をアクティベートする

Adobe GenStudio for Performance Marketingは、Innovidへの広告体験のアクティベーションをサポートしています。

**サポートされている形式**：静的ディスプレイ、HTML5 Zip ディスプレイ。

Innovid エクスペリエンスのアクティベーションは、他の有料広告チャネルへのアクティベーションに必要な[同じ一般的な手順](create-activation.md)に従います。 このページでは、Innovid固有の前提条件と設定フィールドについて説明します。 GenStudio for Performance Marketingでエクスペリエンスをアクティベートしたら、Innovidを使用してエクスペリエンスを確認し、広告を起動します。

GenStudioのシステムマネージャーやエディターは、

## 前提条件

* ターゲット Innovid アカウントへのアクセス。
* Innovidへの読み取りおよび書き込みをおこなうためのアカウントへの管理者アクセス権。

Innovidは、複数のアカウント内でキャンペーンや広告を展開しており、各アカウントにはクリエイティブライブラリがあります。 ターゲットクリエイティブライブラリは、Innovidに既に存在している必要があります。GenStudio for Performance Marketingは、そのクリエイティブライブラリに広告エクスペリエンスを公開しますが、アカウントやクリエイティブライブラリは作成しません。

## Innovid アカウントを接続する

クリエイティブライブラリでアセットを公開する前に、GenStudioのシステムマネージャーがInnovid アカウントをGenStudio for Performance Marketingに接続する必要があります。 Innovidへの読み取りおよび書き込みには、そのアカウントへの管理者アクセス権が必要です。 [有料メディアアカウントの接続](/help/user-guide/connectors/connect-channel.md)を参照してください。

同期が完了したら、追加されたアカウントを表示できます。

## Innovid設定フィールド

承認されたアセットは[!DNL Content]でレビューと承認が完了しているため、アクティブ化中はロックされ、編集できません。 次の項目を編集できます。

* **テキストフィールド**: トラッキング ID （プラットフォームのクリエイティブ名として使用）
* **プラットフォーム設定フィールド**：アカウント、Creative ライブラリ、コンセプト名

アクティベーションが完了すると、Innovidで選択したクリエイティブライブラリにクリエイティブ体験が配信されます。
