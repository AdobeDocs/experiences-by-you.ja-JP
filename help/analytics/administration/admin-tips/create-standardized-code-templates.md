---
title: 標準化されたコードテンプレートの作成
description: ベースライン実装（例：すべての[!DNL Adobe Analytics] サイトに必要なKPIと会社が考えているもの）の場合、組織は可能な限り単一の実装方法を持つ必要があります。
solution: Analytics
feature-set: Analytics
feature: Implementation Basics
topic: Administration
role: Admin
level: Beginner
doc-type: article
thumbnail: 10532.jpg
kt: 10532
exl-id: edd3df73-6d1a-4a26-a984-810cc7dd382f
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
source-wordcount: '358'
ht-degree: 0%
---
# 標準化されたコードテンプレートの作成

**WHAT:** 「ベースライン」実装の場合（つまり、すべての[!DNL Adobe Analytics] サイトに必要なKPIと会社が考えているもの）は、可能な限り単一の実装方法を組織に組み込む必要があります。 例えば、サイト全体で同じデータレイヤー構造を利用し、同じタグマネージャールールとカスタムコードを活用して、内部検索や訪問者プロファイル情報などを取り込みます。

**理由：**&#x200B;繰り返し可能でスケーラブルなベースライン実装を実現することで、新しい要素や新しいサイト/アプリの追加を合理的かつ低い労力で行うことができ、同時に実装をクリーンで簡単にトラブルシューティングできます。 また、統一された方法を使用することで、新しい管理者や開発者がオンラインになり、何を扱っているのかを簡単に理解することができます。

**方法：**&#x200B;新しいサイトまたはタグ付けの機能強化がオンラインになったときに開発者に引き渡すために、単一の形式テンプレートを採用します。 通常、単語文書は、次の項目の概要を説明するのに適しています。

* 実装される変数、目的、設定するタイミング。 例：

| AA変数 | 説明 | 設定するタイミング/場所 | How to Set |
|--- |--- |--- |--- |
| EVAR8 | 内部検索キーワード | 社内検索結果ページのランディングについて | データレイヤー |
| event8 | 内部検索数 | 社内検索結果ページのランディングについて | 起動ルール |

* 設定方法の詳細。 ここで、必要なデータレイヤーオブジェクトとその構文、設定が必要なTMS ルールおよびルール設定の詳細を指定します。
* テスト ケースがQAでカバーされていることを確認し、テスト ケースが成功した場合に表示されるすべての変数を確認します。 開発者がこの機能強化をテストする際に、実装を成功させる際に何を含めるべきかを概説します。

理想的には、このドキュメントは、プロパティ名やページ命名規則などの基本を更新する次のサイトのために調整する必要があります。毎回車輪を再発明する必要はなく、より多くの時間を節約できます。

## 制作者

この文書は次の人によって共同作成されました：

![ クリステル・ガイドン ](assets/Christel-Headshot-150.png)

Christel Guidon氏（NortonLifeLock、デジタル [!DNL Analytics] プラットフォームマネージャー）
[!DNL Adobe Analytics] チャンピオン

![Rachel Fenwick](assets/Rachel-Fenwick-150.png)

Rachel Fenwick、[!DNL Adobe]のシニアコンサルタント
