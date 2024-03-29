---
title: への移行に関する包括的なガイド [!DNL Adobe Analytics] Googleから [!DNL Analytics]
description: 同等の機能の場所と、Googleから移行する際にその機能を効率的に使用する方法について説明します。 [!DNL Analytics] から [!DNL Adobe Analytics]
solution: Analytics
feature: Third-party Integration
role: User
level: Beginner
kt: 9830
thumbnail: 34749.jpg
source-git-commit: c6c9e5b19c601592811151450aecd8dfdd084ff6
workflow-type: tm+mt
source-wordcount: '3323'
ht-degree: 72%

---

# への移行に関する包括的なガイド [!DNL Adobe Analytics] Googleから [!DNL Analytics]{#comprehensive-guide-for-transitioning-to-adobe-analytics}

## 1. はじめに

ツール間の移行での最大の課題の 1 つは、同等の機能がどこにあるのかを知り、それを効率的に使用する方法を学ぶことです。このディスカッションは、ユーザーが [!DNL Adobe Analytics] ( 新しいユーザーとして、またはGoogleからのユーザーとして ) [!DNL Analytics]) が簡単になりました。 GA との詳細な比較。ほとんどのユーザーになじみがある最も適した比較ツールとして、ユーザーが既存の知識を新しいツールセットに関連付けるのに役立つように提供されています。実践に代わるものはありませんが、これは基本を学ぶのに役立ち、移行中に感じる可能性のあるフラストレーションを減らすことができます。

用語を簡単に比較する必要があります。

| **説明** | **[!DNL Adobe Analytics]** | **Google[!DNL Analytics]** |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------|----------------------|
| ページ（またはアプリの画面）を表すイベント指標が表示されました | ページビュー | ページビュー |
| 同じ時間枠で行われる web サイトまたはアプリでのインタラクションのグループを表す指標 | 訪問 | Session |
| 識別されたデバイスを定義する指標（ユーザー情報をつなぎ合わせるための Cookie やその他のビヘイビアーパターンを含む複数の基準に基づく） | ユニーク訪問者 | ユーザー |

## 2. インターフェイス

顧客の比較時 [!DNL Adobe Analytics] とGoogle [!DNL Analytics]、彼らは次のようにコメントします。 [!DNL Adobe]最初は、のインターフェイスが大変な作業でした。 これが真実ですが、信じられないかもしれませんが、それは弱点ではなく強みでもあります。[!DNL Adobe] は、データの視覚化に幅広いツールと柔軟性を提供し、必要なものをより自由に作成できます。

まず、「サイト内」レポートを見てみましょう。

### 2.1. サイト内レポート

#### 2.1.1. ホーム画面

両方 [!DNL Adobe Analytics] とGoogle [!DNL Analytics] ユーザーがログインしたときに表示される最初の表示をカスタマイズする方法を提供します。

##### 2.1.1.1.ワークスペース/カスタムセットのホーム画面 ([!DNL Adobe Analytics])

[!DNL Adobe Analytics] では、すべてのユーザーがログイン時に表示する事前定義済みレポートを作成することを推奨しません。 デフォルトのホームページでは、ユーザーは Workspace のランディング画面に移動します。ここには、各ユーザーが作成または共有したすべてのワークスペースレポートが表示されます。また、各ユーザーは、必要に応じて、これらのレポートのいずれかをホーム画面として設定できます。

![workspace-create-project](assets/ga-to-aa_1.png)

後ほどこのガイドで、ワークスペースについて詳しく説明します。2.1.2.1 節を参照

>[!TIP]
>
>組織の標準レポートを作成／共有して、すぐに独自のレポートを作成しなくても情報を確認できるようにします。



##### 2.1.1.2.ホーム画面のインサイト (Google [!DNL Analytics])

* Google [!DNL Analytics] ホーム画面には、事前に作成されたビジュアライゼーションがいくつかあります。 これらには、次のような情報が含まれています。
* 過去 7 日間のユーザー数、セッション数、バウンス率およびセッション時間
* 過去 30 日間の時間帯別のユーザー数
* 今現在のユーザーと上位のアクティブなページ
* 過去 7 日間のトラフィックチャネル、ソース／メディアおよび参照
* 過去 7 日間の国別セッション数
* 過去 7 日間のトップページ
* 過去 30 日間のアクティブユーザーの傾向
* その他の機能

