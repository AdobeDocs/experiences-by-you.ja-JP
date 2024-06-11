---
title: ドキュメントを含んだインスタンスガバナンスガイドの開発
description: のドキュメントと変更ログを作成および維持するための堅牢な手順を確立する方法を説明します [!DNL Marketo Engage] インスタンス。 これにより、チームの知識の共有に要する時間が節約されるだけでなく、インスタンスの正常性と効率も向上します。
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-14103
thumbnail: KT-14103.jpeg
hide: false
exl-id: e127b84d-ef92-4527-a0e6-a36af35b7ee0
source-git-commit: b2e05ff39e065691dda530ed17762a55cf2e6778
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 1%

---

# ドキュメントを含んだインスタンスガバナンスガイドの開発

レガシーに足を踏み入れる場合 [!DNL Marketo Engage] 例えば、最新の機能および技術ドキュメントが不足しているという課題が発生することがよくあります。 管理者として、適切なインスタンスガバナンスを確保するためのガイドラインを確立することは、見過ごすことができない中核的な責任です。 これは～するための重要な戦略の一つである [確立されたで作業する際の効率の向上 [!DNL Marketo Engage] instance](https://nation.marketo.com/t5/champion-program-blogs/3-tips-to-increase-your-efficiency-in-an-inherited-instance/ba-p/247582).

[!DNL をソースにしたこのステップバイステップのチュートリアル [!DNL Adobe] Marketo Champion] （2018）の Nick Hajdin 氏が、このプロセスを通じて、インスタンス設定の概要を説明し、主な運用プログラムを文書化して、 [!DNL changelog] 厳格なガバナンスポリシーを実施する。

## 継承されたインスタンスにインスタンスガバナンスガイドおよびドキュメントを開発する理由

詳細なドキュメントと [!DNL changelog] は、組織内での効率的な管理と知識伝達に不可欠です [!DNL Marketo Engage] インスタンス。 インスタンスの設定中に行った変更や決定を追跡すると、次の利点があります。

1. スケーラブルな方法で、社内ユーザーのトレーニングを容易に実施できます。
2. ～でより効率的に建設する [!DNL Marketo Engage] 長期的には。
3. メールを詳しく調べる時間を節約するために、今後はインスタンスの正常性と衛生状態を維持します。 [監査記録](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/audit-trail/audit-trail-overview.html)、および [アクティビティログ](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.html) コンテキストを取得します。
4. 転送時の時間の節約 [!DNL Marketo Engage] 新しいことに対する知識 [!DNL Marketo Engage] 管理者（チームに離職率が発生した場合）

## [!DNL Marketo Engage] ガバナンスガイド 101

ガバナンスガイドは、インスタンス設定およびシステム設計要件の情報源として機能します。 このドキュメントに含めることをお勧めする主な情報は次のとおりです。

* プログラム/フォルダー構造
* ユーザーと役割の権限
* 通信の制限
* ガバナンス基準
* プラットフォームへのアクセス権を付与する前に行う社内ユーザーのトレーニング

## のガバナンスガイドを開発および維持する方法 [!DNL Marketo Engage] instance

### 手順 1：現在のガバナンスガイドとドキュメントの状態を特定する

* **継承されたインスタンスのドキュメントが見つかりません：** 最近新しい役割を開始し、継承されたインスタンスのドキュメントが見つからない場合は、 **手順 2 に進む** 用意したダウンロード可能なテンプレートの使用を開始します。
* **ファイルのマニュアルがあります。** おめでとうございます、これは良い兆候です！ 最後の変更が行われている時期を確認するには、それらの関連度を確認してください。 チームメンバーが積極的にメンテナンスしていない場合は、チームメンバーを更新し、内部ユーザーに対して最新のメンテナンス方法を教えることをお勧めします。

### 手順 2：に含める要素を特定する [!DNL Marketo Engage] ドキュメントと [!DNL Changelogs]

形式は、クラウドベースのプラットフォームから共有ドキュメントまで様々です。 組織のニーズに合わせて形式をデザインできます。 [シンプルなドキュメントと変更ログの Excel テンプレートを以下に示します](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx) 基本を学べる重要な要素について説明します。 これには、以下が含まれます。

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
   * 変更前のエクスペリエンス（リンク/スクリーンショットを含む）
   * 変更後のエクスペリエンス（リンク/スクリーンショットを含む）
   * プログラムへの URL

### 手順 3：主要な運用プログラムの現在の状態を特定して文書化する

まず、サブスクリプションレベルで影響を受ける主要な運用プログラムを特定します。 例としては、データ管理があります [!DNL Campaign]s、リードライフサイクル、リードスコアリング、 [!DNL CRM] 同期、配信品質。

特定された運用プログラムごとに、その現在の状態をドキュメント化します。 これには、プログラムの目的、設定、関連するスマートキャンペーンおよび他のツールとの統合（該当する場合）に関する詳細が含まれます。

### 手順 4：適用する [!DNL Changelog] 保守

次のステップは、の厳格なガバナンスポリシーを確立することです [!DNL Marketo Engage] を必要とするインスタンス[!DNL Changelog] メンテナンス。」 このポリシーにより、インスタンス全体で運用プログラムに対して行われた更新が完全にドキュメント化されます。

これらのドキュメントの重要性と、ドキュメントに適切にアクセスして更新する方法について、チームを教育します。 変更ログを維持する責任を割り当てると便利です。そのため、少数の専任のマーケティング運用チームメンバーまたは管理者が、変更を継続的に記録し、承認を提供します。

### 手順 5：ドキュメントを一元化

に関連するすべてのドキュメントを一元的に保存する場所またはリポジトリを確立します。 [!DNL Marketo Engage] インスタンス。 これは、共有ドライブ、専用フォルダー、クラウドベースのシステムのいずれかです。

### 手順 6：定期的なレビューと更新

ドキュメントを正確かつ最新の状態に保つために、ドキュメントの定期的なレビューをスケジュールします。 それは忙しい時間の間に簡単に見過ごすことができます。 プロアクティブにカレンダーにリマインダーを設定して、運用プログラムの変更や最適化を反映するためにチームが定期的に更新を行うようにします。

## 次の手順

これをダウンロードして開始する [シンプルなテンプレート](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx).

上記の手順に従って、ガバナンスガイドとドキュメントを作成します。 プロセスを進める際は、次の経験則に留意してください。

**既存のドキュメントを更新します。**
ドキュメントを最新の状態に保つことが重要です。 過去 3 年間変更されていない場合は、インスタンスを監査する際にドキュメントを修正する時間を確保します。

**共有とトレーニング：**
ドキュメントの共有と [!DNL changelog] と関連するチームメンバーを対象に、これらのレコードの更新方法を説明します。

**定期的な確認：** 新しい変更、最適化、調整が発生した場合に、それらを 1 年を通じて確認および維持するためのスケジュール時間。

包括的な最新ドキュメントの維持 [!DNL Marketo Engage] インスタンスを使用すると、長期的に時間と労力を節約でき、効果的なインスタンス管理が容易になります。

### 作成者

**ニック・ハジン**
[!DNL [!DNL Adobe] Marketoチャンピオン】 （2018 年）
*[!DNL Digital Technology Senior Manager at Accenture]*

![ニック・ハジン](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Nicholas_Hajdin.png){width="30%"}

**エイミー・チウ**
*導入およびリテンション・マーケティング・マネージャ[!DNL Adobe]*

![エイミー・チウ](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width=30%}
