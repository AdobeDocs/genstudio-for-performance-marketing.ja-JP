---
title: App Builder アプリケーションのデプロイ
description: GenStudio for Performance Marketing用のApp Builder アプリまたはアドオンをデプロイします。
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
source-git-commit: 7fdd3f54a0a031bfe26b48983de9cd24baad2f62
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# アプリのデプロイ

アプリを実行すると、デプロイ前にアドオンの動作の予備スナップショットが提供されます。 この情報はデバッグを容易にします。

**アプリを実行するには**:

`https://localhost:9080` でアプリを実行します。

```bash
aio app run
```

**アプリをデプロイするには**:

1. デプロイメント ワークスペースに移動します。

   ```bash
   aio app use -w [deployment_workspace]
   ```

2. アプリをデプロイします。

   ```bash
   aio app deploy
   ```

**再デプロイメントを強制的に実行するには**:

アプリを承認用に再送信しなくても、アプリのビルドとデプロイメントを強制的に行うことができます。

>[!NOTE]
>
>ビルドおよびデプロイメントを強制的に実行すると、既存のデプロイメントが上書きされます。 最初にテスト環境で **アプリを十分にテストします**。

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

```txt
https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create
```

アドオンに満足したら、`query` パラメーターを指定せずに配布する準備が整います。

これで、[ アプリを配布 ](distribute-app.md) できます。
