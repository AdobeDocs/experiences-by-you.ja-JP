---
title: ネイティブ CRM コネクタ用のフィールドの同期
description: Marketo Engageで使用する必要のある CRM フィールドを戦略的に選択することで、最初の CRM 統合を効率化する方法を説明します。 データ要素の演習を実施し、CRM をスムーズに同期するために必要なフィールドを特定します。これにより、販売チームとマーケティングチームの連携が維持されます。
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-04T00:00:00Z
jira: KT-14811
thumbnail: KT-14811.jpeg
exl-id: 42b7ca3d-e445-4c11-ad3d-d4e70c101c8e
source-git-commit: bed599454a75159492f13aab1f802c09d92bf7ed
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# ネイティブ CRM コネクタ用のフィールドの同期

組織内で Salesforce またはMicrosoft Dynamics を使用していますか？ その場合、Marketo Engageのネイティブ CRM コネクタ（Salesforce、Microsoft Dynamics、Veeva）を使用すると、Marketo Engageと CRM の間で関連情報をシームレスに共有することで、マーケティングとセールスアクティビティを調整できます。 最初の CRM 同期を設定する前に、Marketo Engageデータベースをクリーンな状態に保つために、2 つのシステム間で同期させるフィールドを特定してください。

Adobe Professional Servicesが推奨するベストプラクティスを使用して、この演習を実施する方法について詳しく説明します。 沿って進んで標準フィールドとカスタムフィールドを理解し、Marketo Engageと CRM の間の関係を文書化します。

## CRM をMarketo Engageと統合する前に同期するフィールドを特定する

CRM をMarketo Engageと統合する場合、すべての CRM フィールドをMarketo Engageと同期する必要はありません。 必要なフィールドに関する戦略を立てると、Marketo Engageインスタンスがデータフローをより効率的に処理するのに役立ちます。

Marketo Engageと CRM システムの間の初期同期により、既存のほとんどの標準フィールド（メール、姓/名、会社など）に対して自動的に関連付けが行われます。 また、コネクタも同期します [カスタムフィールド](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} リード、連絡先、アカウント、オポチュニティに対して、CRM のこれらのフィールドに自動的にマッピングされる新しいフィールドをMarketo Engageで作成します。

初期同期を実行する前に CRM から同期したいフィールドを特定して整理することは、ネイティブコネクタのセットアッププロセスにおいて重要な手順です。 これをデータ要素の演習と呼びます。この演習では、作成される重複フィールドの数を最小限に抑え、後続の再マッピング手順をできるだけスムーズに行うことができます。 この演習には、通常、マーケティングチームやセールスチーム、CRM 管理者からの入力が含まれ、関連するフィールドのみがMarketo Engageインスタンスに同期されるようにします。

## データ要素の作成方法

通常、ベストプラクティスは、マーケティング目的で必要になる CRM フィールドのみを同期することです。 この演習から始めて、Marketo Engageにマッピングする必要がある CRM のフィールドを整理し、最初の CRM 同期を初めて正しく実行します。

>[!NOTE]
>最初の同期を開始する前に、Marketo Engageに同等のカスタムフィールドが既に存在する CRM にカスタムフィールドがある場合、CRM フィールドのMarketo Engageに新しい「重複」フィールドが作成されます。 最初の同期が完了したら、CRM フィールドを元のMarketo Engageフィールドに再マッピングし、重複したフィールドを非表示にすることができますが、連絡が必要になります [Adobeカスタマーサポート](https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console){target="_blank"} を作成してください。 詳しくは、手順 7 を参照してください。

**手順 1:** CRM で現在使用可能なフィールドの大まかなリストを作成し、Marketo Engageに表示するかどうかをマークします。

* CRM 管理者、マーケティングチーム、セールスチームからのフィードバックを意思決定プロセスに含めます。
* 各フィールドの API 名とフィールドタイプのドキュメント化
* Marketo Engageがこれらのフィールドに対してどのレベルのアクセス権を持つかを指定します（読み取り専用または読み取り/書き込み）


**手順 2:** をレビュー [管理者/「フィールド管理」セクション](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/view-field-mappings-between-marketo-and-salesforce){target="_blank"} :Marketo Engageに含める、システムで以前直接作成されたカスタムフィールドを識別します。

