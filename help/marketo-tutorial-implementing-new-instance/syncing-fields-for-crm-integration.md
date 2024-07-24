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
source-git-commit: 195a1211b8b191032f4d37662b5beee9a0a54de4
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# ネイティブ CRM コネクタ用のフィールドの同期

組織内で Salesforce またはMicrosoft Dynamics を使用していますか？ その場合、Marketo Engageのネイティブ CRM コネクタ（Salesforce、Microsoft Dynamics、Veeva）を使用すると、Marketo Engageと CRM の間で関連情報をシームレスに共有することで、マーケティングとセールスアクティビティを調整できます。 最初の CRM 同期を設定する前に、Marketo Engageデータベースをクリーンな状態に保つために、2 つのシステム間で同期させるフィールドを特定してください。

Adobe Professional Servicesが推奨するベストプラクティスを使用して、この演習を実施する方法について詳しく説明します。 沿って進んで標準フィールドとカスタムフィールドを理解し、Marketo Engageと CRM の間の関係を文書化します。

## CRM をMarketo Engageと統合する前に同期するフィールドを特定する

CRM をMarketo Engageと統合する場合、すべての CRM フィールドをMarketo Engageと同期する必要はありません。 必要なフィールドに関する戦略を立てると、Marketo Engageインスタンスがデータフローをより効率的に処理するのに役立ちます。

Marketo Engageと CRM システムの間の初期同期により、既存のほとんどの標準フィールド（メール、姓/名、会社など）に対して自動的に関連付けが行われます。 また、CRM の [ カスタムフィールド ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} に自動的にマッピングされる新しいフィールドをMarketo Engageに作成することで、リード、連絡先、アカウント、商談の（カスタムフィールド）も同期されます。

初期同期を実行する前に CRM から同期したいフィールドを特定して整理することは、ネイティブコネクタのセットアッププロセスにおいて重要な手順です。 これをデータ要素の演習と呼びます。この演習では、作成される重複フィールドの数を最小限に抑え、後続の再マッピング手順をできるだけスムーズに行うことができます。 この演習には、通常、マーケティングチームやセールスチーム、CRM 管理者からの入力が含まれ、関連するフィールドのみがMarketo Engageインスタンスに同期されるようにします。

## データ要素の作成方法

通常、ベストプラクティスは、マーケティング目的で必要になる CRM フィールドのみを同期することです。 この演習から始めて、Marketo Engageにマッピングする必要がある CRM のフィールドを整理し、最初の CRM 同期を初めて正しく実行します。

>[!NOTE]
>最初の同期を開始する前に、Marketo Engageに同等のカスタムフィールドが既に存在する CRM にカスタムフィールドがある場合、CRM フィールドのMarketo Engageに新しい「重複」フィールドが作成されます。 最初の同期が完了したら、CRM フィールドを元のMarketo Engageフィールドに再マッピングし、重複フィールドを非表示にすることができますが、その場合は [Adobeカスタマーサポート ](https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console){target="_blank"} にお問い合わせください。 詳しくは、手順 7 を参照してください。

**手順 1:** CRM で現在使用可能なフィールドの大まかなリストを作成し、Marketo Engageに表示するかどうかをマークします。

* CRM 管理者、マーケティングチーム、セールスチームからのフィードバックを意思決定プロセスに含めます。
* 各フィールドの API 名とフィールドタイプのドキュメント化
* Marketo Engageがこれらのフィールドに対してどのレベルのアクセス権を持つかを指定します（読み取り専用または読み取り/書き込み）


**手順 2:** 同期インスタンスの [ 管理者/フィールド管理 ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/view-field-mappings-between-marketo-and-salesforce){target="_blank"} セクションを確認して、Marketo Engageに含める、システムで直接作成されたカスタムフィールドを特定します。

* 各フィールドの API 名とフィールドタイプを文書化します。
* CRM で同等のフィールドが既に存在するフィールドを示します。
* CRM に同等のフィールドがまだないフィールドを示します。


**手順 3:** デフォルトのマップフィールドを使用したデータディクショナリの作成の開始

