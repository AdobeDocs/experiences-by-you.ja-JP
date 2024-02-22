---
title: 計算指標によるデータ分析レベルの向上
description: ピアエキスパートが計算指標を使用して、実装を変更せずに新しい指標を作成する方法や、収集済みのデータを使用して、複雑なビジネスの質問に答える方法を説明します。
feature-set: Analytics
feature: Calculated Metrics
role: User
level: Beginner
doc-type: Article
last-substantial-update: 2023-05-16T00:00:00Z
jira: KT-13266
thumbnail: KT-13266.jpeg
exl-id: 301ee179-b154-4cf2-b27e-77f38a8945a0
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '1549'
ht-degree: 3%

---

# 計算指標によるデータ分析レベルの向上

の最も新しいユーザー [!DNL Adobe Analytics] は、データをスライスして多角的に分析する方法として、セグメントに精通しています。 今日は、アナリストツールボックスで次に優れた計算指標をご紹介します。

の高度な機能として [!DNL Adobe Analytics]では、計算指標を使用すると、既に収集したデータを使用して実装を変更することなく、新しい指標を作成できます。 計算指標ビルダーでは、様々な数学関数や統計関数を使用できるので、最も複雑なビジネス上の質問にも答える指標を作成できます。

## 計算指標の概要

計算指標の使用を開始するには、簡単な例を見てみましょう。 オンラインのセルフサービスユーザーの平均注文額 (AOV) がコールアシストユーザーよりも高いかどうかを把握したいとします。 この質問に回答する計算指標を作成するには、次の手順を実行します。

計算指標ビルダーを開くには、上部のナビゲーションを使用して「→」をクリックします **コンポーネント** → **計算指標** → **+追加。** または、 **+記号** 上 **指標** 」と入力します。


![計算 01](assets/calc01.png) ![計算 02](assets/calc03.png) ![計算 03](assets/calc02.png)

![計算 04](assets/calc04.png)

*UI 項目に関する以下の説明*

計算指標ビルダーが開いたら、次の操作を追加または実行します。

**A.** 計算指標の名前。 この名前は、指標コンポーネントのリストに表示されるので、自分や他のユーザーにとって明確な名前にします。例えば、 *コールセンター AOV*.

**B.** 計算指標の説明。 この説明は、ユーザーが&#x200B;**i**」を追加します。 例えば、コールセンター AOV の場合、 *コールセンターの注文支援に関する AOV を計算*.

**C.** 指標の形式：小数、時間、割合または通貨を選択し、小数点以下の桁数と極性を追加します。 ここで、 *形式の通貨、小数点以下の桁数の 0、および* ⬆ *極性には良い（緑）です。*

**D**. トピックを適用し、計算指標をすばやく見つけられるタグを使用している場合は、ここに適用するタグを追加します。 次を追加しました： *AOV* および *コールセンター* タグ。

**E.** このセクションは表示用です。セクション F で計算指標を作成する際に、数式がここに表示されます。

**金。** ここでは、ディメンション (H)、指標 (I) またはセグメント (J) をドラッグ&amp;ドロップして、計算指標および数式の演算子を作成します。 各指標について、歯車をクリックすると、指標タイプ（標準/合計）とアトリビューションモデルを変更できます。 *コールセンターの売上高をドラッグ&amp;ドロップし、その下にドロップします*÷ ￼*. デフォルトの指標タイプとアトリビューションモデルを受け入れます。*

**G**. 使用方法 **+追加** オプションを使用して、ここには必要ない条件や静的な数値を追加できます。

**K.** 最後に、計算を作成する際に、過去 90 日間のデータをここでプレビューできます。

コールセンター AOV を構築したので、オンライン AOV の計算指標も必要です。 これは、上記と同じ手順に従って行います。

次に、計算指標ビルダーを使用するか、フリーフォームテーブル内から直接、3 番目の計算指標を作成して、コールセンターとオンライン AOV を比較し、最終的に次のような計算指標を作成します。

![計算 05](assets/calc05.png)

この例では、買い物客がコールセンターを使用して購入を支援すると、大幅な上昇が見られます。 その後、このデータから、顧客がポップアップオファーやその他のガイド付きエクスペリエンスなどを通じて購入に関するサポートを得る方法に関する決定を通知できます。

## 計算指標でのセグメントの使用

次に、計算指標でセグメントを使用して、顧客の行動、好み、動機に関するより詳しいインサイトを得る方法を見てみましょう。 セグメントと計算指標を使用すると、エクスペリエンスを向上させ、売上高を増やし、顧客満足度と忠誠度を向上させるための、顧客に関する十分な情報を得ることができます。

上記の AOV の例では、コールセンターによる購入の支援により、通常、より高い AOV が使用されることが既にわかっています。 ただし、他の指標では、ほとんどのユーザーが購入時にコールセンターを使用していないことがわかります。

では、どの小売カテゴリ（およびこれらのカテゴリを通るユーザーパス）が最も高い AOV を生み出すのでしょうか。  セグメントと計算指標を組み合わせることで見つけ出すことができます。

そのためには、まず訪問レベルを作成する必要があります *含める* および *除外* 各製品カテゴリのセグメント。 含めるまたは除外する項目は、 **オプション** 歯車をコンテナの右隅に配置します。 初期設定は Include です。

![計算 06](assets/calc06.png) ![計算 07](assets/calc07.png)

これらのセグメントを作成したら、計算指標を作成して質問に対する回答を提供できます。 計算指標ビルダーを開き、次の操作を行います。