* 各フィールドの API 名とフィールドタイプを文書化します。
* CRM で同等のフィールドが既に存在するフィールドを示します。
* CRM に同等のフィールドがまだないフィールドを示します。


**手順 3:** デフォルトのマップフィールドを使用してデータディクショナリの作成を開始

* Marketo Engageではフラット・データベースを使用するので、データ・ディクショナリを次のようにフォーマットすることをお薦めします。

   * 最初の列：Marketo Engageフィールド名
   * 2 番目の列：Marketo EngageAPI 名
   * 3 列目： [Marketo Engageフィールドタイプ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} （ブール値、通貨、日付など）
   * 後続の列では、CRM オブジェクトタイプ（リード、連絡先、アカウント、オポチュニティ）で繰り返し、Marketo Engageに付与したいアクセスのレベル（読み取り、書き込み、編集など）で列を追加します
  <br>

  次のサンプルをご覧ください。
  ![データディクショナリテーブル](/help/marketo-tutorial-implementing-new-instance/assets/data_dictionary.png){width="100%" zoomable="yes"}


* まず、CRM 用に自動的にマッピングされるデフォルトのフィールドを追加します。

   * [Salesforce](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/default-salesforce-field-mapping){target="_blank"}
   * [Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/default-dynamics-field-mapping){target="_blank"}
   * [ヴェーヴァ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping){target="_blank"}

* Marketo Engageの各デフォルトのフィールドが、同期したい CRM のフィールドと一致することを確認します。 例えば、Marketo Engageの「購読解除」フィールドは、CRM の「メールオプトアウト」フィールドになります。
* CRM API の名前、権限、 [データタイプ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} 必要に応じて、

**手順 4:** データ要素へのフィールドの追加

* 各フィールドには、表示名、目的の CRM 権限およびデータタイプを含めます。
* CRM にフィールドが存在するがMarketo Engageには存在しない場合は、Marketo Engageの表示と API 名に、CRM フィールドの同じ値を入力します。
* Marketo Engageにフィールドが存在し、CRM に存在しない場合は、CRM 表示名に目的の値を入力しますが、フィールドが作成されるまで CRM API 名は空白のままにします。
* 両方のシステムで同等のフィールドが存在する場合は、それらを同じ行に含め、データ要素シートの右端にある「メモ」セクションで再マッピングする必要があることを示します。

