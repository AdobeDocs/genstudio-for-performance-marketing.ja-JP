---
title: テンプレートの操作
description: Adobe GenStudio for Performance Marketingでテンプレートを効果的に使用して、クリエイティブプロセスを効率化する方法をご確認ください。
level: Intermediate
role: Developer
feature: Media Templates
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
TQID: https://experienceleague.adobe.com/kXXSni5VZMFH615A-Re1-QjLooEyfXcMwVBwXnxp58s
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: c95c94c1-727b-457a-9184-a4dda4c95ab2id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2: id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: cc72dcf1-72e1-48cc-b434-e7c27d62d67cid: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 70984b2c03e14a14b36fca6dfc62dcda9138949e
workflow-type: tm+mt
source-wordcount: 1410
ht-degree: 1%

---

# テンプレートの操作

GenStudio for Performance Marketingを使用すると、コンテンツ制作者は&#x200B;_テンプレート_&#x200B;を使用して、ブランドに即したマーケティングコンテンツを迅速に作成できます。 テンプレートを利用すれば、事前に設定されたレイアウトやデザイン要素をベースにコンテンツを作成するための時間と労力を大幅に削減できます。 開始するには、[!DNL Content]でカスタムテンプレートをアップロードするか、[!DNL Create]でスターターテンプレートを使用します。 [ スターターテンプレート ](/help/user-guide/templates/starter-templates.md)を使用すると、標準デザインをすばやく開始できます。また、カスタムテンプレートを使用すると、独自のデザインとレイアウトを使用できます。

GenStudio for Performance Marketingでは、アプリケーション内でテンプレートを直接作成することはサポートされていませんが、Adobe InDesign、Illustrator、Expressなどの一般的なデザインツールを使用して、テンプレートを容易にデザインおよび作成できます。 デザインが完成したら、GenStudio for Performance Marketingで使用するように調整できます。 テンプレートの使用を開始するには、次の手順に従います。

