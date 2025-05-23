---
title: Dynamic Chatを使用したオムニチャネルインタラクティブマーケティングのデザイン
description: Adobe Marketo Engageのネイティブな対話型エンゲージメントチャネルであるAdobe Dynamic Chatを使用して、対話型マーケティングのデザインを簡単に開始できます。 このチュートリアルでは、販売会議の予約、web サイトのコンテンツエンゲージメント、イベント/ウェビナーのプロモーションなど、ユースケースを実装するための実用的なレシピを提供します。
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-23T00:00:00Z
jira: KT-14814
exl-id: 160dfb25-9f54-4dce-a08a-4a8d3c4c5368
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '1409'
ht-degree: 0%

---

# Dynamic Chatを使用したオムニチャネルインタラクティブマーケティングのデザイン

マーケターにとって、web サイトは、リードの生成、コンバージョンの向上、販売サイクルの加速に不可欠です。 Web サイトでリアルタイムに訪問者と関わることで、セールスチームがより効率的に購入者を選定できます。 Adobe Marketo Engageのサブスクリプション内のネイティブチャットチャネルであるAdobe Dynamic Chatを使用すると、会話を自動化して、Marketo Engageの能力を強化できます。

このチュートリアルでは、「同僚から学ぶ」セッションで Cornerstone OnDemand のマーケティング運用マネージャー、Sara Barriuso が共有する、思考プロセスと主なユースケースの概要を説明します。 同氏は、Marketo Engageの能力を最大限に引き出すため、組織がどのようにDynamic Chatを使用したかを説明しました。

## 需要生成戦略への会話エンゲージメントの統合

訪問者が、何らかの理由で web サイトを閲覧したとき。 製品やサービスに関するコンテンツを探している場合や、営業担当者と話すための連絡先情報を探している場合があります。 また、追加の製品情報を探している顧客である可能性もあります。 チャットを使用すると、web サイトの訪問者は、セールスチームと話す準備ができている場合に、セルフサービスおよび自己選定をおこなうことができます。

サラ・バリウソがDynamic Chatを導入したとき、彼女はMarketo Engageとのシームレスな統合と、Marketo Engageプログラムをアクティブ化する [ 事前に構築されたアクティビティトリガー](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-activities){target="_blank"} に惹かれました。 彼女は、3 つのオーディエンスセグメントを念頭に置いて、対話型のエンゲージメント戦略を開発しました。

1. 不明な見込み客：プロアクティブにデモ呼び出しを提供して、新しいリードを生成します。
2. 既知のリード/顧客：訪問者がコンテンツの閲覧に費やす時間を延長し、デモ呼び出しを提供して、アップセルとクロスセルの機会を生み出します。
3. 見込み客/顧客：マーケティングキャンペーンの取り組みを拡張して、パーソナライズされたエクスペリエンスを提供します。


## ダイアログの作成を開始するための主なユースケース

これらの戦略を実装するために、Sara は次のユースケースを中心にDynamic Chatダイアログを構築しました。

1. デフォルトの包括的ダイアログ：すべての訪問者に最初のオプションを提供し、より効率的にタスクを遂行するよう導きます。

2. イベントおよびウェビナー登録の促進：web サイト訪問者をイベントやウェビナーに登録して、より迅速に購入段階に導きます。

3. Campaign コンテンツエンゲージメントの拡張：訪問者が web サイト上のコンテンツを閲覧する際に、追加のコンテキストを提供したり、潜在的な質問に対処したりします。

Sara がプロセスを紹介するように、これらのユースケースを実際に見てみましょう。対話型フローのマッピングから、Dynamic ChatやMarketo Engageでのダイアログやターゲティングの設定まで、多岐にわたります。

### ユースケース 1：すべてのサイト訪問者に対するデフォルトのキャッチオール ダイアログ

このダイアログでは、サイト訪問者が選択できる 5 つの最初のオプションが提供され、ペルソナに基づいて必要な情報を見つけるのに役立つ、セルフガイドのエクスペリエンスが作成されます。 開始するには、「お問い合わせ」のメールインボックスを参照して一般的なテーマを特定し、サイト訪問者に適用されるダイアログオプションに分類します。 デモを見て、次の手順に従ってデフォルトの包括的ダイアログを作成します。