GA4 ユーザーには、カスタマイズした独自のレポートをホーム画面に追加するためのより多くのオプションがあります。

![google-analytics-interfaces](assets/ga-to-aa_2.png)

これが、おそらくあなたが最も欠けていることの 1 つです [!DNL Adobe Analytics]. 事前に作成されたホーム画面はありません。 ただし、上記のリストから必要なものをレプリケートしてランディング画面として設定するように、カスタムワークスペースを簡単に設定できます。このトピックに関する詳細は後で説明します（または 2.1.2.1 節を参照）。 [!DNL Adobe] ワークスペース )。

#### 2.1.2. サイト内の Report Builder

分析ツールが提供するシンプルなレポートに加えて、各ツールは、独自のカスタムレポートを作成するためのより強力なツールも提供します。

##### 2.1.2.1. [!DNL Adobe Analytics] Workspace

これが～の大きな力を持つ家だ [!DNL Adobe Analytics]2017 年の導入以来、次の場所に移りました。 [!DNL Analytics] 分析を行い、「レポート」セクションがまもなく終了する主な理由を示します。

このツールを使用すると、ほとんど完全に自由にレポートを作成できます。

レポートはパネルに分割でき、それらのパネルには任意の数のビジュアライゼーションを含めることができます。パネルは、日付範囲や共通セグメントフィルターなどの一般的な情報に設定できます。

パネルとその中のビジュアライゼーションの両方をサイズ変更してドラッグし、アイテムを並べて表示したり、積み重ねたりすることができます。したがって、2 つの異なるデータスイートを並べて比較する場合は、中央で 50/50 に分割されたパネルを作成し、2 つのサイトを並べて簡単に比較できます。

ユーザーが利用できるビジュアライゼーションは多数あります。

* フリーフォームテーブル
* コホートテーブル
* フォールアウト
* フロー
* グラフ
   * 面グラフ（積み重ねおよび非積み重ね）
   * 行
   * 散布図
   * 棒グラフ（積み重ねおよび非積み重ね）
   * ブレット
   * ドーナツ
   * ヒストグラム
   * 横棒グラフ（積み重ねおよび非積み重ね）
* マップ
* ブロックの概要
   * 変更の概要
   * テキストの概要
   * テキスト（コンテキストを提供するために追加情報を入力するためのフリーテキストフィールド）
* ベン

各パネルとビジュアライゼーションにはタイトルを付け、説明を適用して、情報が表示している内容にコンテキストを提供することができます。
In [!DNL Adobe]に設定されたセグメント（基本的にはデータのフィルター）は過去に遡って適用され、フリーフォームテーブルの列に取り込んで、データを並べて比較できます。 例えば、ユーザーがサイトの 2 つの異なるカテゴリのトラフィックを比較する場合は、「カテゴリ A」のセグメントと別の「カテゴリ B」のセグメントを作成できます。

![analytics-page-views-report](assets/ga-to-aa_3.png)

フリーフォームテーブルでは、必要に応じて複数の列とセグメント化を使用して、データを思いどおりに可視化できます。

日付別の分類を表示しない場合は、別のディメンションやセグメントをそこにラッグ＆ドロップするだけで、別の方法でデータを表示できます。例えば、デバイスタイプにセグメントを使用し、モバイル／タブレットユーザーに対してオペレーティングシステム別の分類を追加できます。

![analytics-compare-page-views-report](assets/ga-to-aa_4.png)

Workspace では創造性を伸ばすことができます。「標準」的な分類に制限されるわけではありません。実行する必要のある比較を深く掘り下げるために必要なビジュアライゼーションを作成できます。

>[!TIP]
>
>臆せず自由に使ってみて機能を探ってください。既存の枠にとらわれない考え方がいろいろあります。 さらに、作成したものが自分の考えを示しているかどうかを検証してください。経験が役に立ちます。

