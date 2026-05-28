---
title: 簡単なトラブルシューティング用のCRM同期エラーのログ
description: CRM同期エラーのログを使用して、CRM同期の問題を調査し、円滑に実行する方法を説明します。
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-13875
thumbnail: KT-13875.jpeg
exl-id: 6a38f5dd-5d25-43d8-a1d3-e75ab396e555
source-git-commit: d78210c6d6f5ec22430770c752495959303a9519
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# トラブルシューティング用のCRM同期エラーのログ

[!DNL Marketo Engage]管理者として、インスタンスがCRMと同期しているかどうかを確認することは、[毎日のルーチン ](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508){target="_blank"}の重要な部分である必要があります。 [通知セクション ](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html){target="_blank"} （[!DNL Marketo Engage] インターフェイスの右上隅にあります）では、頻繁な同期の問題を確認して調査できますが、インスタンスの正常性を整理した方法で管理するのに役立つプロ向けのヒントがあります。[!DNL Adobe] Marketo Champion （2019～2022年）、Amy Goldfineは、管理者ユーザーがトラブルシューティングを容易にするために、CRM Sync エラーのログを保持することを推奨しています。

![同期エラーのタブのスクリーンショット ](/help/marketo-tutorial-inherited-instance/_assets/Marketo_Engage_Admin_Salesforce_Sync_Errors_Tab.png)

## CRM同期エラーの記録を保持する理由

CRM同期エラーをログに記録することで、[!DNL Marketo Engage]管理者はCRM管理者の問題と傾向を確認して、根本原因を修正できます。 以下の手順に従って、インスタンスのCRM同期の問題を文書化します。

## CRM同期エラーのログを保持する方法

開始する前に、[CRM Sync Errors Log テンプレート ](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe-Marketo-Engage_CRM-Sync-Error-Log-Template.xlsx)をダウンロードしてください。

**手順1:** [!DNL Marketo Engage]の&#x200B;*[!UICONTROL 管理者] セクション*&#x200B;に移動します。 *[!UICONTROL 統合]*&#x200B;で、使用している[!DNL CRM]に応じて&#x200B;*[!DNL Salesforce]*、*[!DNL Microsoft Dynamics]*&#x200B;または&#x200B;*[!DNL Veeva]*&#x200B;をクリックし、「*[!UICONTROL 同期エラー]*」タブをクリックします。

**手順2:** [!UICONTROL  フィルター] パネル ](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.html#filter-sync-errors){target="_blank"}を使用して、エラーの記録を [!DNL CSV]  ファイルとして[書き出すことを選択できます。 時間が数時間しかない場合、「*[!UICONTROL 同期エラー]*」タブから直接コピー&amp;ペーストすることをお勧めします。

**手順3:** エラーが発生した日付を記録します。

**手順4:**&#x200B;そのエラーの影響を受ける人物レコードの数を入力します。 （CRMでエラーがスローされるのは、1人の場合だけです。 同じエラーを一度に持つ人が多い場合があります。

**手順5:** エラーの影響を受ける1人のユーザーの電子メールアドレスをメモします。 これにより、CRM管理者がエラーを参照して議論することが容易になります。

**手順6:**&#x200B;その人物の[!DNL Marketo Engage]および[!UICONTROL CRM リード/コンタクト ] レコードの人物レコードにリンクを貼り付けます。

**手順7:**&#x200B;最後の列に、エラーの実際のテキストを貼り付けます。

## 次の手順

**エラーコードの特定：** エラーコードを理解するには、開発者ドキュメント [応答レベルのエラーコード テーブル ](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes){target="_blank"}の説明を参照し、エラーを解決するための一般的な次の手順を見つけます。

## 制作者

**Amy Goldfine**\
[!DNL Adobe] Marketo Champion （2019-2022）
*Founder, MarketingOpsAdvice.com*

![Amy Goldfine](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**Amy Chiu**
*アダプション&amp;リテンションマーケティングマネージャー、[!DNL Adobe]*

![Amy Chiu](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}
