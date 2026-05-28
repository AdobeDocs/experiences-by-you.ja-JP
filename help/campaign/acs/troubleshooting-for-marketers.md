---
title: マーケター向けトラブルシューティング
description: 最も一般的なエラーを把握することで、迅速な問題解決と生産性の向上に役立ちます。 これらのトラブルシューティングヒントは、同様のエラーが発生した場合に効果的に解決するのに役立ちます。
solution: Campaign Standard
feature-set: Campaign
feature: Workflows
role: User
level: Beginner, Intermediate, Experienced
doc-type: Article
last-substantial-update: 2023-05-18T00:00:00Z
jira: KT-13256
thumbnail: KT-13256.jpeg
exl-id: 1f27e284-73e3-4f28-988e-51163775eec8
source-git-commit: cae626cb3958ebcda16ac30b0a487ebfe06d50f4
workflow-type: tm+mt
source-wordcount: '740'
ht-degree: 2%

---

# マーケター向けのトラブルシューティング：5つの一般的なワークフローと配信エラー

作成者：[ スライ パトラ ](https://www.linkedin.com/in/suraj-p-51612053/){target="_blank"}、Meijer、シニアコンサルタント

過去5年間、[!DNL Adobe]のExperience Cloud製品に関するシニアエンジニアおよびカスタマーエキスパートとして、1934年に設立されたアメリカのスーパーセンターチェーンである[Meijer](https://www.meijer.com/){target="_blank"}のビジネスユーザーが、ACSで複雑なマーケティングおよびトランザクションキャンペーンを実行できるようにしています。 私が取り組んだプロジェクトには、[!DNL Adobe] Audience Managerと統合されたパーソナライゼーション用のオファーと注文詳細を保存するカスタマイズされたキャンペーンや、セグメント取り込み用のCustomer insightなどがあります。

ACSを使用している間、解決に時間がかかり、フラストレーションが生じる可能性のあるエラーに遭遇しました。 最も一般的なエラーを把握することで、迅速な問題解決と生産性の向上に役立ちます。 以下は、同様のエラーが発生したときに効果的に解決するのに役立つトラブルシューティングのヒントです。

## データタイプの不一致エラー

**エラーコード：**
`PGS-220000 PostgreSQL error: ERROR: operator does not exist: character varying = bigint`

**原因：**
これらのタイプのエラーは、異なるデータタイプのフィールドを使用して調整しようとすると、ワークフローに表示されます。 例えば、文字列フィールドを持つload fileを使用してファイルをアップロードし、その文字列フィールドをデータ型がintのプロファイルフィールドと紐付けようとします。

![data-type-mismatch-error](/help/_assets/kt-13256/data-type-mismatch.png)

**解決策：**
「ファイルを読み込む」アクティビティのフィールドのデータタイプを、一致するデータタイプに変更します。 「ファイルをロード」アクティビティを開きます。 「COLUMN DEFINITION」タブに移動し、目的のフィールドのデータタイプを変更します。


![data-type-mismatch-solution](/help/_assets/kt-13256/data-type-mismatch-solution.png)

## 配信Personalization エラー

**エラーコード：**
`The schema for profiles specified in the transition ('') is not compatible with the schema defined in the delivery template ('nms:recipient'). They should be identical.`

**原因：**
このエラーは、メールアドレスに電子メールを送信しているときに表示されますが、電子メールやその他の識別子がプロファイルと紐付けられていません。 電子メール通信を送信するには、電子メールまたは識別子を常にプロファイルにリンクする必要があります。

![紐付けアクティビティを含むワークフロー](/help/_assets/kt-13256/del-persn-error-wf.png)

**解決策：**
共通IDは、受信者テーブルを含む読み込まれたファイルに存在する必要があります。 この共通キーは、紐付けアクティビティ内の受信者テーブルに読み込みファイルを結合します。 メールは、ワークフロー内のこの紐付け手順を必要とする受信者テーブルに存在しないレコードに送信できません。 これにより、受信する読み込みファイルアクティビティを、プロファイルの電子メール IDなどの識別子と照合します。 `nms:recipient` スキーマはプロファイルテーブルを参照し、受信レコードとプロファイルを照合することで、メール準備中に使用できるようになります。

以下に示すように、紐付けアクティビティのスクリーンショットを参照してください。

![紐付けの詳細を含むワークフロー](/help/_assets/kt-13256/del-persn-error-wf-solution.png)

[紐付け](https://experienceleague.adobe.com/docs/campaign-standard/using/managing-processes-and-data/data-management-activities/reconciliation.html?lang=en)の詳細をご覧ください。

## 共通フィールドデータセットエラー

**エラーコード：**

`The document types of inbound events (''and'') are incompatible (step 'Exclusion'). Unable to perform the operation.`

**原因：**

この問題は、ACS ワークフローで&#x200B;**exclusion アクティビティ**&#x200B;を使用している際に、IDに基づいて除外を実行する際に、プライマリセットと除外セットのフィールド名が同じではない場合に発生します。

![共通フィールドデータセットエラー](/help/_assets/kt-13256/dataset-error.png)

**解決策：**

このエラーを解決するには、次の2つの方法があります。

1. プライマリと除外の両方で同じフィールド名を使用し、そのフィールドをIDとして使用します

   または

2. JOINS除外メソッドを使用して、レコードを除外するフィールドを選択します。

![共通フィールド データセット エラー – 解決策](/help/_assets/kt-13256/dataset-error-solution.png)

## フィールド名がドロップされましたエラー

**エラーコード：**
`XTK-170036 Unable to parse expression 'i__name'`

**原因：**

エラーポイントは、**エンリッチメントアクティビティ**&#x200B;で発生する可能性があります。 最も一般的なものの1つは下に表示されます。

![ フィールド名が削除されましたエラー](/help/_assets/kt-13256/field-name-dropped-error.png)

これは、アクティビティでエクスプレッション名を手動で編集した場合に発生します。 この画像は、式が`name`から`i__name`に変更されたことを示しています。

**解決策：**

このエラーは、次の3つの方法で解決できます。

1. 名前を元の式に戻します。

2. 新しい名前を使用する場合は、**エンリッチメントアクティビティ**&#x200B;の値を変更します。

3. 何が変わったのかを覚えていない場合は、アクティビティを再現することが最善の策です。

## 一時テーブルが削除されたエラー 

**エラーコード：**
`XTK-170024 The temporary schema "temp:deliveryEmail1" is not defined in the current context.`

**原因：**
これは、エンリッチメントやその他のアクティビティを伴う複雑なワークフローでよくあるエラーです。 ワークフローの複数の変更中に、一部のアクティビティワークフローが正しく保存されない可能性があります。

![一時テーブルが削除されましたエラー](/help/_assets/kt-13256/temp-table-dropped-error.png)

**解決策：**
このエラーが発生する可能性がある多くの方法があるので、簡単な修正はありません。 単純なワークフローの場合は、アクティビティを再設定することをお勧めします。 複雑なワークフローでは、ワークフローアクティビティを新しいワークフローにコピーし、保存して再実行することをお勧めします。