レポート内でのみ有効なオンザフライの計算指標やセグメントを作成して、セグメントや計算のリポジトリがあふれないようにすることができます。これにより、他のコンテキストでは使用できないもので組織を混乱させることなく、特定のレポートに必要な項目に的を絞って作成できます。　

この解説は、このツールの紹介にすぎません。基本を学ぶためのより包括的なガイドは他にもあります。これらのガイドを確認したら、次のような包括的なレポートを作成します。

![workspace-dashboard](assets/ga-to-aa_5.png)

ワークスペースは自動保存されないので、レポートリポジトリをいっぱいにすることなく、1 回限りのアドホックレポートを実行しやすくなります。

Workspaces のもう 1 つの強力な機能は、ドロップダウン形式でレポートにインタラクティブな修飾子を適用できることです。これらのドロップダウンは、書き出された CSV や PDF ファイルのレポートでは機能しません。ただし、ライブレポートでは、パネル内のすべてのビジュアライゼーションを更新して、同じレポートを異なる条件で表示できます。複数のドロップダウンを使用することができ、オプションが相互に排他的でない場合、選択された項目は積み重ねられ、情報をきれいに表示できます。

>[!IMPORTANT]
>
>ドロップダウンとフリーフォームの分類の使用について詳しくは、<https://experienceleaguecommunities.adobe.com/t5/adobe-analytics-discussions/the-power-of-dropdown-filters-and-dimension-breakdowns-in-adobe/td-p/434680> を参照してください。

##### 2.1.2.2.GOOGLE [!DNL Analytics]：ダッシュボード、カスタムレポート、保存済みレポート

Google には、インターフェイス内でレポートを作成するためのツールがいくつかありますが、それらは引き続きレポートセクションと同じ表示と制限に従います。

さて、Googleに詳しい人々のために [!DNL Analytics] これを読むとこう言うかもしれません「ちょっと待ってくださいGoogle Data Studio に関してはそれほど良いことではありません [!DNL Adobe]ワークスペースか？」 はい。ただし、Data Studio は、技術的には [!DNL Analytics] ツールを使用し、異なるデータソースへの接続を可能にします。 このツールは、「拡張レポートアクセス」の節、特に 2.2.3 節で後述します。

Google ダッシュボードとカスタムレポートを使用すると、複数のビジュアライゼーションを 1 つのレポートにまとめることができますが、Workspace とは異なり、単純な相関関係と、どのデータをどの列に配置できるかが決まります。

カスタムレポートで最も大きな課題の 1 つは、フィルターを作成する際に、レポートのすべてのタブに適用される点です。同じレポート内の 2 つの異なるフィルターを比較する方法はありません。

表面上の比較の場合は、問題ありません。これらはすべて、 [!DNL Adobe] レガシーダッシュボード、カスタムレポートおよびブックマーク。 ニーズをサポートするために提供される基本ツールは、レポートスイート内に存在します。

#### 2.1.3. レポート

Googleと [!DNL Adobe] には、ディメンションに基づく、作成されたテーブルと基本的なタイムライングラフを持つナビゲーション可能なレポートがいくつかあります。

##### 2.1.3.1. [!DNL Adobe Analytics] レポート

[!DNL Adobe Analytics] には「レポート」セクションもありますが、廃止されてAnalysis Workspaceに置き換えられています。 実際、Workspace はより強力なツールなので、このインターフェイスのサービス終了が発表されました。これらのテーブルのほとんどは、容易に作成したり変更したりできます。[!DNL Adobe]のセクションは、よりはるかに分かれており、これは骨の折れることがあります。

![analytics-site-metrics](assets/ga-to-aa_6.png)

上記のほとんどが Workspaces 経由でアクセスできるので、これらの節の概要と、それらがGoogleとどのように関連しているかを簡単に説明します [!DNL Analytics]をクリックし、まだ関連性のあるレポートをここでハイライトします。

サイト指標には、標準指標（設定したページビュー数、ユニーク訪問者数、訪問回数、カスタムイベント数）が含まれています。これは行動レポート GA に似ていますが、オーディエンスに何が含まれるかも示します ( [!DNL Adobe] では、指標のタイプは分割されません )。

