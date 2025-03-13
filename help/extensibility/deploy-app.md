---
title: App Builder アプリケーションのデプロイ
description: GenStudio for Performance Marketing用のApp Builder アプリまたはアドオンをデプロイします。
source-git-commit: acc54215d980f1f7392401cca9d90ed0ce41b2ec
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---


# アプリのデプロイ

アプリを実行すると、デプロイ前にアドオンの動作の予備スナップショットが得られます。 この情報はデバッグを容易にします。 アプリケーションを承認用に再送信しなくても、デプロイ済みのアプリケーションのビルドとデプロイメントを強制できます。


**アプリを実行するには**:

`https://localhost:9080` でアプリを実行します。

```bash
aio app run
```

**アプリをデプロイするには**:

1. デプロイメントワークスペースに移動します。 例えば、実稼動ワークスペースに移動するには、次の手順を実行します。

   ```bash
   aio app use -w Production
   ```

1. アプリをデプロイします。

   ```bash
   aio app deploy
   ```

**再デプロイメントを強制的に実行するには**:

>[!NOTE]
>
>ビルドおよびデプロイメントを強制的に実行すると、既存のデプロイメントが上書きされます。 最初に、テスト環境でアプリのテストを十分に行います。

```bash
aio app build --force-build
```

```bash
aio app deploy --force-deploy
```

**ビルドとデプロイを同時に行うには**:

```bash
aio app deploy --force-build --force-deploy
```

**アプリを表示するには**:

デプロイ後、GenStudio for Performance Marketingの URL に `query` パラメーターを追加することで、GenStudio for Performance Marketingでアプリを表示できます。

`https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create`

アドオンに満足したら、`query` パラメーターを指定せずに配布する準備が整います。

これで [ アプリを配布 ](distribute-app.md) できます。
