---
title: コホート分析を使用して顧客行動を把握
description: 顧客体験と売上高を向上させるには、企業は顧客の行動を理解する必要があります。 コホート分析は、エンゲージメントとリテンションを把握し、アカウント作成の改善や大量の月にわたるキャンペーンの作成などのアクションを導くのに役立ちます。
feature-set: Analytics
feature: Cohort Analysis
role: User
level: Experienced
doc-type: Article
last-substantial-update: 2023-05-16T00:00:00Z
jira: KT-13213
thumbnail: KT-13213.jpeg
exl-id: 79392eea-a8b6-4ae2-98ef-6ebbd11d88a0
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 12%

---

# コホート分析を使用して顧客行動を把握

顧客体験と売上高を向上させるには、企業は顧客の行動を理解する必要があります。 コホート分析は、エンゲージメントとリテンションを把握し、アカウント作成の改善や大量の月にわたるキャンペーンの作成などのアクションを導くのに役立ちます。

デジタルパフォーマンスの分析は、顧客がビジネスとどのようにやり取りするか、およびエクスペリエンスを向上させるために実行できるアクションを理解する上で重要です。 このブログ投稿では、コホート分析を使用して顧客の行動をより深く理解する方法を検討します。

## 第 1 部：初回訪問と再来訪でのデジタルパフォーマンスの比較

### ステージの設定

あるクライアントは、過去 2 年間のデジタルパフォーマンスを把握しようとしており、デジタルパフォーマンスを高めるロイヤリティープログラムの開発を検討しています。 新規ユーザーとリピートユーザーの現在のサイトを見て、2 つの訪問者グループの現在の行動を把握することができます。

現在のデジタルパフォーマンス

1. 2022 年には、初回訪問からの購入回数の 62%が再来訪からの購入回数の 38%（cookie、複数のデバイスが原因）に対して、初回訪問からの購入回数の 62%が増加しました。
1. 初回訪問回数は、両方の（11.6%と 11.4%の）再来訪回数よりも若干高い率でコンバートされます。
1. 2021 年と比較して、両方のセグメントでコンバージョン率が低下しています。

![訪問回数テーブル](assets/cohort1.png)

## 第 2 部：コホート分析 — 訪問者による食べられる取り決めグローバルな製品

デジタルチャネルの定着度を把握し、リピート購入者を促す機会を把握するために、次に回答するべき質問は、2022 年に毎月サイトに戻ってきた訪問者の量はどれくらいかということですか。

### コホート分析の概要

コホート分析は、コホートが時間の経過と共にブランドとどのように関わっているかを理解するのに役立つツールです。 まず、どの質問に答えるべきかを決定しました。

1. 指定した年で、月別の平均保持期間はどれくらいですか？
1. 指定した 1 年間に毎月再訪するサイト訪問者の数はどれくらいですか？
1. ログインによるリテンションへの影響は何ですか。
1. 保持率を高める特定の製品はありますか？

コホートテーブルの設定方法

1. 日付範囲を 2022 年 1 月から 12 月に設定
1. **インクルージョン条件：** 訪問回数
1. **リターン条件：** 訪問回数
1. **精度：** 月
1. **設定：** ローリング計算\*\*インクルードされた列ではなく、直前の列に基づいてリテンションを計算できます。 つまり、ユーザーは各月に含まれます\*\*
1. **セグメント：** 特定のセグメントを選択して、この分析をさらに促進できます。
   1. 特定のランディングページ
   1. Device Type
   1. マーケティングチャネル
   1. 等。

### 結果の解釈

**2022 年：**

1) 保持率が最も高い月+1 ヶ月は、1 月、4 月、11 月です
1) 最もボリュームの多い月は、2 月と 5 月です
1) 毎月最大 1,000 人の訪問者がサイトに戻ります

![2022 年リテンションテーブル](assets/cohort2.png)

**2021 年：**

1) 保持率が最も高い月+1 ヶ月は、4 月、1 月、3 月です
1) 最もボリュームの多い月は、2 月と 5 月です

![2021 年リテンションテーブル](assets/cohort3.png)

**アクション項目：**

最大 1,000 人の訪問者に基づいてセグメントを作成し、その詳細を確認します。

- どこにありますか？
- 1 年を通じてどの製品を購入していますか。
- 彼らはどの店から買っているのですか。

主要な月は、ボリュームに基づいて保存を促進する機会を強調します。