>[!VIDEO](https://video.tv.adobe.com/v/3454848/?learn=on&captions=jpn)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

#### フェーズ 1

1. ダイアログを作成してテストリンクを作成します。
2. コンバージョンを追跡するための目標を追加します（例：デモリクエストの送信）。
3. 2～3 人にテストしてもらい、フィードバックを収集します。

#### フェーズ 2

1. 「オーディエンス」で、「ターゲット」に Web ページの URL を追加して、ダイアログが表示される場所を示します。
2. 「設定」に、キャンペーン名、説明、優先度、言語を追加します。
3. 「Publish」をクリックします

>[!TAB Marketo Engage]

#### フェーズ 1

1. トラッキングスマートキャンペーンを作成します。
2. 「スマートリスト」で、「ダイアログの目標に到達」トリガーを使用します。 ダイアログを使用したのと同じ目標（例：デモリクエスト）を使用
3. 「フロー」に、コンバージョンを追跡するための「プログラムステータスを変更」ステップを含めます。
4. ソースは「dynamicChat」と表示されます。 スマートキャンペーンを作成して、意味のある名前にソースを更新できます。

#### フェーズ 2

1. トラッキング Smart Campaign がライブの場合は再テストします。

>[!ENDTABS]

#### レベルアップ：アカウントベースマーケティング

業界をターゲットにしたコンテンツを組み込むことで、デフォルトのキャッチオール対話をさらに強化し、訪問者にとって会話をさらに役に立てることができます。 例えば、訪問者がダウンロードできるよう、業界固有のホワイトペーパーやケーススタディを提案します。 デモを視聴し、次の手順に従って、アカウントベースのマーケティング用のデフォルトのキャッチオール ダイアログを作成します。

>[!VIDEO](https://video.tv.adobe.com/v/3429195/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. 「デフォルトダイアログ」のクローンを作成して、名前を変更します。
2. 「ストリームDesigner」で、ダイアログメッセージを対象の業界に合わせて調整します（1 つのストリーム +最初の質問）。
3. 2 ～ 3 人のユーザーにダイアログをテストしてもらい、フィードバックを収集します。
4. テストリンクを作成して共有します。
5. 「オーディエンス」に、ダイアログが表示される web ページの URL を追加し、目的の業界をターゲットに更新します。
6. 「設定」に、キャンペーン名、説明の優先度、言語を追加します。
7. 「Publish」をクリックします。

>[!TAB Marketo Engage]

1. トラッキング Smart Campaign を作成し、目標をテストします。
2. ダイアログを公開した後、トラッキング Smart Campaign を再テストします。

>[!ENDTABS]

### ユースケース 2：イベントおよびウェビナー登録の促進

イベントやウェビナーは、B2B ビジネスが需要を生み出すための一般的なマーケティング戦術です。 彼らは魅力的な経験と見込み客を引き付ける豊富な情報を提供します。 Web サイトの訪問者を今後のイベントやウェビナーに接続することで、見込み客の選定をより迅速に行うことができます。 このダイアログの作成は労力とコストがかからず、成功をすぐに示すことができるため、マーケティングの関係者からサポートを得て、オムニチャネル自動化プランに会話によるエンゲージメントを追加するのに役立ちます。 デモをご覧になり、以下の手順に従ってイベント/ウェビナープロモーションのダイアログを作成します。

>[!VIDEO](https://video.tv.adobe.com/v/3429196/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

#### フェーズ 1

1. 進行中のキャンペーン使用のための「イベント登録」ダイアログ用のテンプレートを作成します。

#### フェーズ 2

1. テンプレートのクローンを作成します。
2. 新しいイベント用のダイアログメッセージにテキストをコピー&amp;ペースト
3. イベントリンクで使用する UTM パラメーターを更新します（例：utm_medium=website&amp;utm_source=adobe）。
4. テストリンクを作成し、「Publish」をクリックしてリクエスターと共有します。
5. ピアレビューを行い、フィードバックを適用します。


>[!TAB Marketo Engage]

#### フェーズ 1

1. ウェビナー/イベントプログラムテンプレート内にトラッキングスマートキャンペーンを作成し、テストします。

#### フェーズ 2

1. Marketo Engage内のトラッキングスマートキャンペーンにキャンペーン名を追加し、テストします。

>[!ENDTABS]


#### レベル アップ：既知のユーザーを登録

Web サイトの訪問者にフォームに入力させることなく、イベントやウェビナーに登録することで、訪問者のエクスペリエンスをさらに向上させることができます。 パーソナライズされたエクスペリエンスは信頼を構築し、訪問者に覚えていることを示します。 イベントとウェビナープロモーションのダイアログをレベルアップする方法を、実際に見てみましょう。

>[!NOTE]
>特定の保護国家/国で発生する可能性のあるセキュリティリスクを考慮し、法務チームに相談して、このパーソナライゼーションを慎重に実装してください。

>[!VIDEO](https://video.tv.adobe.com/v/3429197/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. イベント / ウェビナープロモーションダイアログのクローンを作成します。
2. ストリームDesignerで「はい」と回答した後、クエスチョンカードを追加します。 イベントの詳細のためにこのを保持しますか？」が表示されます。
3. 「はい」と答えた場合 – メッセージカードを追加します「イベント/ウェビナーの詳細を記載した確認メールがメールに届きます」
4. 「いいえ」と答えた場合 – メッセージカードを追加します「登録ページのフォームに入力してください」。
5. テストリンクを作成し、「Publish」をクリックしてリクエスターと共有します。
6. 「オーディエンス」タブに、「[ メールは空ではありません ]」を追加します。

>[!TAB Marketo Engage]

1. この新しいダイアログをMarketo Engage内のトラッキング Smart Campaign に追加し、テストします。

>[!ENDTABS]

### ユースケース 3:Campaign コンテンツエンゲージメントの拡張

魅惑的なウィンドウディスプレイが目を引いて店に引き込まれると想像してください。 受付担当者が製品の選択や質問への回答を支援してくれれば、購入する際の安心感が高まるかもしれません。 このエクスペリエンスをオンラインでレプリケートするには、マーケティングキャンペーンが訪問者を誘導する web ページにDynamic Chatダイアログを表示します。 ユーザーが web コンテンツにエンゲージすると、Dynamic Chatはすぐに関連性の高い会話を表示し、コンテンツの追加や潜在的な疑問への対処を提案します。 これを実現するには、自動化トリガーを活用して、Marketo Engageプログラム内のユーザーエンゲージメントに基づいてDynamic Chatキャンペーンをアクティブ化します。 次に、このユースケースを実現する方法を見てみましょう。

>[!VIDEO](https://video.tv.adobe.com/v/3429199/?learn=on)

Campaign コンテンツエンゲージメントの拡張 – 設定：

>[!VIDEO](https://video.tv.adobe.com/v/3429200/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. メールおよびソーシャルキャンペーンのタッチポイントを使用して、キャンペーン用に新しいリードを生成します。 この例では、タレントヘルス インデックス調査がブランドの web サイトでホストされています。
2. 既存のダイアログテンプレート（デフォルトのキャッチオールダイアログなど）のクローンを作成して、次のシナリオに対応する 3 つのダイアログを作成し、それに応じて「オーディエンス」タブの「ターゲット URL」を更新します。
   * Web 訪問者がマーケティングチャネルから来て、web ページにアクセスしたタイミング。
   * 「ありがとうございます」ページで
   * マーケティングキャンペーン（リターゲティング）を行ってから 45 日以内に web サイトに戻る訪問者

>[!ENDTABS]

## 次の手順

* [ ストリームDesigner](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer){target="_blank"} またはオフラインのフローチャートで、会話フローをマッピングします。
* Dynamic Chatでデフォルトのキャッチオールダイアログを作成します。
* Marketo Engageの自動処理トリガーを使用して、キャンペーン後のエンゲージメントに関する会話をアクティブ化します。


## 作成者

{{sara-barriuso}}

{{amy-chiu}}
