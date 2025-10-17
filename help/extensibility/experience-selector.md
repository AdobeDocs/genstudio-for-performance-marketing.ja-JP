---
title: GenStudio Experience Selector MFE
description: GenStudio アプリおよびアドオン用の Experience Selector マイクロフロントエンドの実装を理解します。
feature: Extensibility, Extensions, Experiences
source-git-commit: d9d6d3825cd953245049de119c66f54274f20fd9
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 6%

---

# GenStudio Experience Selector MFE

エクスペリエンスセレクターは、GenStudio エクスペリエンスを選択するための `ExperienceSelectorDialog` コンポーネントを提供するマイクロフロントエンド（MFE）です。 スタンドアロンのJavaScript バンドルから `renderExperienceSelectorWithSUSI` 関数を読み込むことで、アプリケーション内のコンポーネントを使用します。このバンドルは、デプロイされた最新のマイクロフロントエンドを自動的に読み込み、自然なコンポーネントインターフェイスを表示します。

GenStudio Experience Selector MFE を使用すると、次のことができます。

- GenStudio エクスペリエンスを参照して選択する
- 様々な条件でエクスペリエンスをフィルタリング
- 単一選択モードと複数選択モードの両方をサポート
- SUSI （サインアップログイン）統合による認証の処理
- 異なるフレームワーク間で一貫性のある UI を提供する

## 統合オプション

MFE は、次の 2 つの異なるアプローチを使用して統合できます。

### ESM （ES モジュール）：推奨

```javascript
import { renderExperienceSelectorWithSUSI } from 'https://experience-stage.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/esm/standalone.js';
```

### UMD （Universal Module Definition）

```html
<script src="https://experience-stage.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/umd/standalone.js"></script>
```

## 設定プロパティ

`renderExperienceSelectorWithSUSI` 関数は、次のプロパティを持つ設定オブジェクトを受け入れます。

| Property | タイプ | 必須 | 説明 |
|----------|------|----------|-------------|
| `apiKey` | 文字列 | はい | GenStudio サービスの API キー |
| `imsOrg` | 文字列 | はい | IMS 組織 ID |
| `env` | 文字列 | はい | 環境（`stage`、`prod`） |
| `susiConfig` | object | はい | [SUSI 認証設定 &#x200B;](#susi-configuration) |
| `onSelectionConfirmed` | 関数 | はい | 選択が確定したときのコールバック |
| `onDismiss` | 関数 | はい | ダイアログが閉じたときのコールバック |
| `locale` | 文字列 | いいえ | 言語ロケール（例：`en-US`） |
| `isOpen` | ブール値 | いいえ | 最初のダイアログの状態 |
| `selectionType` | 文字列 | いいえ | 選択モード （`single` または `multiple`） |
| `customFilters` | 配列 | いいえ | カスタムフィルター条件 |
| `dialogTitle` | 文字列 | いいえ | カスタムダイアログのタイトル |

### SUSI 設定

`susiConfig` オブジェクトには、以下が含まれます。

```javascript
{
  clientId: 'genstudio',
  environment: 'stg1', // or 'prod'
  scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
  locale: 'en_US',
  modalSettings: {
    width: 500,
    height: 700
  }
}
```

## QuickStart

1. 以下の使用可能な例から **フレームワークを選択** します
1. **サンプルディレクトリに移動します**。
1. **依存関係をインストール** （React/Vue の例の場合）
1. API キーと IMS 組織を使用して **設定を更新** します。

   ```javascript
   const experienceSelectorProps = {
     locale: 'en-US',
     apiKey: 'exc_app',           
     imsOrg: 'your-ims-org@AdobeOrg',  // Replace with your IMS Org
     env: 'stage', // or 'prod'
     susiConfig: {
        clientId: 'genstudio',
        environment: 'stg1', // or 'prod'
        scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
        locale: 'en_US',
        modalSettings: {
          width: 500,
          height: 700,
        },
     },
     customFilters: ['genstudio-channel:email'],
     selectionType: 'single', // or 'multiple'
     dialogTitle: 'Select Email Templates'
   };
   ```

1. **開発サーバーの実行**

### 実装例

このリポジトリには、様々なフレームワークの使用例が含まれています。

- [Vite ビルドシステムとの統合を示した **完全な React アプリケーション**](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/react-js)。

- [&#x200B; コンポジション API 統合を使用した **Vue 3 アプリケーション**](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vue-js)。

- [2 つの **Vanilla JavaScript実装**](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js):

   - [&#x200B; この **Vanilla ESM** バージョンでは、ES6 モジュールと最新のJavaScriptが使用されています &#x200B;](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-esm)。

   - [&#x200B; この **Vanilla UMD** バージョンでは、スクリプトタグを介して読み込まれた UMD バンドルを使用します &#x200B;](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-umd-global-var)。

## 認証フロー

Experience Selector は、SUSI を通じて次の認証を自動的に処理します。

1. ダイアログが開いたら、既存の認証を確認します。
1. 認証されていない場合、SUSI ログインフローが開きます。
1. 認証が成功すると、エクスペリエンスセレクターが表示されます。
1. ユーザーは、エクスペリエンスを参照して選択できます。
1. 選択したエクスペリエンスは、`onSelectionConfirmed` コールバックを通じて返されます。