- 2 月と 5 月の間に、ボリュームを活用するために、さらにスティッキー性を高める特定の戦術はありますか？

リピート購入者を理解するために、注文に対して分析を繰り返します。

- 同じ月の保持率が最も高い+1 ヶ月か。
- 訪問回数の最も高い月数は、注文件数で同じですか？

## パート 3：インクルージョン条件に 2 つの指標を追加

### ログインの影響について

このクライアントはロイヤリティプログラムの価値を理解しようとしているので、分析の次の手順では、ログイン成功イベントにコホートへのインクルージョン指標としてを追加することが含まれていました。

注意：コホート分析は、計算指標（コンバージョン率など）や非整数指標（売上高など）には使用できません。 コホート分析 で使用できるのはセグメントで使用できる指標のみで、一度に増やせるのは 1 を超える数のみです。

ログインしているユーザーをサイトで保持する可能性は高いか。

より多くのユーザーがログインできたら、どうなるでしょうか？ それは粘り強い経験ですか？

### コホートテーブルの設定

1. **日付範囲の設定：** 1 月から 2022 年 12 月まで
1. **インクルージョン条件：** 訪問回数+ログイン成功イベント
1. **リターン条件：** 訪問回数
1. **精度：** 月
1. **設定：** ローリング計算\*\*インクルードされた列ではなく、直前の列に基づいてリテンションを計算できます。 つまり、ユーザーは各月に含まれます\*\*

### 結果の解釈

**2022 年：**

1) リテンション率が最も高い月+1 ヶ月は、1 月、4 月、11 月です（最初のコホートテーブルと同じ月）
1) 最もボリュームの多い月は、2 月、5 月、12 月です
1) 毎月 2500 人以上の訪問者が再訪します\*\*倍以上

**アクション項目：**

チェックアウト時にユーザーがアカウントを作成できるようにするための、サイトのユーザーエクスペリエンスを調査します。

![コホートテーブル 4](assets/cohort4.png)

## 第 4 部：カスタムDimensionコホート

カスタムディメンションコホート：時間に基づくコホート（デフォルト）ではなく、選択したディメンションに基づくコホートを作成します。多くのユーザーは、時間以外の基準でコホートを分析したいと考えています。新しいカスタムディメンションコホート機能では、顧客が選択したディメンションに基づいてコホートを柔軟に構築することができます。マーケティングチャネル、キャンペーン、製品、ページ、地域、その他のディメンション ( [!DNL Adobe Analytics] を参照して、これらのディメンションの様々な値に基づくリテンションの変化を表示します。 「

カスタムDimensionコホートセグメント定義では、ディメンション項目をリターン定義の一部ではなくインクルージョン期間の一部としてのみ適用します。

カスタムディメンションコホートオプションを選択した後、任意のディメンションをドロップゾーンにドラッグ＆ドロップします。これにより、同じ期間内で類似したディメンション項目を比較できます。 例えば、市区町村のパフォーマンスを並べて比較できます

サイド、製品、キャンペーンなど 上位 14 件のディメンション項目が返されます。 ただし、フィルターを使用して（ドラッグしたディメンションの右側にマウスポインターを置いて）、目的のディメンション項目のみを表示できます。 カスタムディメンションコホートは待ち時間テーブル機能とともに使用することはできません。

### どの製品がサイトの定着率を高めていますか。

カスタムDimensionコホートテーブルでは、平均よりも高い定着率を引き起こしている製品について重点的に説明します。  この表は、注目に値する製品を特徴とする、内部および外部のマーケティングキャンペーンを促進する、上位の製品を特定するのに役立ちます。

**2 月：** 保持率の高い 3 つの製品が立ち上がる

1) Product 1
1) Product 2
1) Product 3

**3 月：**

1) Product 1
1) Product 2
1) Product 3 ：平均保存率に比べ、保存率が高い方がパフォーマンスが優れています。

![コホートテーブル 5](assets/cohort5.png)

## まとめ

コホート分析とカスタムDimensionコホートは、顧客の行動を把握し、デジタルパフォーマンスを向上させるための強力なツールです。 保持率、ログイン率、特定の製品の影響を分析することで、企業はデータに基づく意思決定を行い、顧客体験の向上と成長の促進を図ることができます。

## 作成者

このドキュメントの作成者：

![ジェニファーヤセンダ](assets/jennifer-yacenda.png)

**ジェニファーヤセンダ**，シニアDirectorアットマリオット

[!DNL Adobe Analytics] チャンピオン
