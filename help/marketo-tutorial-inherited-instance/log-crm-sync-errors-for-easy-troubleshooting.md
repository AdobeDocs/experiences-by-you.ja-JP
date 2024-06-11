---
title: CRM 同期エラーをログに記録して、トラブルシューティングを容易にする
description: CRM 同期エラーのログを使用して、CRM 同期の問題を調査し、スムーズに実行する方法を説明します。
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-13875
thumbnail: KT-13875.jpeg
hide: false
exl-id: 6a38f5dd-5d25-43d8-a1d3-e75ab396e555
source-git-commit: b2e05ff39e065691dda530ed17762a55cf2e6778
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# CRM 同期エラーをログに記録して、トラブルシューティングを容易にする

As a [!DNL Marketo Engage] 管理者は、インスタンスが CRM と同期されているかどうかを確認することが、 [日課](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508){target="_blank"}. 一方、は [通知セクション](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html){target="_blank"} （の右上隅で見つけることができます [!DNL Marketo Engage] インターフェイス）を使用すると、頻繁に同期する問題を見つけて調査できます。インスタンスの正常性を組織的に管理するのに役立つヒントが得られます。 [!DNL Adobe] Marketo Champion （2019-2022）、Amy Goldfine は、トラブルシューティングを容易にするために、管理者ユーザーに CRM 同期エラーのログを保持することをお勧めします。

![「同期エラー」タブのスクリーンショット](/help/marketo-tutorial-inherited-instance/_assets/Marketo_Engage_Admin_Salesforce_Sync_Errors_Tab.png)

## CRM 同期エラーを記録するのはなぜですか？

CRM 同期エラーをログに記録する方法 [!DNL Marketo Engage] 管理者は、問題やトレンドを CRM 管理者とレビューして、根本原因を修正することができます。 次の手順に従って、インスタンスの CRM 同期の問題を文書化します。

## CRM 同期エラーのログを保持する方法

開始する前に、をダウンロードしてください [CRM 同期エラーログテンプレート](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe-Marketo-Engage_CRM-Sync-Error-Log-Template.xlsx).

**手順 1:** に移動します *[!UICONTROL Admin] セクション* 。対象： [!DNL Marketo Engage]. 次の下 *[!UICONTROL 統合]*&#x200B;を選択し、 *[!DNL Salesforce]*, *[!DNL Microsoft Dynamics]*、または *[!DNL Veeva]*&#x200B;以下の条件によって異なります [!DNL CRM] を使用する場合は、 *[!UICONTROL 同期エラー]* タブ。

**手順 2:** 次のいずれかを選択できます。 [エラーのレコードをとしてエクスポート [!DNL CSV] 経由でのファイル [!UICONTROL フィルター] panel](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.html#filter-sync-errors){target="_blank"}. 数時間しかない場合は、から直接コピー&amp;ペーストします。 *[!UICONTROL 同期エラー]* tab キーを押すと移動します。

**手順 3:** エラーが発生した日付をメモしておきます。

**手順 4:** そのエラーの影響を受ける人物レコードの数を入力します。 （CRM で 1 人のユーザーに対してのみエラーがスローされる場合があります。 同じエラーを一度に抱える人が多い場合があります）。

**手順 5:** エラーの影響を受ける 1 人のメールアドレスをメモします。 これにより、エラーを簡単に参照して CRM 管理者と話し合うことができます。

**手順 6:** 人物レコードへのリンクをに貼り付けます [!DNL Marketo Engage] および [!UICONTROL CRM リード/連絡先] その人物の記録。

**手順 7:** 最後の列に、エラーの実際のテキストを貼り付けます。

## 次の手順

**エラーコードの特定：** エラーコードを理解するには、開発者向けドキュメントで説明を参照してください [応答レベルのエラーコード テーブル](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes){target="_blank"} そして、エラーを解決するための一般的な次の手順を見つけます。

## 作成者

**エイミー・ゴールドファイン**\
[!DNL Adobe] Marketo チャンピオン（2019 年～2022 年）
*創設者，MarketingOpsAdvice.com*

![エイミー・ゴールドファイン](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**エイミー・チウ**
*の採用とリテンションのマーケティングマネージャー[!DNL Adobe]*

![エイミー・チウ](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}