* Marketo Engageではフラット・データベースを使用するので、データ・ディクショナリを次のようにフォーマットすることをお薦めします。

   * 最初の列：Marketo Engageフィールド名
   * 2 番目の列：Marketo EngageAPI 名
   * 3 番目の列：[Marketo Engageフィールドの種類 ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} （ブール値、通貨、日付など）
   * 後続の列では、CRM オブジェクトタイプ（リード、連絡先、アカウント、オポチュニティ）で繰り返し、Marketo Engageに付与したいアクセスのレベル（読み取り、書き込み、編集など）で列を追加します
  <br>

  次のサンプルをご覧ください。
  ![ データディクショナリテーブル ](/help/marketo-tutorial-implementing-new-instance/assets/data_dictionary.png){width="100%" zoomable="yes"}


* まず、CRM 用に自動的にマッピングされるデフォルトのフィールドを追加します。

   * [Salesforce](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/default-salesforce-field-mapping){target="_blank"}
   * [Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/default-dynamics-field-mapping){target="_blank"}
   * [ ヴィーヴァ ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping){target="_blank"}

* Marketo Engageの各デフォルトのフィールドが、同期したい CRM のフィールドと一致することを確認します。 例えば、Marketo Engageの「購読解除」フィールドは、CRM の「メールオプトアウト」フィールドになります。
* 必要に応じて、CRM API の名前、権限、[ データタイプ ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} を調整します。

**手順 4:** データディクショナリへのフィールドの追加

* 各フィールドには、表示名、目的の CRM 権限およびデータタイプを含めます。
* CRM にフィールドが存在するがMarketo Engageには存在しない場合は、Marketo Engageの表示と API 名に、CRM フィールドの同じ値を入力します。
* Marketo Engageにフィールドが存在し、CRM に存在しない場合は、CRM 表示名に目的の値を入力しますが、フィールドが作成されるまで CRM API 名は空白のままにします。
* 両方のシステムに同等のフィールドが存在する場合は、それらを同じ行に含め、データ要素シートの右端にある「メモ」セクションで再マッピングする必要があることを示します。

