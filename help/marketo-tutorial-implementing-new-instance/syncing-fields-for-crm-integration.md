---
title: ネイティブ CRM コネクタのフィールドの同期
description: Marketo Engageで使用する重要なCRM フィールドを戦略的に選択することで、最初のCRM統合を効率化する方法を説明します。 スムーズなCRM同期に必要なフィールドを特定し、営業部門とマーケティング部門の連携を強化するのに役立ちます。
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-04T00:00:00Z
jira: KT-14811
thumbnail: KT-14811.jpeg
exl-id: 42b7ca3d-e445-4c11-ad3d-d4e70c101c8e
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '2235'
ht-degree: 0%

---

# ネイティブ CRM コネクタのフィールドの同期

組織内でSalesforceまたはMicrosoft Dynamicsを使用していますか？ その場合、Marketo Engageのネイティブ CRM コネクタ（Salesforce、Microsoft Dynamics、Veeva）を使用すると、Marketo EngageとCRM間で関連情報をシームレスに共有することで、マーケティング活動と営業活動を連携させることができます。 初期CRM同期を設定する前に、Marketo Engage データベースをクリーンに保つために、2つのシステム間で同期するフィールドを特定してください。

Adobe Professional Servicesが提案するベストプラクティスを使用して、この演習を実施する方法について詳しくは、こちらを参照してください。 標準フィールドとカスタムフィールドについて理解し、Adobe Marketo EngageとCRMの連携を文書化します。

## CRMとMarketo Engageを連携する前に、同期するフィールドを決めておきましょう

CRMとMarketo Engageを統合する場合、あらゆるCRM フィールドをMarketo Engageに同期する必要がない可能性があります。 必要なフィールドについて戦略的に判断することで、Marketo Engageインスタンスがより効率的にデータフローを処理できるようになります。

