---
title: テンプレートでのロゴスワップの設定
description: テンプレートでブランドロゴのプレースホルダーを設定して、 [!DNL GenStudio for Performance Marketing]でロゴの入れ替えを有効にします。
feature: Create Canvas
role: User
level: Intermediate
source-git-commit: 98cb7ba338878495e6d7b68f3b8c620abae10127
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 2%

---

# テンプレートでのロゴスワップの設定

このガイドでは、[!DNL GenStudio for Performance Marketing]の[ ロゴスワップ機能](/help/user-guide/create/logo-swap.md)を有効にするために、テンプレートでブランドロゴプレースホルダーを設定する方法について説明します。 これらのガイドラインを使用して、様々な画像サイズと縦横比でプレースホルダーが正しく表示されるようにします。

## クイックセットアップ

ロゴ画像には、次の基本的なテンプレートコードを使用します。

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="my-logo"
>
```

必須：

- `src="{{brand_logo}}"` - ロゴの入れ替え機能を有効にします。
- `style="{{defaultLogo}}"` - プレースホルダーの境界線スタイルを適用します。

オプション：

- `class="my-logo"` - サイズとスタイル設定のためのカスタム CSS クラス。

## プレースホルダーの境界線について

ロゴが選択されていない場合、`{{brand_logo}}`には透明な1×1 ピクセル画像が含まれます。 `{{defaultLogo}}` スタイルは、自動的にアウトラインを適用して、プレースホルダーが表示されるようにします。

```css
outline: clamp(1px, 0.1em, 5px) dashed #FFF;
```

ボーダーの動作：

- デフォルトのプレースホルダーが表示されたときに表示されます。
- ロゴを入れ替えると、自動的に消えます。
- 親フォントサイズに基づいて拡大・縮小します。

### 境界線のサイズ

`clamp()`関数は、アウトラインの太さをテンプレートのサイズに適応させます。

| 親フォントサイズ | アウトラインのサイズ |
| --- | --- |
| 10px | 1px （分） |
| 16px | 1.6px |
| 24px | 2.4px |
| 32px | 3.2px |
| 50px+ | 5px （最大） |

数式：`0.1em`は、継承されたフォントサイズの10%に相当し、`1px`から`5px`の間でクランプされます。

## プレースホルダーの境界線のカスタマイズ

CSS クラスを使用して、デフォルトのアウトラインを上書きできます。 `{{defaultLogo}}` スタイルはベースのアウトラインを適用し、クラスは色、幅、スタイルをカスタマイズできます。

Template HTML:

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-custom-border"
>
```

テンプレート CSS:

```css
.logo-custom-border {
  outline-color: #0066CC !important;
  outline-width: 2px !important;
  outline-style: dotted !important;
}
```

>[!NOTE]
>カスタムアウトラインスタイルは、プレースホルダーにのみ影響します。 ロゴを入れ替えると、すべてのアウトラインスタイルが自動的に削除されます。

## 推奨ロゴサイズの設定

プレースホルダーが表示され、レイアウトシフトを防ぐには、CSS クラスで明示的なサイズ設定を行います。

Template HTML:

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-standard"
>
```

テンプレート CSS:

```css
.logo-standard {
  width: 120px;
  height: 60px;
}
```

## ロゴの配置の制御

`object-fit`と`object-position`を使用して、ロゴのコンテナ内での拡大・縮小を制御します。

### 中央に配置されたロゴ（最も一般的）

ロゴは、水平方向と垂直方向の両方の中央に150×80 ピクセル以内に収まるように拡大します。

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-centered"
>
```

```css
.logo-centered {
  width: 150px;
  height: 80px;
  object-fit: contain;
  object-position: center center;
}
```

### 左揃えロゴ

ロゴは左端に揃え、垂直方向に中央に合わせて拡大・縮小します。

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-left"
>
```

```css
.logo-left {
  width: 200px;
  height: 60px;
  object-fit: contain;
  object-position: left center;
}
```

### 右上隅にロゴ

ロゴは右上隅に配置され、フィットするように拡大・縮小されます。

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-top-right"
>
```

```css
.logo-top-right {
  width: 100px;
  height: 100px;
  object-fit: contain;
  object-position: right top;
}
```

## 完全な例

### 最小限の設定

```html
<img src="{{brand_logo}}" style="{{defaultLogo}}">
```