1. **テンプレートをデザイン**：好みのデザインツールを使用して、プリヘッダー、見出し、本文、CTA、画像、フッターなどの要素](#template-elements)を含む[ テンプレートのビジュアルレイアウトを作成します。

2. **テンプレートをコーディング**：デザインをHTMLとインライン CSSに変換して、様々なデバイスでクリーンでレスポンシブなデザインにすることができます。 ターゲットとするオーディエンスを最大限に引き出すために、[ アクセシビリティガイドライン ](accessibility-for-templates.md)を検討してください。

3. **GenStudio for Performance Marketingの準備**: Handlebars テンプレート言語を使用してHTML テンプレートを調整します。 GenStudio for Performance Marketingでコンテンツを動的に生成する場所を示すプレースホルダーを挿入します。 GenStudio for Performance Marketingのテンプレートを[ カスタマイズ ](customize-template.md)する方法を参照してください。

次の手順に従うことで、GenStudio for Performance Marketingで使用できるプロフェッショナルで効果的なテンプレートを作成でき、ブランドに即したコンテンツを迅速かつ効率的に制作できます。

## テンプレート要素

テンプレートとは、HTMLとインライン CSSで定義された一連の命令で、メール、ソーシャル広告、ディスプレイ広告エクスペリエンスの作成に使用できます。 テンプレート要素は、コンテンツ作成に使用する構造を提供します。

以下は、テンプレートで使用される要素のリストと、その特徴に関する詳細です。

| **要素** | **チャネル** | **説明** |
|----------------------|------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **プリヘッダー** | メール | 通常、40～50文字の電子メールの件名を2番目に作成します。これにより、件名が強調されます。 電子メールを開く前に、件名と共に受信トレイに表示されます。 |
| **ヘッダー** | メール | 電子メールを開封すると受信者に表示される電子メールの上部セクションで、トーンを設定し、含まれるコンテンツのコンテキストを提供します。 |
| **見出し** | Meta広告、バナー広告、ディスプレイ広告、LinkedIn | 受信者が最初に見るコンテンツは、興味を引くために説得力のあるものでなければなりません。 |
| **小見出し** | 電子メール、バナー、ディスプレイ広告 | 見出しをサポートするセカンダリテキスト要素。 通常、メインの見出しを補完するために簡潔に設計されており、読者の注目をコンテンツにさらに引き込みます。 |
| **概要テキスト** | LinkedIn | プライマリメッセージは、本文コピーと同様に、コアメッセージを伝えます。 スペース、最大4つの絵文字、句読点など、最大150文字を使用できます。 |
| **本文** | 電子メール、Meta広告、バナー、ディスプレイ広告 | 広告のメインテキストは、コアメッセージを伝えます。 オーディエンスが望ましい行動を起こすように促すことが、魅力的かつ有益で、説得力のあるコンテンツである必要があります。 |
| **CTA** | 電子メール、Meta広告、バナー広告、ディスプレイ広告、LinkedIn | Call-to-actionのボタンは、フレーズとリンクを使用して、リンクのクリックや購入など、オーディエンスに特定のアクションを促します。 |
| **画像** | 電子メール、Meta広告、バナー広告、ディスプレイ広告、LinkedIn | ビジュアルアピールを強化し、テキストを分割し、メッセージをサポートします。 画像は、高品質で魅力的なものにする必要があります。 |
| **フッター** | メール | メールの下部には、問い合わせ情報、ソーシャルメディアリンク、免責事項、配信停止オプションなどの追加コンテンツが記載されています。 |
| **テキストオーバーレイ** | Meta広告 | 見出しと本文のコンテンツをサポートおよび強化するために、画像上に配置されたテキスト。 |

>[!TIP]
>
>各チャネルタイプのテンプレートでGenStudio for Performance Marketingがサポートする[認識済みフィールド名](customize-template.md#recognized-field-names)を参照してください。

## テンプレートをカスタマイズ

GenStudio for Performance Marketingで使用するために、生成AIがコンテンツの挿入に使用するコンテンツプレースホルダー（フィールド）を挿入して、テンプレート ](customize-template.md)を[ カスタマイズします。 GenStudio for Performance Marketingは、`body` フィールドなどの特定のフィールドを認識し、選択したブランドに設定されたチャネルガイドラインに従います。

>[!TIP]
>
>[ アクセシビリティガイドライン ](accessibility-for-templates.md)と[ ベストプラクティス ](/help/user-guide/templates/best-practices-for-templates.md)に従って、より多くのオーディエンスにリーチし、最適なエクスペリエンスを提供してください。

## テンプレートの管理

_[!DNL Templates]_ギャラリーには、GenStudio for Performance Marketingでエクスペリエンスを生成するためにカスタマイズされたテンプレートのインベントリが表示されます。

### テンプレートを検索

各[!DNL Content] ビューには、理想的なアセット、エクスペリエンス、テンプレートを絞り込むためのフィルターオプションが用意されています。 [ ガイドライン ](/help/user-guide/guidelines/overview.md)、[ キーワード ](../content/asset-details.md#user-defined-metadata)、[属性カテゴリ ](/help/user-guide/insights/attributes.md#categories)に基づくフィルターがあり、検索結果が絞り込まれます。

例えば、自分で作成した特定のチャネルタイプまたはアスペクト比のテンプレートを見つける場合があります。

- **[!UICONTROL 作成者]**：自分または特定のユーザーが作成したテンプレートのみを表示するように、_[!UICONTROL テンプレート]_ リストを制限します。
- **[!UICONTROL 縦横比]**：特定の縦横比に合わせてデザインされたテンプレートを表示するには、_[!UICONTROL テンプレート]_&#x200B;のリストを制限します。

次に、電子メール、ディスプレイ広告、Meta広告、LinkedIn広告などのチャネルタイプでフィルタリングを示します。

![ コンテンツテンプレートリスト ](/help/assets/content-templates-filter.png "LinkedIn テンプレートの検索"){width="650"}

テンプレート検索機能は、所有メディアまたは有料メディア用のテンプレートを選択する際に[!UICONTROL 作成]中に利用できます。 特定のフィルターオプションが表示されない場合は、リポジトリ内のテンプレートが対応するメタデータ条件に一致していないことを示します。 テンプレートにメタデータのタグ付けが適切におこなわれていることを確認し、これらのフィルターを通じてテンプレートを検索できるようにします。

### テンプレートを追加

テンプレートをアップロードする前に、[ テンプレートをカスタマイズ ](customize-template.md)のガイダンスに従って、テンプレートが完全に準備され、GenStudio for Performance Marketingで使用できる状態になっていることを確認してください。

**テンプレートを追加するには**:

1. _[!DNL Content]_で、「**[!UICONTROL テンプレート]**」セクションを選択します。

2. 「**[!UICONTROL テンプレートを追加]**」をクリックします。

3. _[!UICONTROL 承認済みテンプレートを追加]_ ペインで、HTML テンプレートファイルを参照するか、HTML テンプレートファイルをドロップスペースにドラッグします。 「**[!UICONTROL 次へ]**」をクリックします。

4. _[!UICONTROL 検出されたフィールドを確認]_ ペインで、フィールドを確認します。 正しいテンプレートを使用していること、およびすべての詳細が期待どおりに表示されていることを確認します。

   メールテンプレートのプレビューの例：

   ![ プレビューフィールドが検出されました](/help/assets/template-detected-fields.png){width="650"}

   >[!TIP]
   >
   >テンプレートが正しくない場合は、**[!UICONTROL 戻る]**&#x200B;をクリックし、前の手順に戻ります。 修正したテンプレートファイルをアップロードします。 または、[ テンプレートコードエディター](/help/user-guide/templates/code-editor.md)を使用して簡単に修正できます。

5. テンプレートのプレビューに問題がなければ、**[!UICONTROL 次へ]**&#x200B;をクリックします。

6. _[!UICONTROL テンプレートの詳細を入力してアップロード]_&#x200B;で、テンプレートに名前を付け、**[!UICONTROL チャネル]** タイプを選択します。

   テンプレート名とチャネルタイプが必要です。 その他の要件には、次のようなものがあります。

   - **Meta**：縦横比が必要
   - **バナーとディスプレイ広告**：ディメンションが必要

7. 検索とフィルタリングでテンプレート識別を改善するために、できる限り多くの詳細を追加します。

8. 「**[!UICONTROL 完了]**」をクリックします。

### テンプレートを更新

テンプレートには、アイコンやロゴなどの静的ファイルを含めることができます。 テンプレートのプレビューを作成した後、[静的コンテンツ ](/help/user-guide/templates/customize-template.md#static-content)は保存されません。 GenStudio for Performance Marketingは、テンプレートで提供されるソースリンクを引き続き参照します。 更新を使用して、これらのアセットの最新バージョンでテンプレートプレビューを更新します。

**テンプレートを更新するには**:

1. _[!DNL Content]_で、「**[!UICONTROL テンプレート]**」セクションを選択します。

2. テンプレートをクリックすると、全体表示と詳細のリストが表示されます。

3. 右上隅の&#x200B;**[!UICONTROL 更新]** （矢印を丸で囲む）をクリックして、テンプレートで使用されているすべてのアセットの更新を実行します。

### テンプレートを使用したエクスペリエンスの作成

GenStudio for Performance Marketingの既存のテンプレートを検索して利用し、より多くのエクスペリエンスを作成します。

**テンプレートを使用してエクスペリエンスを作成するには**:

1. _[!DNL Content]_で、「**[!UICONTROL テンプレート]**」セクションを選択します。

2. テンプレートをクリックすると、全体表示と詳細のリストが表示されます。

3. 右上隅の「**[!UICONTROL エクスペリエンスを作成]**」（ペイントブラシ）をクリックして、テンプレートを使用します。

4. エクスペリエンスの[作成](/help/user-guide/create/overview.md#create-use-cases)を続行します。

## AJOとMarketoのテンプレート

Adobe Journey Optimizer（AJO）またはMarketoで作成したテンプレートをアップロードできます。 GenStudio for Performance Marketingは、アプリケーション固有のパターンを検出して無視し、AJOまたはMarketoで使用するために元のフォームを保持します。 元のAJOまたはMarketoの構文を変更する必要はありません。

GenStudio内のJourney Optimizer ライブラリからAJO テンプレートを使用するには（メールエクスペリエンスの作成時に「**[!UICONTROL AJO テンプレート]**」タブを含む）、Adobe Exchangeから[Journey Optimizer for GenStudio](/help/extensibility/journey-optimizer-for-genstudio.md) アプリをインストールして設定する必要があります。

認識されるアプリケーションパターンは次のとおりです。

- **AJO**: `{{profile.*}}`、`{{context.*}}`
- **Marketo**: `{{my.*}}`、`{{lead.*}}`、`{{system.*}}`

>[!BEGINSHADEBOX]

**前提条件**

- アプリケーション（AJO、Marketo）とGenStudio for Performance Marketingは、統合のために同じIMS組織に属している必要があります
- ユーザーは、「共同作業者」の役割（最下位）以上である必要があります

>[!ENDSHADEBOX]

次に、[ テンプレートをプレースホルダーで](/help/user-guide/templates/customize-template.md) カスタマイズして、GenStudio for Performance Marketingでコンテンツを生成する場所を指定します。 [ テンプレート ](#add-a-template)を[!DNL Content] リポジトリに追加し、テンプレートを検証します。 コードエディターを使用して軽微な修正を行います。