1. 新しく作成したセグメントを検索し、使用するセグメントを **定義** ボックス。 例えば、Kid&#39;s ではなく Women&#39;s と Men の両方のカテゴリを訪問したユーザーの AOV を作成する場合、次の 3 つのセグメントをその領域にドラッグ&amp;ドロップできます。 *女性用の*, *メンズを含む*、および *子を除外*. これをと呼びます。 *セグメントの積み重ね*.

   ![計算 09](assets/calc09.png) ![計算 08](assets/calc08.png)

1. 次に、 **オンライン売上高** 指標を同じコンテナに追加してから、 **オンライン注文**. コンテナは、演算の順序を決定する数式のように機能するので、コンテナ内の項目は後続のプロセスの前に処理されますが、この計算には複数のコンテナやプロセスはありません。
1. 2 つの指標の間の演算子を除算 (÷) に変更します。
1. 選択する **通貨** 形式として **0** 小数点以下の桁数 **上** 極性に関しては
1. 計算指標に名前を付け、説明を入力します。
1. 保存します。

完了すると、計算指標は次のようになります。

![計算 10](assets/calc10.png)

訪問者のカテゴリジャーニーの各組み合わせに対して積み重ねセグメントを使用した計算指標を作成し、データを見て学習内容を見てみましょう。 訪問中に女性と男性の両方のカテゴリを訪問するユーザーの AOV が最も高く、1 つのカテゴリの訪問者と比較すると、上昇率は大きくなります。

![計算 11](assets/calc11.png) ![計算 12](assets/calc12.png)

これを把握することで、ページのレイアウト、製品の配置、プロモーションメッセージを最適化して、チェックアウト前により多くの人々をこれらのカテゴリに入れることができます。

## 貴重だが、どこでも利用できない

**したがって、単純で複雑な計算指標も、アナリストにとって非常に役立ちます。**

ただし、これらの指標は、 [!DNL Adobe Analytics]. 以下では、計算指標を使用できません。

- Analysis Workspace のフォールアウト
- Analysis Workspace のコホート分析
- Data Warehouse
- リアルタイムレポート
- 現在のデータレポート
- [!DNL Analytics] （Target の場合）
- Report Builder

## 計算指標のベストプラクティス

価値のある計算指標がどの程度あるかを理解したので、それらを構築する際のベストプラクティスについて説明します。

1. **数式の構文を確認してください。** 数式の構文が正しいことと、 [!DNL Adobe Analytics] 構文を使用して、意味のある情報を取得できるようにします。
1. **操作の順序を確認します。** 入れ物は慎重に使用し、適切な数学的操作順に入れてください。
1. **データを二重にカウントしない**. 計算指標で使用する数式で同じデータが複数回カウントされないようにすることで、データの二重カウントを回避できます。 多くの場合、 *次を含む* および *除外* 条件を使用する必要があります。
1. **時間の精度を確認します。** 計算指標の時間の精度が、数式で使用されるソース指標と同じであることを確認します。
1. **正確なデータを使用：** 正確で信頼性の高いデータを計算に使用する場合にのみ、価値のある結果が得られます。

## カスタムセグメントのベストプラクティス

でセグメントを作成する場合 [!DNL Adobe Analytics]には、次のベストプラクティスを念頭に置いてください。

1. **簡単にしておけ。** セグメントの複雑さを防ぎます。 できるだけ簡単にして、正確性を確保するために必要な条件のみを使用します。
1. **適切なコンテナタイプを使用してください**. 誤った結果が得られないように、セグメント定義で正しいコンテナタイプ（訪問者、訪問またはヒット）を使用してください。
1. **データを二重にカウントしない**. 計算指標と同様に、セグメントで同じデータが複数回カウントされないようにします。 「含める」コンテナと「除外する」コンテナが役に立ちます。
   1. インクルードコンテナを使用する場合は、 *次を含む* *訪問のすべての内容* ヒットが訪問内の条件に一致する場合。
   1. 除外コンテナを使用すると、 *訪問のすべてのコンテンツを除外* ヒットが訪問内の条件に一致する場合。
1. **コンテナを適切にネストする**. 最も外側のコンテナを使用して、どのデータを含めるかを決定し、残りのデータにネストされたルールを適用します。 ネストされたルールが適用されると、セグメントフローはファネルとして機能し、後続のルールは最初のルールが除外したヒットには適用されません。
1. **データが最新であることを確認します。** 正確な結果を得るには、セグメント定義で正確で最新のデータを使用してください。
1. **セグメントをテストします。** セグメントを他のユーザーにリリースする前に、必ずセグメントをテストして、意図したとおりに動作することを確認してください。
1. **パフォーマンスを考慮します。** セグメントは、レポートの処理に時間がかかる場合があるので、作成時の影響を考慮してください。

## 重要な留意点

でのセグメントと計算指標の組み合わせ [!DNL Adobe Analytics] は、より堅牢で効果的なデータ分析を実現できます。 データを分離して分割し、比較のために計算を作成することで、マーケティングキャンペーンを最適化し、カスタマイズしたダッシュボードとレポートを作成するために使用できる、顧客の行動に関する深いインサイトを得ることができます。 ただし、計算指標は、 [!DNL Adobe Analytics]を参照し、ベストプラクティスに従って、正確で役に立つデータを取得するようにしてください。


## 作成者

このドキュメントの作成者：

![Debbie Kern](assets/calc13.jpeg)

**Debbie Kern**, senior [!DNL Adobe Analytics] Adswerve の管理者

![Adswerve](assets/calc14.png)