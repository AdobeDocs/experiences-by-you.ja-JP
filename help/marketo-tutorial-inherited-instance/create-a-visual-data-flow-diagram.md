---
title: データフロー図を作成し、マーケティングテクノロジースタックを把握する
description: 「リードとデータソース」のダイアグラムを作成してデータのユニバースを理解し、インスタンスを効率的に監査および整理する方法を説明します。
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-13877
thumbnail: KT-13877.jpeg
exl-id: 088bdcf1-4e49-44a7-ac78-a03742ff680b
source-git-commit: d78210c6d6f5ec22430770c752495959303a9519
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 1%

---

# データフロー図を作成し、マーケティングテクノロジースタックを把握する

何年も前から稼働している[!DNL Marketo Engage] インスタンスを引き継ぐ管理者として、インスタンスを効率的に監査して整頓することは不可能な使命です。 [!DNL Adobe] [!DNL Marketo Champion] （2019）のKelly Jo Hortonは、長年の実績を持つインスタンスに足を踏み入れたとき、データの世界に慣れるために、[&#x200B; リードとデータソース&quot;](https://nation.marketo.com/t5/employee-blogs/understand-your-marketing-technology-and-data-create-this/ba-p/296774){target="_blank"}の図を作成することでこの課題に取り組みました。 このチュートリアルでは、Kelly Jo Hortonが共有した例を基に、独自のデータフロー図を作成する方法を説明します。 マーテクエコシステムの実際を知る！

## 継承したインスタンスのアーキテクチャ図を作成する理由

1. **ライブインスタンスから継承したマーケティングテクノロジースタックを理解します。** すべてのマーケティングオペレーションマネージャー/プラットフォームオペレーションマネージャーは、新しい会社を始める際にこの演習を行うことが推奨されます。 この作成プロセスにより、管理者ユーザーは、外部統合から[!DNL Marketo Engage]に送信されたデータとアクティビティの全体像を確認し、API エラーを簡単にトラブルシューティングできます。
2. **外部統合を管理する主要な関係者を理解します。** Kelly Jo Hortonが関係者をすばやく特定するために使用するヒントは、API ユーザーリストを参照することです。
   1. **管理者セクションの「統合>LaunchPoint」タブに移動します。** 「LaunchPoint」タブに移動する方法の詳細：[REST APIで使用するカスタムサービスを作成](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.html?lang=ja){target="_blank"}。
   2. API呼び出し情報セクションの統合/Web サービス タブで、API ユーザーによるAPI使用統計を検索します。 API呼び出し番号をクリックすると、各ユーザーが行った特定の個々の呼び出しを表示できます。

## この視覚的なデータフロー図の作成方法

### 手順1：現在の状態の図

「現在の状態」図を作成します。 次に例を示します。

![現在の状態図](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Current_State_Lead_Data_Sources_KellyJo_Horton.png){align="center"}


### ステップ 2：未来図

技術やシステムのロードマップを技術者以外の関係者に提示する際に使用できる「将来の状態」図を作成します。 次に例を示します。

![未来状態図](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Future-State-Lead-Data-Sources-KellyJo-Horton.png){align="center"}

### 手順3：技術バージョン

各統合のAPI ユーザー名、プッシュ先[!DNL Marketo Engage]または[!DNL Marketo Engage]から取得するデータのタイプの簡単な説明、ミドルウェアフローとトリガーの詳細な図などの詳細を示すテクニカルバージョンを作成します。次に例を示します。

![技術バージョン &#x200B;](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Lead-Data-Source-Diagram-KellyJo-Horton.png){align="center"}


## 次の手順

**例を使用する：**
サンプルデータフロー図のいずれかをダウンロードして、マーケティングテクノロジースタックの現在の状態、個人とデータフローをマッピングしたり、インスタンスを監査する際にデータ宇宙の図をゼロから作成したりします。


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
         <strong>機能別の詳細なレイヤー</strong>   
         </a>
      </div>
      </td>
      <td style="border: 0;">
         <div style="text-align: center;">
         <a href="./_assets/downloads/Lead_Data_Source.zip">
           <strong> リードとデータ Source フロー</strong>  
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
          <img alt="現状と未来の状況ダイアグラム" src="./_assets/Thumbnail_Current-Future State Lead_Data Sources_KellyJo_Horton.png"/>
         </a>
      </div>
      </td>
      <td style="border: 0;">
         <div>
         <a href="./_assets/downloads/Detailed_Layers_by_Functional_Category_Stacked_Technologies.zip">
         <img alt="機能別の詳細なレイヤーのカテゴリ図" src="./_assets/Thumbnail_Detailed_Layers_by_Functional_Category_Stacked_Technologies_KellyJo_Horton.png" />
       </a>
         </div>
      </td>
       <td style="border: 0;">
         <div>
            <a href="./_assets/downloads/Lead_Data_Source.zip">
         <img alt="リードとデータSourceのフロー図" src="./_assets/Thumbnail_Lead-Data Source Diagram_KellyJo_Horton.png" />
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

使用できるツールは次のとおりです。draw.io （Google Docs）、[!DNL Adobe] XD、Figma、Gliffy （Confluence）

**アーキテクチャ図が既に存在する場合はどうなりますか？** 新しいチームメンバーは、さまざまな視点を持つことができます。 新しい[!DNL Marketo Engage]管理者がオンボーディングプロセスの一環としてこの演習を行い、他のユーザーと共有することは価値があります。

## 制作者

**ケリー・ジョー・ホートン**\
[!DNL Adobe] Marketo Champion （2019年）
*Etumosのシニアクライアントパートナー*

![&#x200B; ケリー・ジョー・ホートン &#x200B;](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Kelly_Jo_Horton.png){width="30%"}

**Amy Chiu**
*導入および維持マーケティングマネージャー、[!DNL Adobe]*

![Amy Chiu](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width=30%}