>[!NOTE]
>同期フィルターフィールドの作成を計画している場合（[Salesforce](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"} | [Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/custom-dynamics-sync-filter-details/create-a-custom-dynamics-sync-filter){target="_blank"}）のフィールドを作成する前に、このステップに必ず含めてください。CRM でフィールドを作成するまでは、API 名は空白のままにします。

**手順 5:** CRM 管理者とデータ要素を確認する

* CRM でMarketo Engageに既に存在するフィールド用に新しいフィールドを作成し、新しい CRM フィールドの表示名と API 名でデータディクショナリを更新します。
* CRM 内のリードおよび連絡先オブジェクト間でフィールドマッピングを実行する（[Salesforce](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"} | [Microsoft Dynamics](https://community.dynamics.com/blogs/post/?postid=8a91d93e-2181-45dd-a8fb-1092010bc8f1){target="_blank"}）。 リードを連絡先に変換すると、Marketo Engageでこれらのフィールドを 1 つのフィールドに統合できるようになります。
* データディクショナリに記載されているように、Marketo同期プロファイルに各フィールドに対する適切な権限があることを確認します。
   * [Salesforce でのプロファイル権限の設定 ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited#set-profile-permissions){target="_blank"}
   * [Microsoft Dynamics でのプロファイル権限の設定 ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up#create-application-user-in-microsoft){target="_blank"}
   * [Veeva でのプロファイル権限の設定 ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage#set-profile-permissions){target="_blank"}

**手順 6:** 初期同期の実行

* Marketo Engageと同期するすべてのフィールドに、データディクショナリで定義された適切な権限が CRM にあることを確認します。
* Marketo Engageと同期する **ではない** すべてのフィールドが [Marketo同期プロファイルで非表示 ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync){target="_blank"} になっていることを確認します。 意図せずに同期されたフィールドを削除するよりも、後で同期に新しいフィールドを追加する方がはるかに簡単です。
* CRM を「同期フィルター」フィールドに接続していますか？ Salesforce と同期する場合は、初回同期を開始する前に、Adobeカスタマーサポートに連絡してフィルター機能が有効になっていることを確認してください。


**手順 7:** Marketo Engageの「フィールド管理」セクションを確認する

* 新しく同期されたフィールドの表示と API 名を確認/更新します。
* 再マッピングが必要になる可能性のある重複したフィールドを特定します。 重複したフィールドは、次のようなシナリオで発生します。
   * 同等のフィールドが既にMarketo Engageに存在する場合、CRM のカスタムフィールドは、初めて同期されたときに新しい（重複する可能性がある）フィールドをMarketo Engageに作成します。
   * Marketo-Engage-Only カスタムフィールド（つまり、Marketo Engageで直接作成されたフィールド）と、CRM から同期された同等のフィールドがある場合があります。



**手順 8:** 重複したフィールドが表示された場合に再マッピングを実行するには、Adobeカスタマーサポートにお問い合わせください

* 再マッピングが必要なフィールドについては、サポートに次の情報をお問い合わせください。
   * CRM によって作成された新しい重複フィールドの表示と API 名。
   * CRM フィールドのマッピング先となるMarketo Engageフィールドの表示名。
   * この例 [ こちら ](https://nation.marketo.com/t5/knowledgebase/re-mapping-sfdc-marketo-fields/ta-p/299284){target="_blank"} を参照してください。
* 再マッピングが完了したら、Marketo Engageで再マッピングされたフィールドの API 名を確認し、データディクショナリの「API 名」列の値を更新して、最も正確な情報が含まれるようにします。

## 次の手順

* データ要素を作成し、CRM 統合用のフィールドを整理します。
* CRM の初期同期プロセスについて理解します。

>[!BEGINTABS]

>[!TAB Salesforce]

Marketo Engageと Salesforce を連携させて、セールスデータとマーケティングデータを同期させる方法を説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3424719/?learn=on)

+++**ビデオで使用されているリンク：**

* [Salesforce 同期について ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync){target="_blank"}

* [Salesforce へのMarketo フィールドの追加（Enterprise/Unlimited） ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited){target="_blank"}

* [Salesforce でのMarketo ユーザーの作成（Enterprise/Unlimited） ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited){target="_blank"}

* [Marketoと Salesforce の接続（Enterprise/Unlimited） ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited){target="_blank"}

* [ ユーザーは、Marketoおよび Salesforce Sync に進む前に、Salesforce 側で接続済みアプリを設定する必要があります。](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0){target="_blank"}

* [Salesforce 同期ステータス ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-status){target="_blank"}

* [ フィールドの表示/非表示を切り替える ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/hide-and-unhide-a-field){target="_blank"}

* [ チュートリアル：Marketoの CRM への同期について学ぶ ](https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn){target="_blank"}

+++

>[!TAB Microsoft Dynamics]

Microsoft Dynamics 365 の同期の仕組みと、設定を適切に設定して、2 つのシステムが相互に通信できるようにする方法を説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3424737/?learn=on)

+++**ビデオで使用されているリンク：**

* [Microsoft Dynamics Sync について ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/understanding-the-microsoft-dynamics-sync){target="_blank"}

* [Marketo リード管理ソリューションのダウンロード ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/download-the-marketo-lead-management-solution){target="_blank"}

* [Microsoft Dynamics のMarketo ソリューションの更新 ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/update-the-marketo-solution-for-microsoft-dynamics){target="_blank"}

* [ クライアント Id とアプリ登録に対する同意の付与 ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/grant-consent-for-client-id-and-app-registration)

* [Microsoft Dynamics Sync の検証 ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/validate-microsoft-dynamics-sync){target="_blank"}

* [ 同期ステータス ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/sync-status){target="_blank"}

* [Dynamics 検証の同期に関する問題の修正 ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/fix-dynamics-validation-sync-issues){target="_blank"}

* [ カスタム Dynamics Sync フィルターの作成 ](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/custom-dynamics-sync-filter-details/create-a-custom-dynamics-sync-filter.html){target="_blank"}

* [ 組織サービス URL の表示 ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/view-the-organization-service-url){target="_blank"}

* [Dynamics で削除する前に同期するフィールドの編集 ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/editing-fields-to-sync-before-deleting-them-in-dynamics){target="_blank"}

* [ チュートリアル：Marketoの CRM への同期について学ぶ ](https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn){target="_blank"}

+++

>[!ENDTABS]

### 作成者

{{peter-livadas}}

{{amy-chiu}}
