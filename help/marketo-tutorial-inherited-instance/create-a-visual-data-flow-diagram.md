---
title: マーケティングテクニカルスタックを把握するための視覚的なデータフロー図を作成
description: データユニバースを理解し、インスタンスを効率的に監査および整理するための「リードとデータソース」の図を作成する方法について説明します。
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-13877
thumbnail: KT-13877.jpeg
hide: false
exl-id: 088bdcf1-4e49-44a7-ac78-a03742ff680b
source-git-commit: b2e05ff39e065691dda530ed17762a55cf2e6778
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 2%

---

# マーケティングテクニカルスタックを把握するための視覚的なデータフロー図を作成

を引き継ぐ管理者として [!DNL Marketo Engage] 何年も使用されているインスタンスは、インスタンスを効率的に監査および整理することは不可能なミッションのようなものです。 条件 [!DNL Adobe] [!DNL Marketo Champion] （2019）、Kelly Jo Horton は、長年のインスタンスに足を踏み入れ、この課題に取り組みました。 [「リードとデータソース」の図の作成](https://nation.marketo.com/t5/employee-blogs/understand-your-marketing-technology-and-data-create-this/ba-p/296774){target="_blank"} データの世界に慣れるために。 このチュートリアルでは、Kelly Jo Horton が共有した例を基に、独自のデータフロー図を作成する方法を学びます。 MarTech エコシステムについて説明します。

## 継承されたインスタンスのアーキテクチャ図を作成する理由

1. **ライブインスタンスから継承したマーケティングテクニカルスタックについて理解します。** すべてのマーケティング運用管理者/プラットフォーム運用管理者は、新しい会社で始める際にこの演習を行うことをお勧めします。 この作成プロセスにより、管理者ユーザーは、外部統合からに送信されたデータとアクティビティの全体像を確認できます [!DNL Marketo Engage] API エラーのトラブルシューティングを簡単におこなえます。
2. **外部統合を管理する主な関係者について確認します。** Kelly Jo Horton が関係者をすばやく特定するために使用するヒントは、API ユーザーのリストを参照することです。
   1. **「管理者」セクションの「統合/LaunchPoint」タブに移動します。** 「LaunchPoint」タブに移動する方法について詳しくは、以下を参照してください。 [REST API で使用するカスタムサービスの作成](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.html){target="_blank"}.
   2. API 呼び出し情報セクションの統合/「Web サービス」タブで、API ユーザー別の API 使用状況の統計を確認します。 API 呼び出し番号をクリックすると、各ユーザーが実行した特定の個別の呼び出しを表示できます。

## この視覚的なデータフロー図の演習を行う方法

### 手順 1：現在の状態のダイアグラム

「現在の状態」ダイアグラムを作成します。 次に例を示します。

![現在の状態の図](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Current_State_Lead_Data_Sources_KellyJo_Horton.png){align="center"}


### 手順 2：今後の状況を示す図

テクノロジーとシステムのロードマップを技術者以外の関係者に提示する際に使用できる、「将来の状態」図を作成します。 次に例を示します。

![将来の状態の図](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Future-State-Lead-Data-Sources-KellyJo-Horton.png){align="center"}

### 手順 3：テクニカルバージョン

各統合の API ユーザー名、プッシュするデータのタイプの簡単な説明などの詳細を表示するテクニカルバージョンを作成します [!DNL Marketo Engage] または引っ張られる [!DNL Marketo Engage]と、ミドルウェアのフローとトリガーの詳細な図。  次に例を示します。

![技術バージョン](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Lead-Data-Source-Diagram-KellyJo-Horton.png){align="center"}


## 次の手順

**例から開始する：**
サンプルデータフロー図を 1 つダウンロードして、マーケティングテクニカルスタック、ユーザー、データフローの現在の状態をマッピングするか、インスタンスを監査する際にデータユニバースの図を最初から作成します。


<table style="table-layout:fixed">
   <tr>  
      <td style="border: 0;">
      <div style="text-align: center;">
          <a href="./_assets/downloads/Current_Future_State_Lead_Data_Sources.zip">
            <strong>現在の状態と将来の状態</strong>
         </a>
      </div>
      </td>
      <td style="border: 0;">
      <div style="text-align: center;">
         <a href="./_assets/downloads/Detailed_Layers_by_Functional_Category_Stacked_Technologies.zip">
         <strong>機能カテゴリ別の詳細レイヤー </strong>   
         </a>
      </div>
      </td>
      <td style="border: 0;">
         <div style="text-align: center;">
         <a href="./_assets/downloads/Lead_Data_Source.zip">
           <strong>リードとデータソースのフロー </strong>  
         </a>
         </div>
       </td> 
       <td style="border: 0;">
         <div style="text-align: center;">
         <a href="./_assets/downloads/Simple_World_Class_Stage_Stack.zip">
          <strong>簡略化された図</strong>  
         </a>
         </div>
        </td>  
   </tr>
   <tr>
    <td style="border: 0;">
         <div>
          <img alt="現在の状態と将来の状態の図" src="./_assets/Thumbnail_Current-Future State Lead_Data Sources_KellyJo_Horton.png"/>
         </a>
      </div>
      </td>
      <td style="border: 0;">
         <div>
         <a href="./_assets/downloads/Detailed_Layers_by_Functional_Category_Stacked_Technologies.zip">
         <img alt="機能カテゴリ別詳細レイヤー図" src="./_assets/Thumbnail_Detailed_Layers_by_Functional_Category_Stacked_Technologies_KellyJo_Horton.png" />
       </a>
         </div>
      </td>
       <td style="border: 0;">
         <div>
            <a href="./_assets/downloads/Lead_Data_Source.zip">
         <img alt="リードとデータソースのフロー図" src="./_assets/Thumbnail_Lead-Data Source Diagram_KellyJo_Horton.png" />
         </a>
         </div>
      </td>
     <td style="border: 0;">
         <div>
            <a href="./_assets/downloads/Simple_World_Class_Stage_Stack.zip">
             <img alt="簡略化された図" src="./_assets/Thumbnail_Simple_World_Class_Stage_Stack.png" />
         </a>
         </div>
      </td>
</table>

次のツールを使用できます。draw.io （Google ドキュメント）、 [!DNL Adobe] XD、Figma、Gliffy （Confluence）

**アーキテクチャ図がすでに存在する場合はどうなりますか？** 新しいチームメンバーは、異なる視点を持つことができます。 新しいものを持つことには価値がある [!DNL Marketo Engage] 管理者は、オンボーディングプロセスの一環としてこの演習を行い、他のユーザーと共有します。

## 作成者

**ケリージョ ホートン**\
[!DNL Adobe] Marketo チャンピオン （2019）
*Etumos のシニア・クライアント・パートナー*

![ケリージョ ホートン](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Kelly_Jo_Horton.png){width="30%"}

**エイミー・チウ**
*導入およびリテンション・マーケティング・マネージャ[!DNL Adobe]*

（/help/marketo-tutorial-inherited-instance/_assets/authors/[!DNL Adobe]_Author_Amy_Chiu.png） {width=30%}