ここには「ボット」レポートがあります。ボットからのトラフィックはすべての標準レポートから除外されていますが、2 つのレポートで、何が起こっているのか、どのボットがサイトにアクセスしているのかのインサイトを確認できるレポートが 2 つあります。これは、サイトに頻繁にヒットする既知のスパマーボットを除外するカスタムボットルールを設定する場合に特に便利です。メインのレポートがフラッディングすることなく、それらのボットがそのトラフィックを実行していることについてのインサイトを得ることができます。ボットレポートは現在、Workspace からは利用できません（ただし、間もなく登場するレポートの新機能により、ユーザーはボットレポートでもこの情報を取得できるようになります）。

サイトコンテンツは [!DNL Adobe] 標準ディメンション：ページ名、サイトセクション、階層、サーバーなど。 Workspace ではこれらのディメンションすべてを利用できます。

Mobile は、モバイルデバイス固有のデータ（デバイス、デバイスタイプなど）をグループ化したものです。Workspace ではこれらを利用できます。

Workspace ではパスを利用できません。Workspace にはフロー図があり、単一ページ／値のインフローとアウトフローを確認できます。一方、パスを使用すると、web サイトで最もよく使用されるパスを表示できます。デフォルトでは、最初に設定されるパスレポートはページです。ただし、「ページタイプ」の値などのカスタム prop に対してこれをオンにできます。ページタイプ内のパスを確認できます。パスについて個人的に気に入っているもう 1 つの点は、情報を表示する簡単な方法であることです。ワークスペースのフロー図（見ようとしている量によって異なります）は、圧倒される可能性があります。両方を試してみることをお勧めします。それぞれ、達成しようとしていることに応じて用途と価値があります。フローでは任意のディメンションを使用できますが、パスは管理パネルのプロップで設定する必要があります。

トラフィックソース、 [!DNL Campaign]およびマーケティングチャネルレポートは、すべてGoogleの製品の獲得レポートに似ています。 トラフィックソースは実際のリファラーに焦点を当てています。 [!DNL Campaign]が [!DNL Campaign] コードとマーケティングチャネルでも、 [!DNL Campaign] コードに加えて、情報の処理方法に関してユーザーが決定した追加のロジックも適用されます。 [!DNL Adobe] では、ルールの設定方法をより自由に使用できます。 一方、Google は多数の機能が用意されているので、考え方も変える必要があります。デフォルトでは、Googleの属性は [!DNL Campaign] コードは 6 か月です。 [!DNL Adobe]のアトリビューションは、デフォルトで 1 週間に設定されています。 これは管理者設定で変更できますが、Workspace では、実際に任意のディメンションにカスタムアトリビューションを適用して、「即座」の柔軟性を大幅に高めることができます。

訪問者保持率レポートと訪問者プロファイルレポートは、Googleのオーディエンスレポートに似ています [!DNL Analytics]. 保持率は返品頻度に重点を置いていますが、訪問者プロファイルはユーザーの地理とテクノロジーに重点を置いています。

カスタムコンバージョンレポートとカスタムトラフィックレポートは、両方ともカスタムディメンションレポートです。 コンバージョンは eVar です。 ヒット、訪問、月、年などの値にカスタムの有効期限を設定できます。 この値は上書きされない限り、設定された時間枠のユーザーに対して永続的に保持されます。 トラフィック変数は prop です。 パスレポート用に、またはリストアイテムとして設定することもできます（選択した区切り文字に基づいて複数の値を分割します）。

メディアは、特別なメディアトラッキングを設定したビデオやオーディオファイルなどに使用されます。

カスタムレポートは、ユーザーがレポートインターフェイス内で作成した列と分類をカスタマイズして、カスタムレポートとして保存できるセクションです。ただし、前述のように、Workspace では非常に強力な分類と相関関係が可能であるため、カスタマイズした情報はすべてそこで作成する必要があります。これは、Workspace が存在する前の優れたソリューションでした。

ブックマークセクションはカスタムレポートに似ており、頻繁に使用するレポートをレポートインターフェイス内でブックマークして、簡単に見つけられるようにすることができます。

