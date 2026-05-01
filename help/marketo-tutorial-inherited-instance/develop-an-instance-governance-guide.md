---
title: ドキュメントを使用したインスタンスガバナンスガイドの開発
description: ' [!DNL Marketo Engage]  インスタンスのドキュメントと変更履歴を作成および維持するための堅牢な手順を確立する方法について説明します。'
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-14103
thumbnail: KT-14103.jpeg
exl-id: e127b84d-ef92-4527-a0e6-a36af35b7ee0
source-git-commit: d78210c6d6f5ec22430770c752495959303a9519
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 1%

---

# ドキュメントを使用したインスタンスガバナンスガイドの作成

従来の[!DNL Marketo Engage] インスタンスに移行する際、多くの場合、最新の機能ドキュメントや技術ドキュメントが不足するという課題が伴います。 管理者にとって、適切なインスタンスのガバナンスを確保するためのガイドラインを策定することは、見落とすことのできない重要な責任です。 これは、確立された [!DNL Marketo Engage]  インスタンス [&#128279;](https://nation.marketo.com/t5/champion-program-blogs/3-tips-to-increase-your-efficiency-in-an-inherited-instance/ba-p/247582)で作業する際に効率性を向上させるための重要な戦略の1つです。

[!DNL [!DNL Adobe] Marketo Champion] （2018）のNick Hajdinから提供されたこのステップバイステップチュートリアルでは、このプロセスをガイドして、インスタンスの設定の概要、主要な運用プログラムの文書化、厳格なガバナンスポリシーを適用するための[!DNL changelog]のメンテナンスを行います。

## 継承したインスタンスのインスタンスガバナンスガイドを作成する

詳細なドキュメントと[!UICONTROL 変更履歴]は、[!DNL Marketo Engage] インスタンス内での効率的な管理と知識の転送に不可欠です。 インスタンスのセットアップ中に行った変更や決定を追跡することで、次のことが可能になります。

1. 拡張可能な方法で、社内ユーザーをより簡単にトレーニング。
2. [!DNL Marketo Engage]でより効率的に長期的に構築します。
3. 電子メールを掘り下げる時間を節約するために、インスタンスの健全性と健全性を今後も維持します。コンテキストを取得するために、[監査証跡](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/audit-trail/audit-trail-overview.html?lang=ja)、[&#x200B; アクティビティログ &#x200B;](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.html?lang=ja)。
4. チームが離職した場合、[!DNL Marketo Engage]知識を新しい[!DNL Marketo Engage]管理者に転送する際の時間を節約します。

## [!DNL Marketo Engage] ガバナンスガイド 101

ガバナンスガイドは、インスタンスの設定とシステム設計要件に関する信頼できる唯一の情報源として機能します。 このドキュメントに含めることをお勧めする重要な情報は次のとおりです。

* プログラム/フォルダー構造
* ユーザーおよび役割の権限
* 通信の制限
* ガバナンス基準
* プラットフォームへのアクセスを許可する前に、社内ユーザートレーニングを実施する

## [!DNL Marketo Engage] インスタンスのガバナンスガイドを開発および管理する方法

### ステップ 1：ガバナンスの現状を把握するガイドとドキュメント

* **継承したインスタンスのドキュメントが見つかりません：**&#x200B;最近新しい役割を開始し、継承したインスタンスのドキュメントが見つからない場合は、**手順2**&#x200B;に進み、提供したダウンロード可能なテンプレートを使用します。
* **ファイルに関するドキュメントがあります：**&#x200B;おめでとうございます。これは良いサインです。 関連性を確認し、最後の変更がいつ行われるのかを確認してください。 チームメンバーが積極的にメンテナンスしていない場合は、更新して、社内ユーザーに最新の状態を保つ方法を教育することをお勧めします。

### 手順2: [!DNL Marketo Engage] ドキュメントに含める要素を特定し、[!DNL Changelogs]

形式は、クラウドベースのプラットフォームと共有ドキュメントで異なります。 自社のニーズに合ったフォーマットを設計できます。 [簡単なドキュメントと変更履歴のExcel テンプレート &#x200B;](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx)が用意されています。ここでは、最初に使用できる重要な要素について説明します。 これには、以下が含まれます。

* ドキュメント
   * プログラムテンプレート名
   * チャネル
   * 作成日
   * 作成者
   * プログラムの目的
   * ステータス
   * プログラムテンプレートへのリンク
   * メモ
* 変更ログ
   * プログラムテンプレート名
   * 変更日
   * 更新者
   * 更新の目的
   * 変更前のエクスペリエンス（リンクやスクリーンショットを含む）
   * 変更後のエクスペリエンス（リンクやスクリーンショットを含む）
   * プログラムへのURL

### ステップ 3：主要な事業プログラムの現状を特定し、文書化する

まず、購読レベルで影響を与える主要な運用プログラムを特定しましょう。 例としては、データ管理[!DNL Campaign]s、リードライフサイクル、リードスコアリング、[!DNL CRM]同期、配信品質などがあります。

特定した各プログラムについて、その現状を文書化します。 これには、プログラムの目的、設定、関連するスマートキャンペーン、他のツールとの統合に関する詳細が含まれます（該当する場合）。

### 手順4: [!UICONTROL 変更履歴]のメンテナンスを適用する

次の手順は、「[!UICONTROL 変更履歴]」のメンテナンスを義務付ける[!DNL Marketo Engage] インスタンスに対して厳格なガバナンスポリシーを確立することです。 このポリシーにより、インスタンス全体で運用プログラムに加えられた更新を詳細に文書化できます。

そうしたドキュメントの重要性と、適切にアクセスして更新する方法をチームに周知しましょう。 変更ログを管理する責任を割り当てると役に立つ可能性があります。そのため、いくつかのマーケティング業務チームのメンバーや管理者が、変更を一貫して記録し、サインオフを提供しています。

### 手順5：ドキュメントの一元管理

[!DNL Marketo Engage] インスタンスに関連するすべてのドキュメントを保存するための一元的な場所またはリポジトリを確立します。 これには、共有ドライブ、専用フォルダー、クラウドベースのシステムなどがあります。

### 手順6：確認と更新

ドキュメントの定期的なレビューをスケジュールして、正確かつ最新の状態を保つようにします。 忙しい時には簡単に見落とす事ができます。 カレンダーにリマインダーを積極的に設定し、業務プログラムの変更や最適化を反映して、チームが定期的に更新されるようにします。

## 次の手順

この[&#x200B; シンプルなテンプレート &#x200B;](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx)をダウンロードして開始します。

上記の手順に従って、ガバナンスガイドとドキュメントを作成します。 プロセスを進める際には、次の経験則を考慮してください。

**既存のドキュメントを更新します。**
ドキュメントを最新の状態に保つことが重要です。 過去3年間変更されていない場合は、インスタンスを監査する際に、ドキュメントを修正する時間を確保します。

**共有とトレーニング：**
ドキュメントと[!DNL changelog]を関連するチームメンバーと共有し、これらのレコードを更新する方法について教育します。

**定期的レビュー：**&#x200B;新しい変更、最適化、または調整が発生した場合に、年間を通じてそれらをレビューおよび管理する時間を事前に設定します。

お使いの[!DNL Marketo Engage] インスタンスの包括的かつ最新のドキュメントを維持することで、長期的な時間と労力を節約し、効果的なインスタンス管理を促進できます。

### 制作者

**Nick Hajdin**
[!DNL [!DNL Adobe] Marketo Champion] （2018）
*[!DNL Digital Technology Senior Manager at Accenture]*

![Nick Hajdin](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Nicholas_Hajdin.png){width="30%"}

**Amy Chiu**
*導入および維持マーケティングマネージャー、[!DNL Adobe]*

![Amy Chiu](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width=30%}
