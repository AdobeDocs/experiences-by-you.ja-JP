---
title: マーケター向けトラブルシューティング
description: 最も一般的なエラーを把握することで、問題をより迅速に解決し、生産性を高めることができます。 これらのトラブルシューティングヒントは、同様のエラーが発生した場合に効果的に解決するのに役立ちます。
solution: Campaign Standard
feature-set: Campaign
feature: Workflows
role: User
level: Beginner, Intermediate, Experienced
doc-type: Article
last-substantial-update: 2023-05-18T00:00:00Z
jira: KT-13256
thumbnail: KT-13256.jpeg
exl-id: 24a6815b-52d1-4bd6-9d27-522720a91f83
source-git-commit: 35e62c4f1a093b4f755e175e9b553a43887e4292
workflow-type: tm+mt
source-wordcount: '722'
ht-degree: 5%

---

# マーケター向けのトラブルシューティング：ワークフローと配信に関する 5 つの一般的なエラー

基準： [スラジ・パトラ](https://www.linkedin.com/in/suraj-p-51612053/){target="_blank"}（メイジェール・シニア・コンサルタント）

シニアエンジニアおよび顧客エキスパートとして： [!DNL Adobe] 過去 5 年間のExperience Cloud製品を、 [メイジェール](https://www.meijer.com/){target="_blank"}:1934 年に設立されたアメリカのスーパーセンターチェーンで、ACS と共に複雑なマーケティングキャンペーンとトランザクションキャンペーンを展開しています。 私が取り組んだいくつかのプロジェクトには、と統合され、パーソナライゼーションのオファーと注文の詳細を保存するカスタマイズされたキャンペーンが含まれています。 [!DNL Adobe] Audience Manager、およびセグメント取り込みに関する顧客インサイト。


ACS を使用している間にエラーが発生しました。このエラーは、解決に時間がかかり、面倒になる場合があります。 最も一般的なエラーを把握することで、問題をより迅速に解決し、生産性を高めることができます。 以下に、同様のエラーが発生した場合に効果的に解決するのに役立つトラブルシューティングのヒントを示します。

## データタイプ不一致エラー

**エラーコード:**
`PGS-220000 PostgreSQL error: ERROR: operator does not exist: character varying = bigint`

**原因：**
これらのタイプのエラーは、異なるデータタイプのフィールドを使用して紐付けを試みると、ワークフローに表示されます。 例えば、文字列フィールドを持つ load file を使用してファイルをアップロードする場合、string フィールドを、データ型が int のプロファイルフィールドに紐付けしようとします。

![data-type-mismatch-error](/help/_assets/kt-13256/data-type-mismatch.png)

**解決策：**
「ファイルを読み込み」アクティビティのフィールドのデータタイプを、一致するデータタイプに変更します。 「ファイル読み込み」アクティビティを開きます。 「COLUMN DEFINITION」タブに移動し、目的のフィールドのデータ型を変更します。


![data-type-mismatch-solution](/help/_assets/kt-13256/data-type-mismatch-solution.png)

## 配信のパーソナライゼーションエラー

**エラーコード:**
`The schema for profiles specified in the transition ('') is not compatible with the schema defined in the delivery template ('nms:recipient'). They should be identical.`

**原因：**
このエラーは、電子メールをアドレスに送信する際に表示されますが、電子メールまたはその他の識別子は、プロファイルと紐付けされていません。 E メール通信を送信するには、E メールまたは識別子を常にプロファイルにリンクする必要があります。

![紐付けアクティビティを含むワークフロー](/help/_assets/kt-13256/del-persn-error-wf.png)

**解決策：**
共通 ID は、読み込まれたファイルと受信者テーブルから取得したものである必要があります。 この共通キーは、紐付けアクティビティ内で読み込みファイルを受信者テーブルに結合します。 ワークフロー内でこの紐付け手順が必要な受信者テーブルに存在しないレコードには、E メールが送信されない場合があります。 その際、「受信読み込みファイル」アクティビティを、プロファイルからの電子メール ID などの識別子に紐付けします。 The `nms:recipient` スキーマはプロファイルテーブルを参照し、受信レコードをプロファイルに紐付けすることで、e メールの準備中に使用できるようになります。

以下に示す紐付けアクティビティのスクリーンショットを参照してください。

![紐付けの詳細を含むワークフロー](/help/_assets/kt-13256/del-persn-error-wf-solution.png)

詳細情報： [紐づけ](https://experienceleague.adobe.com/docs/campaign-standard/using/managing-processes-and-data/data-management-activities/reconciliation.html?lang=en).

## 共通フィールドデータセットエラー

**エラーコード:**
`The document types of inbound events (''and'') are incompatible (step 'Exclusion'). Unable to perform the operation. `

**原因：**
この問題は、 **除外アクティビティ** ACS ワークフローでは、ID に基づいて除外を実行する際に、プライマリセットと除外セットに同じフィールド名がない場合に発生します。


![共通フィールドデータセットエラー](/help/_assets/kt-13256/dataset-error.png)

**ソリューション:**

このエラーを解決する方法は 2 つあります。

1. プライマリと除外の両方で同じフィールド名を使用し、そのフィールドを ID として使用します

   または

2. JOINS 除外メソッドを使用して、レコードを除外するフィールドを選択します。

![一般的なフィールドデータセットエラー — ソリューション ](/help/_assets/kt-13256/dataset-error-solution.png)

## フィールド名ドロップエラー

**エラーコード:**
`XTK-170036 Unable to parse expression 'i__name'`

**原因**：:

エラーポイントは、 **エンリッチメント活性**. 最も一般的な例を以下に示します。

![フィールド名ドロップエラー](/help/_assets/kt-13256/field-name-dropped-error.png)

これは、アクティビティの式の名前を手動で編集した場合に発生します。 この図は、式が次の場所から変更されたことを示しています： `name `から `i__name`.

**ソリューション:**

このエラーは、次の 3 つの方法で解決できます。

1. 名前を元の式に戻します。

2. 新しい名前を使用する場合は、 **エンリッチメント活性**.

3. 何が変更されたかを覚えていない場合は、アクティビティを再作成することをお勧めします。

## 一時テーブルの削除エラー 

**エラーコード:**
`XTK-170024 The temporary schema "temp:deliveryEmail1" is not defined in the current context.`

**原因：**
これは、エンリッチメントやその他のアクティビティが関わる複雑なワークフローで発生する一般的なエラーです。 ワークフローに対する複数の変更中に、一部のアクティビティワークフローが正しく保存されない可能性があります。

![一時テーブルの削除エラー ](/help/_assets/kt-13256/temp-table-dropped-error.png)

**解決策：**
このエラーは多くの方法で発生する可能性があるので、簡単な修正はありません。 単純なワークフローの場合は、アクティビティを再設定する方が効果的です。 複雑なワークフローでは、ワークフローアクティビティを新しいワークフローにコピーし、保存して再実行する方が効果的です。
