---
title: CRM 同期エラーをログに記録してトラブルシューティングを容易にします
description: CRM 同期エラーのログを使用して CRM 同期の問題を調査し、スムーズに実行させる方法を説明します。
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
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# CRM 同期エラーをログに記録してトラブルシューティングを容易にします

As a [!DNL Marketo Engage] 管理者。インスタンスが CRM と同期しているかどうかを確認することが、 [日課](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508){target="_blank"}. While the [Notifications section](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html){target="_blank"} ( ページの右上隅にある [!DNL Marketo Engage] インターフェイス ) は、頻繁な同期の問題を見つけて調査する場所です。インスタンスの正常性を整理的に管理するのに役立つヒントがあります。 [!DNL Adobe] Marketoチャンピオン (2019-2022)、Amy Goldfine は、トラブルシューティングを容易にするために、管理者ユーザーに CRM 同期エラーのログを保持することをお勧めします。

![「同期エラー」タブのスクリーンショット](/help/marketo-tutorial-inherited-instance/_assets/Marketo_Engage_Admin_Salesforce_Sync_Errors_Tab.png)

## CRM 同期エラーの記録を保持する理由

CRM 同期エラーをログに記録して、 [!DNL Marketo Engage] 管理者は、CRM 管理者に問題やトレンドを確認して、根本原因を修正できます。 インスタンスの CRM 同期の問題を文書化するには、以下の手順に従います。

## CRM 同期エラーのログを保持する方法

開始する前に、 [CRM 同期エラーログテンプレート](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe-Marketo-Engage_CRM-Sync-Error-Log-Template.xlsx).

**手順 1:** 次に移動： *[!UICONTROL 管理者] セクション* in [!DNL Marketo Engage]. の下 *[!UICONTROL 統合]*&#x200B;をクリックし、 *[!DNL Salesforce]*, *[!DNL Microsoft Dynamics]*&#x200B;または *[!DNL Veeva]*( [!DNL CRM] を使用し、 *[!UICONTROL 同期エラー]* タブをクリックします。

**手順 2:** 次の項目を選択できます。 [エラーのレコードを [!DNL CSV] ～を通してファイルを送る [!UICONTROL フィルター] パネル](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.html#filter-sync-errors){target="_blank"}. 数時間しかない場合は、 *[!UICONTROL 同期エラー]* タブを使用すると便利です。

**手順 3:** エラーが発生した日付をメモしておきます。

**手順 4:** そのエラーの影響を受ける人物レコードの数を入力します。 ( 場合によっては、CRM で 1 人のユーザーに対してのみエラーが発生することがあります。 同時に同じエラーを持つ人が多くいることもあります )。

**手順 5:** エラーの影響を受ける 1 人の人物の E メールアドレスをメモします。 これにより、CRM 管理者と簡単に参照して、エラーについて話し合うことができます。

**手順 6:** [!DNL] 内の人物レコードへのリンクを貼り付け [!DNL Marketo Engage]] および [!UICONTROL CRM リード/連絡先] その人物の記録。

**手順 7:** 最後の列に、エラーの実際のテキストを貼り付けます。

## 次の手順

**エラーコードの特定：** エラーコードを理解するには、開発者向けドキュメントの説明を参照してください [応答レベルのエラーコードの表](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes){target="_blank"} エラーを解決するための典型的な次の手順を見つけます。

## 作成者

**Amy Goldfine**\
[!DNL Adobe] Marketoチャンピオン (2019-2022)
*創業者、 MarketingOpsAdvice.com*

![Amy Goldfine](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**エイミーチウ**
*導入およびリテンションマーケティングマネージャ ( )[!DNL Adobe]*

![エイミーチウ](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}
