---
title: マーケター向けの  [!DNL Adobe] [!DNL Campaign] 成功のベストプラクティス 10 件
description: 役立つ 10 のベストプラクティスを学ぶ [!DNL Adobe] [!DNL Campaign] 実際の担当者は、デジタル消費者の変革を解き放ち、迅速化し、顧客にとってより優れたエクスペリエンスを提供します。
doc-type: article
solution: Campaign
feature-set: Campaign
feature: Personalization, [!DNL Campaign]s, Subscriptions, Deliverability
role: User
level: Beginner
jira: KT-11772
last-substantial-update: 2023-01-31T00:00:00Z
exl-id: add6ed84-892d-4901-9dd2-b0cba0c57290
source-git-commit: 7bbe86435c683f41509a8cbe6b117b354309644a
workflow-type: tm+mt
source-wordcount: '1276'
ht-degree: 81%

---

# [!DNL] のベストプラクティスの 10 個 [!DNL Adobe] [!DNL Campaign]] マーケター向け成功

クリスチャン・クリムチクは自称的なものです。[!DNL Adobe] 「Nerd」（7 年間 [!DNL） [!DNL Adobe] Experience Cloud] の専門知識（主に [!DNL] に焦点を当てたもの） [!DNL Adobe] [!DNL Campaign]]. As an [!DNL Adobe] 大規模な CPG 会社、Christian および彼のチームのプラットフォーム所有者は [!DNL [!DNL Campaign]] をクリックします。 厳しい規制要件と、ダイレクトメール、メール、SMS／MMS にわたるマルチチャネルの消費者マーケティングキャンペーンをシームレスに調整および管理します。

この記事では、クリスチャンは、助けるために彼のベストプラクティスを共有します [!DNL Adobe] [!DNL Campaign] 実際の担当者は、デジタル消費者の変革を解き放ち、迅速化し、顧客にとってより優れたエクスペリエンスを提供します。


## 1. 包括的でまとまりのあるマーケティングと配信計画の作成

[!DNL] を使用して成功を収めるための最初の手順 [!DNL Adobe] [!DNL Campaign]] は、ツールと顧客の期待を理解することです。これは、あらゆるタイプのマーケティングに当てはまります。 消費者に連絡するために使用するチャネルを明確に定義して理解し、それらのチャネルを使用するタイミングと理由を把握します。

