---
title: 新しいインスタンスの整理と命名規則の確立
description: Marketo Engageインスタンス内に優れた組織を設定する方法を説明します。これにより、組織内の将来のマーケターがプログラム間を簡単に移動し、アセットを変更して、レポートを取り込めるようになります。
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-03T00:00:00Z
jira: KT-14813
thumbnail: KT-14813.jpeg
exl-id: 19b3de9e-53f3-4308-b46e-7b8f756c30a0
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 2%

---

# 新しいインスタンスの整理と命名規則の確立

新しいMarketo Engageインスタンスを実装する管理者は、組織内の今後のマーケターがインスタンス内を簡単に移動できるように、基盤を構築します。 ツリーフォルダーの構造と命名規則に慣れることで、インスタンスを整頓し、長期的な成功に向けて設定できます。 このチュートリアルには、AdobeおよびMarketo Engageチャンピオン（2019～2020）の Natalie Kremer が推奨する例が含まれており、[ フォルダーを整理し、アセットに一貫した名前を付ける ](https://nation.marketo.com/t5/champion-program-blogs/keep-marketo-engage-organized-with-folders-and-naming/ba-p/245630){target="_blank"} のに役立ちます。

## フォルダーの構造化と命名規則の適用が必要な理由

インスタンス内で整理しておくことで、自分自身や同僚がキャンペーン、プログラム、アセットを追跡したり、プログラムのパフォーマンスをレポートしたりすることが容易になります。 インスタンス内のナビゲーションツリーを整理し、大規模に構築するには、[ フォルダー ](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-folders){target="_blank"}、[ 標準の命名規則 ](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs#naming-schemes){target="_blank"}、および [ クローン作成 ](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs#cloning){target="_blank"} などの機能を使用することをお勧めします。

## Marketo Engageインスタンスの整理方法

>[!VIDEO](https://video.tv.adobe.com/v/3422765/?quality=12&learn=on&captions=jpn)

### 手順 1 - プログラムを整理するためのフォルダー構造の設定

インスタンスを整理する最初の手順は、[ フォルダー構造を設定 ](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/create-new-campaign-folder.html?lang=ja) し、プログラムとアセットを見つけやすく整然と格納することです。

ツリー内のフォルダーを構造化する際のクイックヒントを次に示します。

* 検出性を確保するために、フラットなフォルダー構造を維持します。
* 組織のチーム構造（地域やチームなど）またはイニシアチブ（ニュースレターなど）を反映するようにフォルダーを構築します。
* 時間ベースのラベルを含めて、検索性を有効にし、アーカイブに適したタイミングを知らせます（例：2024 年）。
   * 管理者は、少なくとも年に 1 回フォルダーをアーカイブすることをお勧めします。 年次フォルダー名を使用して、ライブスマートキャンペーンを簡単に非アクティブ化し、年末にフォルダー全体をアーカイブできます。

以下は、これらのヒントを実践するフォルダーの例です。

**ツリー内のフォルダー名**

>[!BEGINTABS]

>[!TAB マーケティングアクティビティ]

![ フォルダーマーケティングアクティビティ ](/help/marketo-tutorial-implementing-new-instance/assets/folders-marketing-activities.png)

>[!TAB Design Studio]

![Folder Design Studio](/help/marketo-tutorial-implementing-new-instance/assets/folders-design-studio.png)

>[!TAB データベース]

![ フォルダーデータベース ](/help/marketo-tutorial-implementing-new-instance/assets/folders-database.png)

>[!ENDTABS]

### 手順 2 - プログラム内でのフォルダーの作成

次に、プログラムレベルでフォルダー構造を適用します。 ベストプラクティスとして、ローカルアセットをサブフォルダーに格納すると、プログラムを整理し、内部ユーザーがプログラムを効率的に変更またはレポートできるようになります。 一般的なサブフォルダーには、メール、ランディングページ、スマートキャンペーン、リスト、レポートなどが含まれます。

**プログラム内のフォルダー名**
* キャンペーン - *インタラクションとステータストラッキングを管理するすべてのキャンペーン用のフォルダー*
* ローカル Assets - *このプログラムに固有のすべてのアセットのフォルダー*
   * メール
   * ランディングページ
   * スマートキャンペーン
   * リスト - *プログラム固有のリストがある場合にのみ必要です。*
   * Forms - *プログラム固有のFormsがある場合にのみ必要です。ほとんどのFormsはグローバルAssetsです。*
   * レポート - *プログラム固有のレポートがある場合にのみ必要です。*

### 手順 3 - プログラムとアセットの命名規則の作成

ツリーのフォルダー構造を作成したら、プログラムとアセットに一貫した名前を付けます。 これは、命名規則を標準化すると、命名プロセスを内部で拡張するのに役立つ場合です。 次に、検索性を確保するために命名規則を確立するために使用できるコンポーネントを示します。

* プログラムタイプの略語 – メール、コンテンツ、育成、ウェビナーなど。
* カテゴリ – プログラムのタイプ – スタンドアロンメール、ニュースレターなど。
* 日付 – プログラムの開始日
* 簡単な説明 – プログラムの簡単な説明

次に、値を式に入力し、様々なプログラムタイプのプログラム名を生成します。

#### プログラム命名規則

| **プログラムの種類の略称** | **YYYY** | **\-** | **MM** | **\-** | **DD （オプション）** | **カテゴリ** | **\-** | **プログラムの簡単な説明** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| EM - メール送信（メールプログラム） | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの概要 |
| NL - ニュースレター | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの概要 |
| ENG - エンゲージメントプログラム | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの概要 |
| WBN - ウェビナー | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの概要 |
| IW - インタラクティブウェビナー | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの概要 |
| TS - トレードショー | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの概要 |
| LE - ライブイベント（ロードショー） | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの概要 |
| UG - User Group | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの概要 |
| WC:Web サイト・コンテンツ | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの概要 |
| CS - コンテンツシンジケーション | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの概要 |
| LI - リスト インポート | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの概要 |
| OA - オンラインAdvertising | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの概要 |
| PPC - クリック課金 | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの概要 |

| **例** |
| --- |
| ES 2023-10 Gated Content - XYX ホワイトペーパー |
| WC-2023-10 – 月次ウェビナー – ABC 導入事例 |

#### アセットの命名規則

アセットの命名まで 1 レベル下げると、プログラム名を繰り返さず、今後のクローン作成の使用のために短い識別子と汎用識別子を使用することをお勧めします。 次の点に注意してください。

* プログラムプロセスでの順序に基づいてアセットに番号を付けます。
* 命名コンポーネントを「。」ではなく「–」（ハイフン）を使用して区切ります。（ドット）または「\_」（アンダースコア）。
   * なぜでしょうか。 Marketo Engageでは、プログラム名とキャンペーン名を区切るためにドットを使用します。 アセットにハイパーリンクが設定されている場合、「\_」を使用すると、表示されなくなります。
* アセット名に標準の頭字語を使用して参照を短縮し、引き続き認識しやすくします。

これらを念頭に置いて、これらのヒントを次のアセットに適用し、名前を生成する式を作成します。

##### プログラムプロセスのシーケンスに基づいてアセットに名前を付ける

| **プログラムプロセスのシーケンス** | **\-** | **説明** |
| --- | --- | --- |
| 01 | \- | 説明 |
| 02 | \- | 説明 |
| 03 | \- | 説明 |

| **例：スマートリスト** |
| --- |
| 01 - メールを送信 |
| 02 – 開封済み |
| 03 – クリック |
| 04 入力済みフォーム |
| 05 – 影響（プログラム成功） |
| 06 – 購読解除 |

##### アセットにアセットタイプの略語で名前を付ける

| **資産の種類の略称** | **アセットタイプ** | **\-** | **目標の説明** |
| --- | --- | --- | --- |
| LP - ランディングページ | LP | \- | 目標の説明 |
| メール – メール（アウトバウンド） | EMAIL | \- | 目標の説明 |
| アラート – メールアラート | アラート | \- | 目標の説明 |
| WF - Web フォーム | WF | \- | 目標の説明 |
| EXCL – 除外リスト | 除く | \- | 目標の説明 |
| SLST - スマート・リスト | SLST | \- | 目標の説明 |
| LST – 静的リスト | LST | \- | 目標の説明 |

| **例** |
| --- |
| LP-Registration |
| LP-ThankYou |
| E メール – 送信 |
| メールニュースレター |
| EMAIL-Invitation |
| EMAIL-Reminder |
| EXCL-Competitors |

##### ダウンロード可能なファイル（.pdf）にアセットタイプの略称を付けます

| **アセットタイプ** | **コンテンツの説明** | **\-** | **資産の種類の略称** | **.** | **PDF** |
| --- | --- | --- | --- | --- | --- |
| WP – 白紙 | コンテンツの説明 | \- | WP | 。 | pdf |
| CS – 導入事例 | コンテンツの説明 | \- | CS | 。 | pdf |
| DS - データシート | コンテンツの説明 | \- | DS | 。 | pdf |

| **例：ダウンロード可能なPDFファイル** |
| --- |
| XYZ-Gadget-DS.pdf |
| Acme-Company-CS.pdf |
| How-XYZ-Gadgets-make-life-easier-WP.pdf |

>[!CAUTION]
>
>上記の例でファイルに名前を付ける場合は、スペースを使用せず、アンダースコア「\_」を使用しないでください

## 次の手順

* Marketo Engageー構造と命名規則の作成をサポートするために、[Folder Organization and Naming Conventions](./assets/adobe-marketo-engage-organization-and-naming-conventions.xlsx){target="_blank"} をダウンロードします。
* 標準の命名規則で必要なコンポーネントを決定したら、Google Sheet またはMicrosoft Excel に式を構築することを検討してください。 今後の使用のために、スプレッドシートに値を入力するだけでプログラム名を生成できます。
* フォルダー構造全体に合わせたら、最も頻繁な使用例と、チームが受け取る最も一般的なリクエストに基づいて、必要なテンプレートを検討します。 次に、最初のプログラムテンプレートの作成を開始します。 以下では、[Adobe Marketo Engage プログラムテンプレート ](https://business.adobe.com/blog/how-to/get-started-with-marketo-engage-program-templates){target="_blank"} の基本を学びます。

### 作成者

{{natalie-kremer}}

{{amy-chiu}}
