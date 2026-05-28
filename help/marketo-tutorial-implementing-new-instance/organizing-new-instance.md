---
title: 新しいインスタンスの整理と命名規則の確立
description: Marketo Engageインスタンス内で優れた組織を設定し、組織内の将来のマーケターがプログラムを簡単にナビゲートし、アセットを変更し、レポートを取得できるようにする方法を説明します。
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-03T00:00:00Z
jira: KT-14813
thumbnail: KT-14813.jpeg
exl-id: 19b3de9e-53f3-4308-b46e-7b8f756c30a0
source-git-commit: cae626cb3958ebcda16ac30b0a487ebfe06d50f4
workflow-type: tm+mt
source-wordcount: '1291'
ht-degree: 2%

---

# 新しいインスタンスを整理し、命名規則を確立する

新しいMarketo Engageインスタンスを導入する管理者は、組織内の将来のマーケターがインスタンスを容易に移動できる基盤を構築する必要があります。 ツリーフォルダーの構造と命名規則に慣れることで、インスタンスを整頓し、長期的な成功に備えることができます。 このチュートリアルでは、AdobeとMarketo Engage Champion （2019-2020）が推奨する例を取り上げて、フォルダーとアセット名を一貫して[整理できるよう支援します](https://nation.marketo.com/t5/champion-program-blogs/keep-marketo-engage-organized-with-folders-and-naming/ba-p/245630){target="_blank"}。

## フォルダーを構造化し、命名規則を適用する必要があるのはなぜですか？

インスタンスを整理することで、キャンペーン、プログラム、アセットを追跡し、プログラムのパフォーマンスを報告することが容易になります。 インスタンス内のナビゲーションツリーを整理して大規模に構築するには、[&#x200B; フォルダー](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-folders){target="_blank"}、[標準の命名規則](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs#naming-schemes){target="_blank"}、[複製](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs#cloning){target="_blank"}などの機能を使用することをお勧めします。

## Marketo Engage インスタンスを整理する方法

>[!VIDEO](https://video.tv.adobe.com/v/3421577/?quality=12&learn=on)

### 手順1 - プログラムを順番に配置するためのフォルダー構造の設定

インスタンスを整理するための最初のステップは、プログラムとアセットを見つけやすく整理された方法で[&#x200B; フォルダー構造](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/create-new-campaign-folder.html)に設定することです。

以下に、ツリー内のフォルダーを構造化する際の簡単なヒントを示します。

* 見つけやすいようにフラットなフォルダー構造を維持。
* 組織のチーム構造（地域やチームなど）や取り組み（ニュースレターなど）を反映させるためにフォルダーを構成します。
* 時間ベースのラベルを含めることで、検索性を高め、アーカイブに適したタイミングを示すことができます（例：2024）。
   * 管理者は、少なくとも年に1回はフォルダーをアーカイブすることをお勧めします。 年間フォルダー名を使用すると、ライブスマートキャンペーンを簡単に非アクティブ化し、年末にフォルダー全体をアーカイブできます。

以下は、これらのヒントを実践するためのフォルダーの例です。

**ツリー内のフォルダー名**

>[!BEGINTABS]

>[!TAB マーケティングアクティビティ]

![&#x200B; フォルダーのマーケティング活動](/help/marketo-tutorial-implementing-new-instance/assets/folders-marketing-activities.png)

>[!TAB  デザインスタジオ ]

![&#x200B; フォルダーデザインスタジオ &#x200B;](/help/marketo-tutorial-implementing-new-instance/assets/folders-design-studio.png)

>[!TAB データベース]

![&#x200B; フォルダーデータベース &#x200B;](/help/marketo-tutorial-implementing-new-instance/assets/folders-database.png)

>[!ENDTABS]

### 手順2 - プログラム内のフォルダーの作成

次に、プログラムレベルでフォルダー構造を適用します。 ベストプラクティスとして、ローカルアセットをサブフォルダーに格納すると、プログラムを整頓し、内部ユーザーがプログラムを効率的に変更または報告できるようになります。 一般的なサブフォルダーには、メール、ランディングページ、スマートキャンペーン、リスト、レポートなどが含まれます。

プログラム内の&#x200B;**フォルダー名**

* キャンペーン – インタラクションとステータスの追跡を管理しているすべてのキャンペーンの&#x200B;*フォルダー。*
* ローカル Assets – このプログラムに固有のすべてのアセットの&#x200B;*フォルダー。*

   * メール
   * ランディングページ
   * スマートキャンペーン
   * リスト - *プログラム固有のリストがある場合にのみ必要です。*
   * Forms - *プログラム固有のFormsがある場合にのみ必要です。ほとんどのFormsはグローバル Assetsです。*
   * レポート - *プログラム固有のレポートがある場合にのみ必要です。*

### 手順3 - プログラムとアセットの命名規則を作成する

ツリー内にフォルダー構造が用意されたら、プログラムとアセットに一貫した名前を付ける必要があります。 これは、命名規則を標準化することで、社内の命名規則プロセスを拡大するのに役立ちます。 検索性を確保するために命名規則を確立するために使用できるコンポーネントを以下に示します。

* プログラムタイプの略語 – メール、コンテンツ、ナーチャリング、ウェビナーなど
* カテゴリー – プログラムの種類 – スタンドアロンメール、ニュースレターなど。
* 日付 – プログラム開始日
* 簡単な説明 – プログラムについての簡単な説明

次に、値を数式に入れて、さまざまなプログラムタイプのプログラム名を生成します。

#### プログラム命名式

| **プログラムタイプの略語** | **YYYY** | **\-** | **MM** | **\-** | **DD （オプション）** | **カテゴリ** | **\-** | **プログラムの簡単な説明** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| EM - メール送信（メールプログラム） | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの簡単な説明 |
| NL - ニュースレター | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの簡単な説明 |
| ENG - エンゲージメントプログラム | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの簡単な説明 |
| WBN - ウェビナー | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの簡単な説明 |
| IW - インタラクティブウェビナー | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの簡単な説明 |
| TS - トレードショー | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの簡単な説明 |
| LE - ライブイベント（Roadshow） | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの簡単な説明 |
| UG - ユーザーグループ | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの簡単な説明 |
| WC - Web サイトのコンテンツ | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの簡単な説明 |
| CS - コンテンツシンジケーション | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの簡単な説明 |
| LI - リストの読み込み | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの簡単な説明 |
| OA - Online Advertising | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの簡単な説明 |
| PPC - クリック課金 | YYYY | \- | MM | \- | DD （オプション） | カテゴリ | \- | プログラムの簡単な説明 |

| **例** |
| --- |
| ES 2023-10 ゲーテッドコンテンツ - XYX ホワイトペーパー |
| WC-2023-10 – 月次ウェビナー – ABCのユーザー事例 |

#### アセット命名式

アセットの命名に至るまで、プログラム名を繰り返さず、将来のクローン作成に短い汎用識別子を使用することをお勧めします。 ここでは、いくつかの重要なヒントを紹介します。

* プログラムプロセスでの順序に基づいてアセットに番号を付けます。
* 「。」（ドット）または「\_」（アンダースコア）ではなく、「 – 」（ハイフン）を使用して命名規則コンポーネントを区切ります。
   * なぜでしょうか？ Marketo Engageでは、ドットを使用してプログラム名とキャンペーン名を区切ります。 「\_」を使用すると、アセットがハイパーリンクされているときに表示されなくなります。
* アセット名に標準的な頭字語を使用することで、参照を短くし、認識を容易にします。

これらを念頭に置いて、次のヒントを次のアセットに適用し、名前を生成するための数式を作成します。

##### プログラムプロセスのシーケンスに基づいてアセットに名前を付けます

| プログラムプロセスの&#x200B;**シーケンス** | **\-** | **説明** |
| --- | --- | --- |
| 01 | \- | 説明 |
| 02 | \- | 説明 |
| 03 | \- | 説明 |

| **例：スマートリスト** |
| --- |
| 01-Send Email |
| 02-Opened |
| 03 – クリック |
| 04-Filled-out Form |
| 05影響（プログラムの成功） |
| 06 – 登録解除 |

##### アセットタイプの略語を使用してアセットに名前を付けます

| **アセットタイプの略語** | **アセットタイプ** | **\-** | 目標&#x200B;**の**&#x200B;説明 |
| --- | --- | --- | --- |
| LP - ランディングページ | LP | \- | 目標の説明 |
| 電子メール – 電子メール（アウトバウンド） | EMAIL | \- | 目標の説明 |
| アラート – メールアラート | アラート | \- | 目標の説明 |
| WF - Web フォーム | WF | \- | 目標の説明 |
| EXCL – 除外リスト | EXCEL | \- | 目標の説明 |
| SLST - スマートリスト | SLST | \- | 目標の説明 |
| LST – 静的リスト | LST | \- | 目標の説明 |

| **例** |
| --- |
| LP-Registration |
| LP-ThankYou |
| EMAIL-Outbound |
| EMAIL-Newsletter |
| EMAIL-Invitation |
| EMAIL-Reminder |
| EXCL-Competitors |

##### ダウンロード可能なファイル（.pdf）にアセットタイプの省略形を付けます

| **アセットタイプ** | **コンテンツの説明** | **\-** | **アセットタイプの略語** | **.** | **PDF** |
| --- | --- | --- | --- | --- | --- |
| WP - ホワイトペーパー | Content Description | \- | WP | 。 | pdf |
| CS - ケーススタディ | Content Description | \- | CS | 。 | pdf |
| DS - データシート | Content Description | \- | DS | 。 | pdf |

| **例：ダウンロード可能なPDF ファイル** |
| --- |
| XYZ-Gadget-DS.pdf |
| Acme-Company-CS.pdf |
| How-XYZ-Gadgets-make-life-easier-WP.pdf |

>[!CAUTION]
>
>上記の例でファイルに名前を付ける場合は、スペースを使用せず、アンダースコア「\_」の使用を避けてください

## 次の手順

* フォルダー構造と命名規則の作成をサポートするために、ワークシート [Marketo Engageの組織と命名規則](./assets/adobe-marketo-engage-organization-and-naming-conventions.xlsx){target="_blank"}をダウンロードします。
* 標準的な命名規則で必要なコンポーネントを決定したら、数式をGoogle シートまたはMicrosoft Excelに組み込むことを検討してください。 今後の使用のために、スプレッドシートに値を入力するだけで、プログラム名を生成できます。
* 全体的なフォルダー構造を整えたら、最も頻繁に使用するユースケースやチームが受ける最も一般的なリクエストにもとづいて、必要なテンプレートを考える必要があります。 最初のプログラムテンプレートの作成を開始します。 [Adobe Marketo Engage プログラムテンプレート &#x200B;](https://business.adobe.com/blog/how-to/get-started-with-marketo-engage-program-templates){target="_blank"}を使い始めるには、この記事を読んでください。

### 制作者

{{natalie-kremer}}

{{amy-chiu}}