ダッシュボードは、データのレポートレットを 1 つのビジュアライゼーションにまとめることができるレガシー製品でした。ただし、Workspace の機能（2.1.2.1 節）は操作が非常に簡単であるため、これは、この機能が廃止される前に再作成する必要があるレガシーレポートへのアクセスポイントとしてのみ存在します。

ターゲットを使用すると、特定の期間内のターゲットに基づいてレポートを作成できます。 チームはキャンペーンを監視して、トラフィックターゲットを達成するために順調に進んでいるかどうかを確認できます。

ここにあるすべてのレポートでは、複数の指標列とディメンションの分類が可能でした。ただし、ビジュアライゼーションの単純さと、どの要素を相関させることができるかの背後にあるロジックのいくつかは、フラストレーションを引き起こすこともありました。

##### 2.1.3.2.GOOGLE [!DNL Analytics] レポート

Google [!DNL Analytics] では、これらのレポートを次のセクションに分割します。リアルタイム、オーディエンス、獲得、行動および会話 (GA3)、ライフサイクル（獲得、エンゲージメント、収益化、定着）、ユーザー（サブセクション：デモグラフィックとテック）。

![google-analytics-interface-compare](assets/ga-to-aa_7.png)

これらのビジュアライゼーションの微調整、セカンダリディメンションの分類の追加、ビジュアライゼーションの変更、データへのフィルター作成などを行えます。カスタマイズを保存済みレポートとして保存できます。

これらは、データに対する迅速で簡単なインサイトを提供します。ただし、ユーザーなどを同じテーブル内のページのページビューと比較したり、複数のディメンションを追加して追加のデータを表示したりすることはできません。

これらは迅速な分析データには適していますが、本当に深く掘り下げる必要がある場合は、制限があります。

### 2.2. 拡張レポートアクセス

「サイト内レポート」に加えて、ほとんどのツールは、ツールの外部で分析を行い、もう少しカスタマイズされたものを作成できる拡張機能を提供します。

#### 2.2.1. [!DNL Adobe Analytics] Report Builder(Microsoft® Excel 拡張機能 )

Workspace は優れたツールですが、複数のデータソースをつなぎ合わせるために、データをカスタマイズされたスプレッドシートに取り込む必要がある場合があります。ここで、Report Builder が役立ちます。

Report Builderは、Microsoft® Excel 用のプラグインで、 [!DNL Adobe Analytics] Excel 内で操作できる表形式のデータを取り込むためのデータ。 通常、これを効率的に使用するには、データをいくつかの生データタブに取り込み、Excel セル参照を使用してこれらのタブから単一の統合レポートにデータを取り込み、グラフとビジュアライゼーションを作成します。

>[!NOTE]
>
>Report Builder には、このプラグインにアクセスするユーザーに適用する必要がある特別な権限があります。この機能は、ツールの適切な使用方法を学んだユーザーに付与する必要があります。

#### 2.2.2.2. [!DNL Adobe Analytics] API 接続

必要に応じて [!DNL Adobe Analytics] Excel 以外の何かによって消化されるデータ、およびボットルールの除外を含む処理済みデータを使用する [!DNL Adobe]データを直接取り込むためのの API。 次に、スクリプトを介して処理するか、別のシステムで使用するためにデータベースに追加します。

API は、プルリクエストで指定されているように、分類とセグメントを適用して相関データを取り込むことに注意が必要です。

[!DNL Adobe]の Workspace（セクション 2.1.2.1）は、API を使用してレポートを作成します。Workspace でデバッグモードを有効にすると、使用した正確な API 呼び出しが表示されます。 この方法を使用すれば、API 呼び出しをすばやく作成することができます。Workspace を使用して取り込むデータを作成および検証すると、それらの API 呼び出しを使用してデータを独自の処理に出力できます。


#### 2.2.3.GOOGLE [!DNL Analytics] Data Studio

読み進めた方は、上記から、Data Studio をと同等のものとして挙げたことを既にご存じでしょう。 [!DNL Adobe]の Workspace。 Data Studio を使用すると、Googleにプルインできます。 [!DNL Analytics] データを含むデータを抽出し、他のソースからのデータも抽出します。 このことは、分析データを他の収集されたデータと統合する場合に便利です。しかし、Google [!DNL Analytics]と同じタイプのビジュアライゼーション制限が存在します。 行と列の形成方法はまだ制限されています。

