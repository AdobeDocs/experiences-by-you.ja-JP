---
title: 標準化された命名規則の作成
description: 標準化された命名規則は、AA管理UIで有効になっている変数名自体と、ディメンションに渡される値の両方に適用されます。
solution: Analytics
feature-set: Analytics
feature: Implementation Basics
topic: Administration
role: Admin
level: Beginner
doc-type: article
thumbnail: 10531.jpg
kt: 10531
exl-id: 79cec21e-2b52-4e7b-88ad-db137a8cef4e
product_v2:
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
    internal-label: Analytics
feature_v2:
  - id: a421fb65-2c82-457a-921c-28c46b697a39
    internal-label: Analytics basics
subfeature_v2:
  - id: c24fe15a-643a-47bd-8278-5e027df49785
    internal-label: Implementation basics
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 749b293ab38b8ea5a5f72517bd5c3455399137c2
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%
---
# 標準化された命名規則の作成

**WHAT:**&#x200B;標準化された命名規則は、[!DNL Adobe Analytics] （AA）管理UIで有効になっている場合と、ディメンションに渡される値の両方に適用されます。 （例えば、ページ名は変数名として「ページ名（v1）」となり、渡されるページ名の値は統一され、「sitename|homepage」や「sitename|search|searchresults」などの特定の構造/階層に従う必要があります）。

**理由：**&#x200B;命名規則は、すべての要素を統一し、ユーザーがインターフェイスを理解しやすくするための優れた方法です。 最初からこれらを作成し、プラットフォームとコードで適用すると、これらを拡張しやすくなります。

**方法：** インターフェイスとタグ付けドキュメントは、「名前」と「説明」の両方に一致する必要があります。これにより、ユーザーはExcel ドキュメントを取得する必要がなくなり、インターフェイスで直接データを理解できるようになります。 一貫性を保つために、すべて小文字にすることをお勧めします。

プラットフォーム全体でページ名の一貫性を保つことが常に最善です（アプリの画面名も同様です）。 例えば、「`property:section:sub section:sub sub section:unique page name`」を変数/ディメンションに設定できます。 これらすべてがデータレイヤーの個別のフィールドである場合は、JS ファイル/ローンチでページ名を直接作成することもできます。 これらの要素をすべて独自のディメンションに設定することで、サイトやアプリの特定のプロパティや領域をより簡単に分解し、トラフィックとフローをより詳細に把握できます。

命名規則のような簡単なものも含め、ユーザーがデータを簡単に見つけて理解できるようにするものは、[!DNL Adobe Analytics]の使用を増やし、ビジネスに対してより優れたインサイトを提供します。

## 制作者

この文書は次の人によって共同作成されました：

![ クリステル・ガイドン ](assets/Christel-Headshot-150.png)

Christel Guidon氏（NortonLifeLock、デジタル [!DNL Analytics] プラットフォームマネージャー）
[!DNL Adobe Analytics] チャンピオン

![Rachel Fenwick](assets/Rachel-Fenwick-150.png)

Rachel Fenwick、[!DNL Adobe]のシニアコンサルタント