[!DNL Adobe][!DNL Campaign] は、様々な方法で通信を実行および調整できる柔軟なツールです。[顧客の半数は、各購買ジャーニーで 3～5 つのチャネルを利用しています](https://www.mckinsey.com/capabilities/operations/our-insights/redefine-the-omnichannel-approach-focus-on-what-truly-matters)。したがって、これらのチャネルの使用方法を事前に理解し、計画を立てることは、プラットフォームの可能性を最大限に引き出し、顧客の共感を得るために重要です。

## 2. 顧客データの文書化と理解

<!-- Sandra, this paragraph opens as if it's going to discuss the advantages of segmentation, but it left me hanging. So, I hit the Hubspot link and dug into it a bit, and it seemed to me like the juicy information is this quote: 

"A study by Hubspot revealed that 30% of the marketers who participated in it used market segmentation techniques to improve email engagement. Segmented campaigns had 14.31% higher open rates and saw 101% more clicks than non-segmented campaigns.

"Email marketers who segmented their audience before campaigning stated that the revenue generated increased to up to 760%. Targeted and segmented emails bring in 58% of all revenue." [Link](https://www.notifyvisitors.com/blog/segmentation-statistics/) 

I added that second paragraph about 760% revenue and broke up the rest of the section, touched it up to help make the Hubspot example a little more impactful. If I altered this section too much, you can reject the change. It didn't have mistakes, but it felt like it didn't tie the segment example strongly enough to the point about data design. See if this is okay...-->

[Hubspot の調査](https://www.linkedin.com/pulse/customer-segmentation-effective-b2b-business-industry-sabreen)によると、セグメント化されたキャンペーンは、セグメント化されていないキャンペーンよりも開封率が 14.31％高く、クリック数が 101％増加しました。キャンペーンの前にオーディエンスをセグメント化したメールマーケターは、生成された収益が最大 760％増加したと述べています。

In [!DNL Adobe] [!DNL Campaign]を使用すると、セグメント化をすばやく簡単に調整できます。 ただし、このプロセスを合理化して促進するために、キャンペーンオペレーターとマーケティング担当者は、キャンペーンの作成と実行を設計およびリクエストする際に、基礎となるデータを文書化して理解する必要があります。 [!DNL] をサポートする管理者や開発者と提携する際には、現在のデータと、必要なデータを予測する方法を理解することが重要です [!DNL Campaign]] インスタンスに置き換えます。

キャンペーンは、それらをサポートする基礎となるデータ構造と同じくらい優れています。また、このデータ構造を把握して文書化することは、プラットフォームを統合したり、消費者データプラットフォームに移行したりする際に問題が発生した場合にも役立ちます

## 3. キャンペーンのタイミングの計画

顧客と同じように、日常生活があります。キャンペーンの送信とオーケストレーションは、このリズムに対応する必要があります。そうしないと、[送信メールの 85％が開封されず、送信メールの 98％がクリックスルーされない](https://www.validity.com/resource-center/state-of-email-2021/)ので、顧客に到達できない可能性があります。

例えば、顧客が朝に電話をチェックして最安値をチェックしている場合は、プロモーションのテキストメッセージを送信することを検討します。次のホットトレンドを夜にブラウジングしている場合は、無料配送のプロモコードを記載したフォローアップメールを送信することを検討します。また、[!DNL] のヒートマップツールを使用することも重要です [!DNL Campaign]] をクリックして、ワークフローと送信がいつ実行中かを追跡します。 複数のブランド間で通信を調整して促進することは、困難な場合があります。[メールのリズム、ケイデンス、タイミングを監視し、把握すること](https://experienceleaguecommunities.adobe.com/t5/adobe-campaign-classic-blogs/predictive-send-time-optimization-with-adobe-campaign/ba-p/561554?profile.language=ja)[!DNL Campaign]は、メッセージと インスタンスの全体的な安定性と強度にとって非常に重要です。

## 4.パーソナライゼーションを重要な場合に利用する

現在、消費者は受信するメッセージにある程度のパーソナライゼーションを期待しています。 [顧客の 80％は、パーソナライズされたエクスペリエンスを提供するブランドから購入する可能性が高くなります](https://us.epsilon.com/power-of-me)。件名にブランド名が入っているのもよいですが、パーソナライゼーションを使用すれば、さらに先に進むことができます。閲覧した製品を含めたり、類似の製品と関連付けたり、ブランドの包括的なエクスペリエンスやルックアンドフィールを強化し続けることができます。 すべてのビットがカウントされ、エンゲージメントとメッセージの開封率が促進されます。

## 5. クリエイティブアセットの健全な在庫を保有する

クリエイティブアセットは、効果的かつ円滑なキャンペーン配信エンジンの原動力です。消費者に届くのに成功すればするほど、またマーケティングプロセスを拡大して成熟させるほど、よりクリエイティブなコンテンツが必要になります。消費者は、これを期待しています。

いくら早くできたとしても、チームが設定できる次回の配信と同じ程度です。多くの場合、それには新しい魅力的なコンテンツが必要です。[!DNL [!DNL Adobe] [!DNL Campaign]] では、テンプレートの設定や、これらの配信の受信、準備が簡単におこなえます。 ただし、[Litmus のレポート](https://www.litmus.com/resources/state-of-email/)によると、マーケターの 58％が、1 つのメールキャンペーンを作成するのに 2 週間以上かかると述べているので、クリエイティブの健全なパイプラインを持つことが重要です。

## 6. 購読および環境設定の理解と管理

購読の環境設定の管理と維持は、すぐに複雑になり、様々なレベルのリスクを引き起こす可能性があります。顧客が応答しないチャネルを介して間違ったメッセージを送信した場合と同じように、10 人中 9 人の消費者は、否定的なエクスペリエンスがあると、将来そのブランドで買い物をする可能性が低くなると述べています。規模が大きくなると、規制やコンプライアンスに関するリスクや罰金にさらされる可能性があります。

[!DNL] のエキスパートによる使用を通じて、オプトインの管理と、進化し続けるこのエコシステムの育成に関する戦略を事前に策定 [!DNL Adobe] [!DNL Campaign]] やその他のマーケティングテクノロジーツール 多くの場合、これはキャンペーンの最大の成功指標の 1 つであるので、キャンペーン戦略が成長し、成熟するにつれて、慎重に計画することで計り知れない成果が得られます。

## 7. 配信品質の理解と計画

_配信品質_&#x200B;は、神秘的で複雑な概念のように思われることがよくあります。配信品質の重要な基本ルールは、戦略的計画です。IP アドレスをウォームアップし、優れたレピュテーションを構築するには時間がかかります。そのレピュテーションの低下は急速に発生する可能性があり、発生したダメージを改善することが困難になります。実際、**メールの 6 通のうち 1 通がインボックスに届いていません**。

配信品質の問題は、技術的な要因や、マーケティングに対する消費者の反応に基づく問題など、複数の要因によって発生する可能性があります。キャンペーンを作成して実行する際、および遡及プロセスで[配信品質](https://business.adobe.com/jp/products/campaign/email-deliverability.html)を念頭に置くことで、健全で安定した環境を維持し、顧客に対して引き続きポジティブなエクスペリエンスを提供できます。

## 8. キャンペーン遡及プロセスの計画と開発

キャンペーンの配信とオーケストレーションで多忙になると、達成したことを確認し、プロセスとキャンペーンのセグメント化を再評価することは、多くの場合、それ以上ではないにしても強力です。キャンペーン実行の規模と速度に応じて、2～4 週間ごとにキャンペーン遡及プロセスを開催します。

テンプレート化された一連の質問を作成すると、キャンペーンのリードタイム、クリエイティブ、または他の多くのトピックのセグメント化を改善する方法について、深く思慮深い会話を行うのに役立ちます。以前に実行した内容から学ぶ場合にのみ、改善してより速くなることがあります。

## 9. テストと反復

新しいことに挑戦する際、最初からうまくいくとは限りません。したがって、プロセスと戦術をテストして反復することが重要です。見込みのない、またはぴったりの顧客グループを試してみます。クリエイティブを切り替えます。新しいコールトゥアクションを試してみます。変更のための変更は生産的ではありませんが、時間の経過と共に多くの小規模で正確な実験を積み重ねることで、将来、ユーザーや顧客に大きな利益をもたらす可能性があります。

## 10. 可能な限り俊敏性を維持

マーケットは変化し続けており、これまでになく速いペースで動いています。競争力を維持し、高まる顧客の期待に応え続けるためには、キャンペーンチームが可能な限り身軽さと俊敏性を維持するよう推奨することが重要です。

[デジタルマーケティングリーダーの 35％は、最大の課題は組織内にあると考えています](https://www.gartner.com/en/newsroom/press-releases/gartner-says-35--of-digital-marketing-leaders-believe-the-bigges)。これを実現するには、いくつかのプラットフォームでクロストレーニングをおこない、データフローや構造などの理解を深めます [!DNL Adobe] ソリューションを作成し、キャンペーンのコンティンジェンシープランを作成します。 この考え方は様々な方法で実現できますが、短期的および長期的な成功を収めるには、アジャイルと計画に対する全体的なコミットメントが重要です。