それでもこのツールは強力なので、使用をやめろと言うつもりはありませんが、私の個人な経験として、個人的には厳密なビヘイビアーが非常に制限されていると感じています。


#### 2.2.4. Google スプレッドシート拡張機能

独自の用途で、Googleから拡張された方法でデータを取り込む必要がある場合 [!DNL Analytics]私が選択した個人用ツールは、 Google Spreadsheet Extension です。 GA テーブルへの複数の接続を確立する必要がありますが、生データからセルを参照して必要なレポートを作成できます。次に、Google スプレッドシートのグラフ機能を使用して視覚化します。


## 3. 生データの書き出し

実際に生データが必要な場合は、 [!DNL Adobe] Googleは、この方法で情報を取り込む機能を提供します。

### 3.1. [!DNL Adobe] データフィード

2.2.2 節で、私は [!DNL Adobe Analytics] 「処理済みのデータ」から API が取り出されました。 生データフィードは、管理パネルで設定された「処理ルール」によって処理されるデータを取り込みますが、この生データには、その他のすべての場所で除外されるすべてのデータが含まれます。

これは、すべてのボット除外、内部 IP フィルター処理されたデータ、その他の除外データが生データフィードに含まれることを意味します。このデータを識別するフラグがあるので、データレイクを作成する場合、エンジニアリングチームは、フラグンしたがってこのデータを処理するロジックを作成できます。

生データフィードは、データのすべての列を送信するようにカスタマイズすることも、より焦点を絞ったフィードが必要な場合は特定の列のみを送信するようにカスタマイズすることもできます。

フィードは、FTP、SFTP、S3 などに直接送信できます。


### 3.2. Google Big Query

残念ながら、これは私が使用した経験のない 1 つのGoogleツールです。 理論的には、次のようになります。 [!DNL Adobe]のデータフィード ( エンジニアリングチームがGoogleから生データにアクセスできるようにする ) [!DNL Analytics] アカウント。

ただし、エンジニアは、生データの完全なダンプではなく、SQL クエリを使用してデータにアクセスし、ターゲット化された生データや生データのすべての列を取り込むことができます。

## 4. まとめ

他のシステムと同様に、ツールを快適に使用するためには練習が必要です。うまくいけば、このガイドは、を使い始める際に役立ちます。また、 [!DNL Adobe Analytics].

しかし、私は両方を使うことを勧めたいと強調する [!DNL Adobe Analytics] とGoogle [!DNL Analytics] (GOOGLE [!DNL Analytics] は、無料版のみです )。 確実なシステムはありませんが、これによりバックアップシステムを使用してデータを確実に保持できます。

このガイド以外にも、戦略の改善に役立つリソースが多くあります。

* [[!DNL Adobe] Experience League](https://experienceleague.adobe.com/?lang=ja#home)  — チュートリアル、ビデオ、ドキュメントおよびコミュニティフォーラムが含まれます
* [[!DNL Adobe] ユーザーグループ](https://analytics-augs.adobe.com/)  — ユーザーが相互に接続し、実装を改善するのに役立つ、コミュニティ実行イベントのハブ。
* [[!DNL Adobe Analytics] ユーザーグループYouTubeチャネル](https://www.youtube.com/channel/UCQOHnCs7KZgsuFHVzwboQuA)  — を作成できませんでした [!DNL Adobe Analytics] ユーザーグループセッション？ 世界中の過去のユーザーグループセッションを再視聴して、同業者がどのようにツールを使用しているかを知ることができます。
* [チャットSlackチャネルを測定](https://www.measure.chat/)  — との接続 [!DNL Adobe Analytics] 世界中のユーザーと共有し、業界の知識を共有し、仲間に質問し、測定に焦点を当てた関心グループに参加します。
* その他

## 作成者

このドキュメントの作成者：

![Jennifer Dungan](assets/Jennifer_Dungan_Headshot150.png)

Jennifer Dungan、最適化マネージャ [!DNL Analytics] トースターで

[!DNL Adobe Analytics] チャンピオン