Adobe Marketo EngageとCRMを初回に同期することで、既存の標準フィールド（電子メール、名/姓、会社など）の多くを自動的に関連付けることができます。 さらに、コネクタは、CRMからこれらのフィールドに自動的にマッピングされる新しいフィールドをMarketo Engageに作成することで、リード、取引先責任者、アカウント、商談の[&#x200B; カスタムフィールド &#x200B;](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"}も同期します。

最初の同期を実行する前に、CRMから同期するフィールドを特定して整理することは、Native Connectorのセットアッププロセスにおける重要なステップです。 これはデータ要素の演習と呼ばれ、作成される重複フィールドの数を最小限に抑え、その後のリマッピングステップをできるだけスムーズに実行するのに役立ちます。 通常、この演習では、マーケティング部門と営業部門およびCRM管理者から情報を収集し、関連するフィールドのみがMarketo Engage インスタンスに同期されるようにします。

## データディクショナリの構築

一般的に、ベストプラクティスは、マーケティング目的で必要となるCRM フィールドのみを同期することです。 Marketo Engageにマッピングする必要があるCRMのフィールドを整理し、最初のCRM同期を正しく実行するには、この演習から始めます。

>[!NOTE]
>最初の同期を開始する前に、既にMarketo Engageに同等のカスタムフィールドがあるCRMのカスタムフィールドがある場合、CRM フィールドの新しい「重複」フィールドがMarketo Engageに作成されます。 最初の同期が完了すると、CRM フィールドを元のMarketo Engage フィールドに再マッピングし、重複するフィールドを非表示にできますが、そうするには、[Adobe カスタマーサポート &#x200B;](https://experienceleague.adobe.com/ja/docs/customer-one/using/home#create-a-support-ticket-with-admin-console){target="_blank"}にお問い合わせください。 詳しくは、手順7を参照してください。

**手順1:** CRMで現在使用可能なフィールドのリストを作成し、それらをMarketo Engageに表示するかどうかをマークします。

* CRM管理者、マーケティング部門、営業部門からのフィードバックを意思決定プロセスに組み込みましょう。
* 各フィールドのAPI名とフィールドタイプを文書化します
* これらのフィールド（読み取り専用または読み取り/書き込み）に対して、Marketo Engageがどのレベルのアクセス権を持つかを決定します


**手順2:** Marketo Engage インスタンスの[管理者/ フィールド管理セクション &#x200B;](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/field-management/view-field-mappings-between-marketo-and-salesforce){target="_blank"}を確認して、同期に含めるシステム内で以前に直接作成したカスタムフィールドを特定します。

* 各フィールドのAPI名とフィールドタイプを文書化します。
* CRMに同等のフィールドが既にあるフィールドを示します。
* CRMに同等のフィールドがないフィールドを示します。


**手順3:** デフォルトのマップフィールドを使用してデータ要素の構築を開始する

* Marketo Engageではフラットデータベースを使用するので、データディクショナリのフォーマットを次のように設定することをお勧めします。

   * 最初の列：Marketo Engage フィールド名
   * 2列目：Marketo Engage API名
   * 3番目の列：[Marketo Engage フィールドの種類](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} （ブール値、通貨、日付など）
   * 後続の列では、CRM オブジェクトタイプ（リード、取引先責任者、アカウント、商談）に対して、Marketo Engageに付与するアクセス権レベル（読み取り、書き込み、編集）の列を追加して、これを繰り返します
  <br>

  その例を次に示します。
  ![&#x200B; データ辞書テーブル &#x200B;](/help/marketo-tutorial-implementing-new-instance/assets/data_dictionary.png){width="100%" zoomable="yes"}


* まず、CRMに自動的にマッピングされるデフォルトフィールドを追加します。

   * [Salesforce](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/default-salesforce-field-mapping){target="_blank"}
   * [Microsoft Dynamics](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/default-dynamics-field-mapping){target="_blank"}
   * [Veeva](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping){target="_blank"}

* Marketo Engageの各デフォルトフィールドが、同期するCRMのフィールドと一致することを確認します。 例えば、Marketo Engageの「購読解除」フィールドは、CRMの「電子メールオプトアウト」フィールドである可能性があります。
* 必要に応じて、CRM APIの名前、権限、および[&#x200B; データタイプ &#x200B;](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"}を調整します。

**手順4:** データ要素に追加フィールドを追加する

* 各フィールドの表示名、目的のCRM権限、データタイプを含めます。
* フィールドがCRMに存在するが、Marketo Engageには存在しない場合は、Marketo Engageの表示名とAPI名をCRM フィールドから同じ値で入力します。
* フィールドがMarketo Engageに存在するがCRMに存在しない場合は、フィールドが作成されるまで、CRM表示名を目的の値で入力しますが、CRM API名は空白のままにします。
* 両方のシステムに同等のフィールドが存在する場合は、同じ行にそれらを含め、データ要素シートの右端にある「メモ」セクションで再マッピングする必要があることを示します。

>[!NOTE]
>同期フィルターフィールド （[Salesforce](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"} | [Microsoft Dynamics](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/custom-dynamics-sync-filter-details/create-a-custom-dynamics-sync-filter){target="_blank"}）を作成する場合は、必ずこの手順に含めますが、フィールドがCRMに作成されるまで、API名は空白のままにします。

**手順5:** CRM管理者とのデータ辞書のレビュー

* Marketo Engageに既に存在するフィールドのフィールドをCRMに作成し、新しいCRM フィールドの表示名とAPI名でデータディクショナリを更新します。
* CRM （[Microsoft Dynamics](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"} | [Salesforce](https://community.dynamics.com/blogs/post/?postid=8a91d93e-2181-45dd-a8fb-1092010bc8f1){target="_blank"}）のリード オブジェクトと取引先責任者オブジェクト間でフィールドマッピングを実行します。 リードが連絡先に変換されると、フィールドをMarketo Engageの1つのフィールドに統合できるようになります。
* Marketo Sync Profileが、データディクショナリに記載されているように、各フィールドに対する適切な権限を持っていることを確認します。
   * [Salesforceでプロファイル権限を設定](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited#set-profile-permissions){target="_blank"}
   * [Microsoft Dynamicsでプロファイル権限を設定する](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up#create-application-user-in-microsoft){target="_blank"}
   * [Veevaでプロファイル権限を設定](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage#set-profile-permissions){target="_blank"}

**手順6:**&#x200B;最初の同期を実行

* Marketo Engageと同期するすべてのフィールドに、データディクショナリで定義されているCRM内の適切な権限があることを確認します。
* Marketo Engageと同期するフィールドのうち&#x200B;**not**&#x200B;が[Marketo Sync Profile](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync){target="_blank"}から非表示になっていることを確認します。 意図せず同期されたフィールドを削除するよりも、新しいフィールドを同期に追加する方がはるかに簡単です。
* CRMを「同期フィルター」フィールドに接続していますか？ Salesforceに同期する場合は、最初の同期を開始する前に、Adobe カスタマーサポートに連絡して、フィルター機能がオンになっていることを確認してください。


**手順7:** Marketo Engageのフィールド管理セクションを確認する

* 新しい同期フィールドの表示とAPI名を確認または更新します。
* 再マッピングが必要な可能性のある重複フィールドを特定します。 フィールドの重複は、次のような場合に発生します。
   * CRMのカスタムフィールドは、同等のフィールドが既にMarketo Engageに存在する場合、Marketo Engageで初めて同期したときに、新しい（重複する可能性がある）フィールドを作成します。
   * Marketo-Engage専用のカスタムフィールド（つまり、Marketo Engageで直接作成されたフィールド）と、CRMから同期された同等のフィールドがある場合があります。



**手順8:**&#x200B;重複したフィールドが表示された場合は、Adobe カスタマーサポートに連絡して再マッピングを実行してください

* 再マッピングが必要なフィールドについては、次の情報をサポートに問い合わせてください。
   * CRMによって作成された新しい重複フィールドの表示とAPI名。
   * CRM フィールドをマッピングするMarketo Engage フィールドの表示名。
   * この例[HERE](https://nation.marketo.com/t5/knowledgebase/re-mapping-sfdc-marketo-fields/ta-p/299284){target="_blank"}を参照してください。
* 再マッピングが完了したら、Marketo Engageで再マッピングされたフィールドのAPI名を確認し、データディクショナリの「API名」列の値を更新して、最も正確な情報が含まれていることを確認します。

## 次の手順

* CRM統合用のフィールドを整理するためのデータ要素を構築します。
* CRMの初期同期プロセスの概要

>[!BEGINTABS]

>[!TAB Salesforce]

Adobe Marketo EngageとSalesforceを連携させることで、どのようにセールスとマーケティングのデータを同期させることができるのかをご確認ください。

>[!VIDEO](https://video.tv.adobe.com/v/3453797/?captions=jpn&learn=on)

+++**ビデオで使用されているリンク：**

* [Salesforce Syncについて](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync){target="_blank"}

* [SalesforceへのMarketo フィールドの追加（Enterprise/Unlimited）](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited){target="_blank"}

* [SalesforceでのMarketo ユーザーの作成（Enterprise/Unlimited）](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited){target="_blank"}

* [MarketoとSalesforceの連携（Enterprise/Unlimited）](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited){target="_blank"}

* [ユーザーは、MarketoとSalesforce Syncに進む前に、Salesforce側でコネクテッドアプリを設定する必要があります。](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0){target="_blank"}

* [Salesforce Sync ステータス](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-status){target="_blank"}

* [フィールドの非表示と再表示](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/field-management/hide-and-unhide-a-field){target="_blank"}

* [チュートリアル：MarketoのCRMへの同期について説明します](https://experienceleague.adobe.com/ja/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn){target="_blank"}

+++

>[!TAB Microsoft Dynamics]

Microsoft Dynamics 365 syncの仕組みを説明し、設定を適切に設定して、2つのシステムが互いに話し合えるようにします。

>[!VIDEO](https://video.tv.adobe.com/v/3430209/?captions=jpn&learn=on)

+++**ビデオで使用されているリンク：**

* [Microsoft Dynamics Syncについて](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/understanding-the-microsoft-dynamics-sync){target="_blank"}

* [Marketo リード管理ソリューションのダウンロード](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/download-the-marketo-lead-management-solution){target="_blank"}

* [Microsoft Dynamics用Marketo ソリューションのアップデート](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/update-the-marketo-solution-for-microsoft-dynamics){target="_blank"}

* [クライアント IDとアプリ登録に対する同意の付与](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/grant-consent-for-client-id-and-app-registration)

* [Microsoft Dynamics Syncの検証](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/validate-microsoft-dynamics-sync){target="_blank"}

* [同期ステータス](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/sync-status){target="_blank"}

* [Dynamics検証同期の問題の修正](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/fix-dynamics-validation-sync-issues){target="_blank"}

* [カスタム Dynamics Sync フィルターの作成](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/custom-dynamics-sync-filter-details/create-a-custom-dynamics-sync-filter.html?lang=ja){target="_blank"}

* [組織サービス URLの表示](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/view-the-organization-service-url){target="_blank"}

* [Dynamicsでフィールドを削除する前に同期するフィールドの編集](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/editing-fields-to-sync-before-deleting-them-in-dynamics){target="_blank"}

* [チュートリアル：MarketoのCRMへの同期について説明します](https://experienceleague.adobe.com/ja/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn){target="_blank"}

+++

>[!ENDTABS]

### 制作者

{{peter-livadas}}

{{amy-chiu}}