>[!NOTE]
>同期フィルターフィールド（[Salesforce](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"} | [Microsoft Dynamics](https://community.dynamics.com/blogs/post/?postid=8a91d93e-2181-45dd-a8fb-1092010bc8f1){target="_blank"}）、この手順では必ず含めてください。ただし、CRM でフィールドを作成するまでは、API 名は空白のままにします。

**手順 5:** CRM 管理者とデータ要素を確認する

* CRM でMarketo Engageに既に存在するフィールド用に新しいフィールドを作成し、新しい CRM フィールドの表示名と API 名でデータディクショナリを更新します。
* CRM のリードおよび連絡先オブジェクト間のフィールドマッピングの実行（[Salesforce](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"} | [Microsoft Dynamics](https://community.dynamics.com/blogs/post/?postid=8a91d93e-2181-45dd-a8fb-1092010bc8f1){target="_blank"}）に設定します。 リードが連絡先に変換されると、これらのフィールドをMarketo Engage内の 1 つのフィールドに確実に統合できます。
* データディクショナリに記載されているように、Marketo同期プロファイルに各フィールドに対する適切な権限があることを確認します。
   * [Salesforce でのプロファイル権限の設定](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited#set-profile-permissions){target="_blank"}
   * [Microsoft Dynamics でのプロファイル権限の設定](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up#create-application-user-in-microsoft){target="_blank"}
   * [Veeva でのプロファイル権限の設定](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up#create-application-user-in-microsoft){target="_blank"}

**手順 6:** 初期同期の実行

* Marketo Engageと同期するすべてのフィールドに、データディクショナリで定義された適切な権限が CRM にあることを確認します。
* すべてのフィールドを選択するようにしてください  ***ではない*** Marketo Engageと同期するは次のとおりです [Marketo同期プロファイルで非表示](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync){target="_blank"}. 意図せずに同期されたフィールドを削除するよりも、後で同期に新しいフィールドを追加する方がはるかに簡単です。
* CRM を「同期フィルター」フィールドに接続していますか？ Salesforce と同期する場合は、最初の同期を開始する前に、Adobeカスタマーサポートに連絡して、フィルター機能がオンになっていることを確認します。


**手順 7:** Marketo Engageの「フィールド管理」セクションを確認します。

* 新しく同期されたフィールドの表示と API 名を確認/更新します。
* 再マッピングが必要になる可能性のある重複したフィールドを特定します。 重複したフィールドは、次のようなシナリオで発生します。
   * 同等のフィールドが既にMarketo Engageに存在する場合、CRM のカスタムフィールドは、初めて同期されたときに新しい（重複する可能性がある）フィールドをMarketo Engageに作成します。
   * Marketo-Engage-Only カスタムフィールド（つまり、Marketo Engageで直接作成されたフィールド）と、CRM から同期された同等のフィールドがある場合があります。



**手順 8:** 重複したフィールドが表示された場合、再マッピングを実行するには、Adobeカスタマーサポートにお問い合わせください

* 再マッピングが必要なフィールドについては、サポートに次の情報をお問い合わせください。
   * CRM によって作成された新しい重複フィールドの表示と API 名。
   * CRM フィールドのマッピング先となるMarketo Engageフィールドの表示名。
   * この例を参照してください。 [こちら](https://nation.marketo.com/t5/knowledgebase/re-mapping-sfdc-marketo-fields/ta-p/299284){target="_blank"}.
* 再マッピングが完了したら、Marketo Engageで再マッピングされたフィールドの API 名を確認し、データディクショナリの「API 名」列の値を更新して、最も正確な情報が含まれるようにします。

## 次の手順

* データ要素を作成し、CRM 統合用のフィールドを整理します。
* CRM の初期同期プロセスについて理解します。

>[!BEGINTABS]

>[!TAB Salesforce]

Marketo Engageと Salesforce を連携させて、セールスデータとマーケティングデータを同期させる方法を説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3424719/?learn=on)

+++**ビデオで使用されているリンク：**

* [Salesforce 同期について](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.html){target="_blank"}

* [Salesforce へのMarketo フィールドの追加（Enterprise/Unlimited）](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.html){target="_blank"}

* [Salesforce でのMarketo ユーザーの作成（Enterprise/Unlimited）](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.html){target="_blank"}

* [Marketoと Salesforce の接続（Enterprise/Unlimited）](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.html){target="_blank"}

* [ユーザーは、Marketoおよび Salesforce Sync に進む前に、Salesforce 側で接続済みアプリを設定する必要があります。](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.html){target="_blank"}

* [Salesforce 同期ステータス](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-status.html){target="_blank"}

* [フィールドの非表示と表示](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/hide-and-unhide-a-field.html){target="_blank"}

* [チュートリアル：Marketoの CRM への同期について](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn.html){target="_blank"}

+++

>[!TAB Microsoft Dynamics]

Microsoft Dynamics 365 の同期の仕組みと、設定を適切に設定して、2 つのシステムが相互に通信できるようにする方法を説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3424737/?learn=on)

+++**ビデオで使用されているリンク：**

* [Microsoft Dynamics Sync について](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/understanding-the-microsoft-dynamics-sync.html){target="_blank"}

* [Marketo Lead Management Solution のダウンロード](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/download-the-marketo-lead-management-solution.html){target="_blank"}

* [Microsoft Dynamics 用のMarketo ソリューションの更新](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.html){target="_blank"}

* [クライアント Id とアプリ登録に同意する](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/grant-consent-for-client-id-and-app-registration.html)

* [Microsoft Dynamics Sync の検証](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/validate-microsoft-dynamics-sync.html){target="_blank"}

* [同期ステータス](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/sync-status.html){target="_blank"}

* [Dynamics 検証同期の問題を修正](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/fix-dynamics-validation-sync-issues.html){target="_blank"}

* [カスタム Dynamics Sync フィルターの作成](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/custom-dynmaics-sync-filter-details/create-a-custom-dynamics-sync-filter.html){target="_blank"}

* [組織サービスの URL を表示](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/view-the-organization-service-url.html){target="_blank"}

* [Dynamics で削除する前に同期するフィールドの編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/editing-fields-to-sync-before-deleting-them-in-dynamics.html){target="_blank"}

* [チュートリアル：Marketoの CRM への同期について](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn.html){target="_blank"}

+++

>[!ENDTABS]

### 作成者

{{peter-livadas}}

{{amy-chiu}}

