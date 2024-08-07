---
title: 標準化された命名規則の作成
description: 標準化された命名規則は、AA 管理 UI で有効にした場合の変数名自体と、ディメンションに渡される値の両方に適用されます
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
source-git-commit: c568ed0a06551d910b6f533698ec47c15adecf6c
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# 標準化された命名規則の作成

**対象：** 標準化された命名規則は、[!DNL Adobe Analytics] （AA）管理 UI で有効にした場合の変数名自体と、ディメンションに渡される値の両方に適用されます （つまり、ページ名は変数名として「ページ名（v1）」とし、渡されるページ名の値は「サイト名|ホームページ」や「サイト名|検索|検索結果」のように特定の構造と階層に従うように統一する必要があります）。

**理由：** 命名規則は、すべてを統一し、ユーザーが理解しやすいインターフェイスを維持するための優れた方法です。 最初からこれらを作成し、プラットフォームとコードで適用すると、拡張が容易になります。

**方法：** 「名前」と「説明」の両方で、インターフェイスとタグ付けドキュメントが一致する必要があります。これにより、ユーザーは Excel ドキュメントを取り込む必要がなくなり、インターフェイスで直接データを把握できるようになります。 一貫性を保つため、常に小文字のみを使用することもお勧めします。

ページ名（アプリの場合は画面名）は、プラットフォーム全体で常に統一しておくとよいでしょう。 例えば、「`property:section:sub section:sub sub section:unique page name`」を変数またはディメンションに設定できます。 これらがすべてデータレイヤーで別々のフィールドになっている場合は、JS ファイルまたは Launch で直接ページ名を作成することもできます。 これらの要素をすべて独自のディメンションに設定すると、サイトやアプリの特定のプロパティや領域をより簡単に分類し、トラフィックやフローをより深く理解できます。

命名規則のように単純なものを含め、ユーザーがデータを見つけて理解しやすくなれば、[!DNL Adobe Analytics] の使用率を高め、ビジネスにより優れたインサイトをもたらします。

## 作成者

このドキュメントの共同作成者：

![Christel Guidon](assets/Christel-Headshot-150.png)

Christel Guidon （NortonLifeLock、デジタル [!DNL Analytics] ッドレスプラットフォームマネージャー）
[!DNL Adobe Analytics] チャンピオン

![ レイチェル・フェンウィック ](assets/Rachel-Fenwick-150.png)

Rachel Fenwick （[!DNL Adobe] 社シニアコンサルタント）