>[!NOTE]
>この設定は機能しますが、透明な1×1 ピクセル画像が自然なサイズに折りたたまれるため、プレースホルダーがほとんど見えない場合があります。 表示されるプレースホルダーには、`width`と`height`のCSS クラスを使用します。

### 推奨される設定

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="brand-logo"
>
```

```css
.brand-logo {
  width: 120px;
  height: 60px;
  object-fit: contain;
  object-position: center center;
}
```

### カスタム枠線を使用した詳細設定

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="sponsor-logo"
>
```

```css
.sponsor-logo {
  width: 180px;
  height: 90px;
  object-fit: contain;
  object-position: left center;
  outline-color: #0066CC !important;
  outline-width: 2px !important;
  outline-style: solid !important;
}
```

### サイズの境界を持つ柔軟な設定

レスポンシブテンプレートや様々なロゴサイズには、`min-*`および`max-*`のプロパティを使用します。

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-flexible"
>
```

```css
.logo-flexible {
  min-width: 20px;
  min-height: 20px;
  max-width: 200px;
  max-height: 100px;
  object-fit: contain;
  object-position: center center;
}
```

仕組み：

- `min-width`と`min-height`は、プレースホルダーを表示したままにします。
- `max-width`と`max-height`は、大きすぎるロゴがレイアウトを壊さないようにします。
- ロゴは、これらの境界内で比例して拡大・縮小されます。

## CSS プロパティリファレンス

| カテゴリ | プロパティ | 値 | 目的 |
| --- | --- | --- | --- |
| 必須（HTML） | `src` | `{{brand_logo}}` | ロゴの入れ替え機能を有効にします。 |
| 必須（HTML） | `style` | `{{defaultLogo}}` | プレースホルダーのアウトラインを適用します。 |
| 推奨（CSS クラス） | `width` | `120px` | ロゴの最大幅を設定します。 |
| 推奨（CSS クラス） | `height` | `60px` | ロゴの最大の高さを設定します。 |
| 推奨（CSS クラス） | `object-fit` | `contain` | 切り抜かずにロゴを拡大・縮小します。 |
| 推奨（CSS クラス） | `object-position` | `center center` | ロゴの整列を制御します。 |
| オプション （CSS クラス） | `outline-color` | `#FF0000` | アウトラインの色を変更します。 |
| オプション （CSS クラス） | `outline-width` | `3px` | アウトラインの太さを変更します。 |
| オプション （CSS クラス） | `outline-style` | `solid` | アウトラインのスタイルを変更します。 |
| 柔軟なサイズ変更（CSS クラス） | `min-width` | `20px` | プレースホルダーの可視性を確保します。 |
| 柔軟なサイズ変更（CSS クラス） | `min-height` | `20px` | プレースホルダーの可視性を確保します。 |
| 柔軟なサイズ変更（CSS クラス） | `max-width` | `200px` | オーバーフローの防止： |
| 柔軟なサイズ変更（CSS クラス） | `max-height` | `100px` | レイアウトの境界を制御します。 |

## ベストプラクティス

実行：

- 常に`{{brand_logo}}`と`{{defaultLogo}}`を含める。
- プレースホルダーが表示されるように`width`と`height`を定義します。
- サイズとアウトラインのカスタマイズにCSS クラスを使用します。
- `object-fit: contain`を使用してロゴの縦横比を保持します。
- さまざまなサイズや縦横比のロゴでテストしましょう。

悪い例：

- `outline`の代わりに`border`を使用してください（境界線は自動的に非表示にされません）。
- インラインスタイルにサイズプロパティを設定します。
- サイズの制約を省略します（プレースホルダーは1×1 ピクセルでレンダリングされます）。
- `object-fit: cover`を使用してください（ロゴが切り抜かれる可能性があります）。

## トラブルシューティング

境界線が表示されない：

- `style="{{defaultLogo}}"`が含まれていることを確認します。
- `width`と`height`がCSS クラスで定義されていることを確認します。

プレースホルダーが小さすぎます（1 px）:

- CSS クラスに明示的な`width`と`height`を追加します。

スワップ後に境界線が消えない：

- CSS クラスで`border`ではなくアウトライン プロパティを使用してください。

ロゴが切り抜かれます。

- `cover`の代わりに`object-fit: contain`を使用してください。

ロゴが小さすぎるか、大きすぎるか：

- CSS クラスで`width`と`height`を調整します。

カスタムの境界線が表示されない：

- `{{defaultLogo}}`が`style`属性にあることを確認してください。
- CSS クラスにカスタム `outline-*` プロパティを配置します。
