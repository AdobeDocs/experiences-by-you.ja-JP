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
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# CRM 同期エラーをトラブルシューティング用にログ記録

[!DNL Marketo Engage] 管理者は、インスタンスが CRM と同期しているかどうかを確認することが、「毎日のルーチン [ の重要な部分になるはず ](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508){target="_blank"} す。 [ 通知 ](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html?lang=ja){target="_blank"} セクション（[!DNL Marketo Engage] インターフェイスの右上隅にあります）では頻繁な同期の問題を見つけて調査しますが、インスタンスのヘルスを組織的に管理するのに役立つヒントが用意されています。 Marketo Champion （2019-2022）の [!DNL Adobe]、管理者ユーザーは、トラブルシューティングを容易にするために、CRM 同期エラーのログを保持することをお勧めします。

![ 「同期エラー」タブのスクリーンショット ](/help/marketo-tutorial-inherited-instance/_assets/Marketo_Engage_Admin_Salesforce_Sync_Errors_Tab.png)

## CRM 同期エラーを記録するのはなぜですか？

管理者は、CRM 同期エラーをログに記録 [!DNL Marketo Engage] ることで、CRM 管理者と問題やトレンドをレビューし、根本原因を修正することができます。 次の手順に従って、インスタンスの CRM 同期の問題を文書化します。

## CRM 同期エラーのログを保持する方法

開始する前に、[CRM 同期エラーログテンプレート ](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe-Marketo-Engage_CRM-Sync-Error-Log-Template.xlsx) をダウンロードしてください。

**手順 1:** [!DNL Marketo Engage] の *[!UICONTROL 管理者 &#x200B;] セクション* に移動します。 *[!UICONTROL 統合]* の下で、使用する [!DNL CRM] に応じて「*[!DNL Salesforce]*」、「*[!DNL Microsoft Dynamics]*」、または「*[!DNL Veeva]*」をクリックし、「*[!UICONTROL 同期エラー]*」タブをクリックします。

**手順 2:** [ フィルター ] パネルを使用して、エラーのレコードを  [!DNL CSV]  ファイルとしてエクスポート [[!UICONTROL &#x200B; することを選択できます &#x200B;]](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.html?lang=ja#filter-sync-errors){target="_blank"}。 数時間しかない場合は、「同期エラー *[!UICONTROL タブから直接コピーして貼り付け]* 方法をお勧めします。

**手順 3:** エラーが発生した日付をメモします。

**手順 4:** このエラーの影響を受ける人物レコードの数を入力します。 （CRM で 1 人のユーザーに対してのみエラーがスローされる場合があります。 同じエラーを一度に抱える人が多い場合があります）。

**手順 5:** エラーの影響を受けた 1 人の人物のメールアドレスをメモします。 これにより、エラーを簡単に参照して CRM 管理者と話し合うことができます。

**手順 6:** [!DNL Marketo Engage] 内の人物レコードへのリンクを貼り付け、その人物の [!UICONTROL CRM リード/連絡先 &#x200B;] レコードを貼り付けます。

**手順 7:** 最後の列に、エラーの実際のテキストを貼り付けます。

## 次の手順

**エラーコードの特定：** エラーコードを理解するには、開発者向けドキュメント [ 応答レベルのエラーコードの表 ](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes){target="_blank"} の説明を調べ、エラーを解決するための一般的な次の手順を見つけます。

## 作成者

**エイミー・ゴールドファイン**\
[!DNL Adobe] Marketo チャンピオン（2019 年～2022 年）
*創業者、MarketingOpsAdvice.com*

![ エイミー・ゴールドファイン ](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**エイミー・チウ**
*[!DNL Adobe]* の導入およびリテンション・マーケティング・マネージャ

![ エイミー・チウ ](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}
