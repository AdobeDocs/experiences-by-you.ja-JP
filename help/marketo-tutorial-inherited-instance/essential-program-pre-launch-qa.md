---
title: 成功のための必須プログラム事前起動品質保証 QA プロセス
description: 社内チームがより正確かつ効率的にプログラムを作成および開始できるように、プログラムの事前起動用 QA プロセスを開発する方法について説明します。
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-13888
thumbnail: KT-13888.jpeg
hide: false
exl-id: c377fe5f-2d77-4fd0-9ac4-5ad65506f582
source-git-commit: b2e05ff39e065691dda530ed17762a55cf2e6778
workflow-type: tm+mt
source-wordcount: '4903'
ht-degree: 2%

---

# 成功に向けたプリローンチ品質保証プロセスの基本プログラム

次の場合： [!DNL Marketo Engage] 管理者、またはマーケティング運用チームは、お客様に直面するミスを避けるために、プログラム設定を適切に確認することが重要です。 ミスを減らす過程でミスから学ぶことはできますが、拡張性のあるプロセスではありません。 ビルダーとパワーユーザー/レビュー担当者の間でプログラムの起動前品質保証（QA）プロセスを設計および実行して、時間を節約し、エラーを防ぎ、内部ユーザーをより迅速にトレーニングする方法について説明します。

このチュートリアルでは、 [!DNL Marketo Engage] 管理者は、社内チームの規模を拡大できるように、プログラムの事前開始 QA プロセスを開発できます。 プログラム事前起動チェックリスト（ [!DNL Adobe] Marketo チャンピオン（2021）、 [Grace Brebner のブログ投稿](https://nation.marketo.com/t5/champion-program-blogs/the-ultimate-go-live-checklist/ba-p/245759)を例として、主要な要素と要件を順を追って説明します。

## ローンチ前の QA プロセスを設計する必要があるのはなぜですか。

次よりも新しい場合： [!DNL Marketo Engage]を使用すると、プログラムを構築する際に確認すべき内容がわからない場合があります。 季節的にも [!DNL Marketo Engage] 管理者、あなたの記憶に基づいてプログラムを見直すことは危険です。 このタイミングで、プログラムの起動前チェックリストが機能します。 プログラムの QA プロセスをスムーズに進めるだけでなく、ビルダーに対して一般的な落とし穴に気づくようトレーニングします。

* **時間節約：** 確立された QA プロセスを確立しないと、最終的にプログラムのビルドプロセスに時間がかかり、マーケティングプログラムを市場に投入する時間が長くなります。 独自のプログラムの事前起動リストを設定し、内部ユーザーが QA プロセスを理解すると、それを使用することで、プログラム設定の精度が向上します。
* **セルフイネーブルメント：** マーケティングチームが構築しているプログラムに関連するチェックリストを確認することにより、社内ユーザーをトレーニングする構造化されたカリキュラムが提供されます。 彼らがチェックリストを使って自己確認を行うたびに、それは彼らの筋肉メモリを構築します。 あなたが経験豊富であっても [!DNL Marketo Engage] 管理者は他のユーザーのプログラムを確認し、チェックリストをチェックできるようにすることで、一般的な落とし穴を見逃すのを防ぐことができます。

## プログラムの事前起動 QA プロセスの設計の基本を学びます。

### 手順 1:QA プロセスを検討する

QA プロセスを通じて考える際は、次の質問に回答してください。

* **レビュアーおよび承認者の役割を担えるのは誰ですか？**
より小さな組織の場合、 [!DNL Marketo Engage] 管理者は、マーケティング操作とマーケティング操作のハイブリッドな役割を果たす場合があります。 ビルダー以外のユーザーであることをお勧めします [!DNL Marketo Engage] パワーユーザーがプログラムを監査することを検討してください。 新しい視線を組み合わせることで、問題の発見に役立ちます。

* **ビルダーとレビュー担当者はどのように共同作業を行い、メモや変更をドキュメント化しますか？**
スプレッドシートやプロジェクト管理プラットフォーム内で整理しておくことができます。 以下のチェックリストを参照し、組織に最適な形式にテンプレートを変換します。 チームは、ローンチのプログラムを作成およびレビューするたびに、テンプレートをコピーするだけです。

### 手順 2：プログラムの事前起動を実行する

プログラムの事前起動チェックリストを行ごとに参照して、プログラムの QA 範囲を把握します。

**注意すべき経験則：**

* このプログラムの起動前チェックリストは、すべてに適合する 1 つのサイズではありません。 関係のあるものを使用し、関係のないものは無視または削除し、組織のニーズに合わせてカスタマイズします。 チェックリストを分割して、プログラムのビルドに関連する部分のみを使用することもできます。
* 要件を明確に定義します。 各要素の受け入れ条件を考慮して、オフラインテンプレートで編集します。

### 手順 3：社内チームのガイドラインを作成する

社内チームがプログラムのローンチ前チェックリストを使用するためのガイドラインを作成し、QA プロセスをより効率的に実行するまでテストを実施します。

次に例を示します。

* ビルダーは、チェックリストに従って確認、メモ、承認を行うために、プログラムの事前起動チェックリストをクローンする必要があります。
* ビルダーに、ある列でセルフレビューを行わせ、レビュー担当者に、要件の横にある別の列でメモをドキュメントしてもらいます。
* レビュー担当者のみが「最終確認」セクションに入力するようにします。 このセクションでは、QA プロセス全体を通して変更が適切に行われたことを確認するために、いくつかの主要なチェックを繰り返すようにレビュー担当者に指示します。

### 手順 4：定期的にチェックリストを再参照

チームがこの演習を数回実行するため、見つからない項目や適用されない項目がある場合があります。 このチェックリスト（四半期など）を参照して、レビュー項目と承認基準を更新し、プログラム QA プロセスを微調整してください。

## テンプレートの例：プログラム事前起動チェックリスト {#pre-launch-checklist}

>[!NOTE]
>画面が小さい場合は、下のタブをスクロールして詳細を確認できます。

>[!BEGINTABS]

>[!TAB 主な詳細と計画]

| # | レビュー領域 | 尋ねる質問 | 例 | 合格条件 | その他のリソース |
|---|---|---|---|---|---|
| 1 | **プログラムタイプ** | それは適切ですか？ | エンゲージメントプログラムの場合、それは論理的ですか？ デフォルトの場合、論理的ですか？ | **はい：** <br>この質問に「はい」と答えることができない場合は、プログラムの種類を変更する必要があります。 | [プログラムについて](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.html){target="_blank"} |
| 2 | **チャネル** | チャネルは適切ですか？ チャネルステップ/プログラムのステータスは、プログラムの成功管理をサポートしていますか？ | ニュースレターとして設定した場合、これは理にかなっていて、プログラムのステータスはプログラムの目的をサポートしていますか。それとも、既存のものを適切でないように歪めようとしていますか。 | **はい：** <br>この質問に「はい」で答えられない場合は、チャネルを変更するか、で新しいチャネルの作成について話し合う必要があります。 [!DNL Marketo Engage] 管理者 | [プログラムチャネルの作成](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html){target="_blank"}<br><br> [チャネルについて](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags.html#channel){target="_blank"} |
| 3 | **プログラム命名規則** | このセットは命名規則に従っていますか？ 命名規則ツールまたはスプレッドシートがある場合は、それにリンクします。 | 数式： [プログラムタイプ] - [日付] [カテゴリ]: [簡単な説明] | **はい：** <br>この質問に「はい」と答えることができない場合、または「確信がない」と答えられない場合は、命名規則を確認し、必要に応じてプログラム名を更新します。 | [新しいを整理するためのベストプラクティス [!DNL Marketo Engage] instance](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/fundamentals/best-practices-to-organize-a-new-instance.html){target="_blank"} |
| 4 | **期間コスト** | プログラムに期間原価タグを割り当てているか？ | 7 月に発売される eBook の作成に 1000 円を費やした場合、プログラムの期間コストは 7 月に 1000 円になります。 | **はい：** <br>この質問に「はい」と答えられない場合は、期間コストを（ゼロのみの場合でも）に追加します。 | [プログラムでの期間コストの使用](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.html){target="_blank"} |
| 5 | **成功** | プログラムの目標と成功指標は特定されていますか？ どうやってプログラムを測定するか知ってる？ プログラムのステータス変更をマークしましたか？ | 「チャット」チャネルの場合、ステータスの進行状況は、「メンバー」、「エンゲージメント」、「コンバート」になります。 | **はい：** <br>この質問に「はい」で答えることができない場合、キャンペーンが何らかの影響を与えたかどうかを簡単に理解することはできません。 主な目的を特定し、7 日後に手動でリストを読み込む場合でも、その目的を測定する手段を特定します。 | [プログラムのステータス](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.html#program-statuses){target="_blank"} |
| 6 | **オーディエンス** | プログラムのオーディエンスを特定しましたか？ |  | **はい：** <br>この質問に「はい」と答えられない場合は、送信を計画する前に確認してください。 |  |
| 7 | **トークン** | 必要なプログラムトークンをすべて更新しましたか？ | ウェビナープログラムの場合、イベントの日付、イベントのタイトル、説明、カレンダーファイルなどを更新しましたか？ | **はい/該当なし** <br>「はい」と答えることができない場合や、適用されるかどうかがわからない場合は、プログラムの「トークン」タブを確認してください。 更新が必要なローカルトークンがプログラムに含まれているかどうかを確認します | [プログラムのトークンについて](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.html){target="_blank"} |

>[!TAB Web パーソナライゼーションキャンペーン]

| # | レビュー領域 | 尋ねる質問 | 合格条件 | その他のリソース |
|---|---|---|---|---|
| 1 | **デザイン** | デザインはブランドガイドラインと一致していますか？ | **はい：** <br>「はい」を選択してもこれに回答できない場合は、正当な理由が必要であるか、アセットを再設計する必要があります。 |
| 2 | **テスト** | デバイス間でのテストは実施されていますか。 ブラウザーですか？ 両方ともクリーンにレンダリングし、機能しますか？ | **はい：** <br>「はい」と答えられない場合は、デバイスとブラウザーをまたいでこれをテストする必要があります。 |
| 3 | **データ** | キャンペーンにフォームがある場合、そのフォームはテストされていますか？ すべてのトリガーが期待どおりに流れますか？ すべてのフォームフィールドを正確にマッピングしますか？ フィールドだけでなく、人物レコードのアクティビティログを確認することで、これを証明できますか？ | **はい：** <br>「はい」と答えることができない場合は、これをテストする必要があります。 | [フォームフィールドを非表示に設定する](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.html){target="_blank"}<br><br> [非表示のフォームフィールド値を設定](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/forms/form-fields/set-a-hidden-form-field-value.html){target="_blank"} |
| 4 | **トラッキング** | キャンペーンにフォームがある場合、送信のソースを追跡するための非表示の UTM フィールドが用意されていますか？ これらはテスト済みですか。 | **はい/いいえ：** 「いいえ」を選択した場合は、このフォームに誘導されたソースを追跡する機能が制限されることを理解する必要があります。 | [リファラーパラメーター](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/forms/form-fields/set-a-hidden-form-field-value.html#referrer-parameter){target="_blank"} |
| 5 | **GDPR/CASL コンプライアンス** | <li>フォームを通じてデータが取り込まれた場合、オプトインは企業ポリシーに準拠していますか。 <li>機能するプライバシーポリシーリンクを含むコレクションのステートメントを提供しますか？ | **はい：** <br>関連するコンプライアンス環境を理解する：この質問に「はい」と回答できない場合は、「プライバシーポリシー」セクションを更新して、準拠していることを確認する必要があります。 **不明な場合は、法務チームに適切なアドバイスを求めてください。** | [プライバシーの管理](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/privacy-management.html){target="_blank"} |
| 6 | **Google [!DNL Analytics] 統合** | Web パーソナライゼーションとGoogleの統合 [!DNL Analytics]? | **はい/いいえ：**<br>「いいえ」と答えた場合は、web パーソナライゼーションの影響を追跡する機能は制限されていることを理解する必要があります。 | [Googleでのパーソナライズされたリマーケティング](https://experienceleague.adobe.com/docs/marketo/using/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.html){target="_blank"} |
| 7 | **Web セグメント** | <li>選択したセグメントは適切で、適切なドメインに適用されますか。 <li>Googleに送信されているセグメントです [!DNL Analytics]? | **はい：** <br> 「はい」と答えることができない場合は、更新する必要があります。 | [Web セグメント](https://experienceleague.adobe.com/docs/marketo/using/product-docs/web-personalization/using-web-segments/web-segments.html){target="_blank"}<br><br>[Web の検索 [!DNL Campaign]特定のセグメントを使用している](https://experienceleague.adobe.com/docs/marketo/using/product-docs/web-personalization/using-web-segments/find-web-campaigns-that-are-using-a-specific-segment.html){target="_blank"} |

>[!TAB ランディングページ]

| # | レビュー領域 | 尋ねる質問 | 合格条件 | その他のリソース |
|---|---|---|---|---|
| 1 | **デザイン** | デザインはブランドと整合性が取れているか。 適切なテンプレートを使用しているか。 | **はい：** <br> イエスと答えることができない場合は、正当な理由が必要であるか、再設計する必要があります。 | [Marketo ランディングページテンプレートの編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-templates/edit-a-marketo-landing-page-template.html){target="_blank"} |
| 2 | **テスト** | デバイスやブラウザーをまたいでテストされていますか。 両方ともクリーンにレンダリングし、機能しますか？ | **はい：** <br>「はい」と答えられない場合は、デバイスとブラウザーをまたいでプレビューリンクをテストする必要があります。 | [ランディングページのプレビュー](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/preview-a-landing-page.html){target="_blank"} |
| 3 | **URL** | ページ URL はカスタマイズされていますか？ これは論理的ですか。命名規則に従っていますか。 | **はい：** <br>「はい」と答えることができない場合は、ページ URL を更新する必要があります。 | [ランディングページ URL の変更](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/change-the-landing-page-url.html){target="_blank"} |
| 4 | **Meta/OG タグ** | OG タグは設定されていますか。 タイトル、説明、画像など。 これらは、ソーシャル共有でのページの表示方法に影響します。 | **はい：** <br>「はい」と答えることができない場合は、すべてのタグを更新する必要があります。 | [ランディングページのタイトルとメタデータの編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/edit-landing-page-title-and-metadata.html){target="_blank"} |
| 5 | **ロボット** | 設定は何ですか？ ニーズを考慮して意味をなしますか？ | **はい：** <br>「はい」と答えることができない場合は、更新する必要があります。 | [ロボットってどういう意味？](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/edit-landing-page-title-and-metadata.html){target="_blank"} |
| 6 | **パーソナライゼーション** | ページにパーソナライズされた要素（動的コンテンツ、スニペットなど）がある場合は、テストしましたか？ それらはすべて期待どおりに機能しますか？ | **はい/該当なし：** <br>「はい」または「いいえ」と答えられない場合は、テストに進んでください。 | [ランディングページでの動的コンテンツの使用](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/personalizing-landing-pages/use-dynamic-content-in-a-landing-page.html){target="_blank"}<br><br> [動的コンテンツを含むランディングページのプレビュー](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/preview-a-landing-page-with-dynamic-content.html){target="_blank"} |
| 7 | **画像** | 使用されるすべての画像が適切に圧縮されていますか。 画像にテキストがオーバーレイされている場合は、明確に読みやすいですか？ これらの画像を使用する権利はありますか？また、ブランドで使用していますか？ | **はい/該当なし：** <br> メールの読み込み速度を向上させるには、すべての画像（使用されている場合）を圧縮する必要があります。 | [アップロードした画像またはファイルの置換](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/images-and-files/replace-an-uploaded-image-or-file.html){target="_blank"} |
| 8 | **コピー** | そのコピーを読んで、文法の間違いがないか確認しましたか。 ブランドの声のトーンのコピーですか？ コピーを見れば、ページの目的が明確になりますか？ | **はい/該当なし：** <br> 「はい」または「いいえ」と答えることができない場合は、コピーを確認します。 |
| 9 | **フォーム** | ランディングページにフォームがある場合、正しいフォームが参照されているかどうかを確認します。 Marketo以外のランディングページを使用している場合は、フォームアセットページからも埋め込みコードを確認し、影響を受けないようにします [古い URL 構造は 2023 年 8 月に非推奨（廃止予定）となりました](https://nation.marketo.com/t5/product-documents/upcoming-changes-to-design-studio-urls/ta-p/306632){target="_blank"}. | **はい/該当なし：** <br> 「はい」（または「該当なし」）と答えることができない場合は、修正してください。 | [フォームのあるランディングページ](https://experienceleague.adobe.com/docs/marketo/using/getting-started-with-marketo/quick-wins/landing-page-with-a-form.html){target="_blank"}<br><br> [Web サイトへのフォームの埋め込み](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.html){target="_blank"}<br><br>[Design Studio の URL の変更](https://nation.marketo.com/t5/product-documents/upcoming-changes-to-design-studio-urls/ta-p/306632)<br> |
| 10 | **ありがとうございました** | ページにフォームがある場合、送信時に成功メッセージが表示されたり、「ありがとうございます」ページにリダイレクトされたりしますか？ | **はい/該当なし：** <br> 「はい」（または「該当なし」）と答えることができない場合は、送信後の設定を修正します。 | [ランディングページのリダイレクト](https://experienceleague.adobe.com/docs/marketo/using/getting-started-with-marketo/quick-wins/redirect-a-landing-page.html){target="_blank"} |
| 11 | **GDPR/CASL コンプライアンス** | フォームを通じてデータが取り込まれた場合、はオプトインに準拠していますか。また、プライバシーポリシーのリンクを使用してコレクションステートメントを提供していますか。 | **はい：** <br>関連するコンプライアンス環境を把握する：この質問に「はい」と答えられない場合、を更新して準拠していることを確認する必要があります。 わからない場合は、適切なアドバイスを求めてください。 | [プライバシーの管理](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/privacy-management.html){target="_blank"} |
| 12 | **トラッキング** | 持っていますか。 [!DNL Google Analytics]、タグマネージャー、Munchkin 設定のいずれかまたは両方を、意図したとおりにページに適用しますか？ このランディングページのマンチキンをデフォルトでオンまたはオフにしますか？ | **はい/該当なし：**<br>「はい」または「該当なし」と回答できない場合は、で確認してください [!DNL Marketo Engage] 管理者。 | [Munchkin コードが機能しているかどうかをテストします](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.html#test-if-your-munchkin-code-is-working){target="_blank"} |

>[!TAB フォーム]

| # | レビュー領域 | 尋ねる質問 | 合格条件 | その他のリソース |
|---|---|---|---|---|
| 1 | **レスポンシブ** | フォームデバイスはレスポンシブか | **はい：** <br>yes を返すことができない場合は、CSS を更新してレスポンシブにする必要があります。さもないと、パフォーマンスに影響が出る可能性があります。 |  |
| 2 | **デザイン** | フォームブランドのデザインは一貫していますか？ | **はい：** <br>「はい」を選択してもこれに回答できない場合は、正当な理由が必要であるか、CSS を更新してブランドで作成する必要があります。 |  |
| 3 | **データフロー** | すべてのデータが、意図したとおりにフィールドにマッピングされますか。 テストレコードのアクティビティログを確認して、これを証明しましたか？ | **はい：** <br>「はい」が返されない場合は、マッピングを修正してテストする必要があります。 | [個人のアクティビティログを見つける](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.html){target="_blank"} |
| 4 | **トラッキング** | このフォームへの送信のソースを追跡するために、非表示の UTM フィールドが配置されていますか？ これらはテスト済みですか。 | **はい/いいえ：** <br>「いいえ」と答えた場合は、このフォームに対するユーザーのダイレクトをトラッキングする機能が制限されていることを理解します。 | [フォームフィールドを非表示に設定する](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.html){target="_blank"}<br><br>[非表示のフォームフィールド値を設定](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/forms/form-fields/set-a-hidden-form-field-value.html){target="_blank"} |
| 5 | **GDPR/CASL コンプライアンス** | フォームを通じてデータが取り込まれた場合、はオプトインに準拠していますか。また、機能するプライバシーポリシーのリンクを含んだコレクションステートメントを提供していますか。 | **はい：** <br>関連するコンプライアンス環境を把握する：この質問に「はい」と答えられない場合、を更新して準拠していることを確認する必要があります。 **わからない場合は、適切なアドバイスを求めてください。** | [プライバシーの管理](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/privacy-management.html){target="_blank"} |

>[!TAB スマートキャンペーン]

| # | レビュー領域 | 尋ねる質問 | 合格条件 | その他のリソース |
|---|---|---|---|---|
| 1 | **精度** | 必要な機能がすべて揃っている [!DNL Campaign]チェック、レビュー、および正確と見なされましたか？ | **はい：** <br>「はい」と答えられない場合は、続行する前にこれらを修正して確認する必要があります。 | [スマート [!DNL Campaign] Checklist](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/smart-campaign-checklist.html){target="_blank"} |
| 2 | **送信数** | メール送信キャンペーンが（トリガーされていない）バッチキャンペーンの場合は、「スケジュール」タブでリード数を確認します。リード数は期待した数に調整されますか。 中止しきい値を下回っていますか。 | **はい：** <br>「はい」と答えられない場合は、続行する前にこれらを修正して確認する必要があります。 | [メールプログラムのスケジュール設定](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.html){target="_blank"} |
| 3 | **プライマリルール** | プライマリセグメント/リストは、適切な場合や適切な場合に使用されていますか？ | **はい、または該当なし：**<br> プライマリリスト/セグメント化は、参照する必要があるフィールドの数を減らし、人的エラーのリスクを軽減するように設計されています。 プライマリスト/セグメント化を使用しない場合は、ルールに自信を持っている必要があります。 |  |
| 4 | **アトリビューション** | プログラムが新しいリード（イベントプログラムなど）を取得する場合、必要に応じてアトリビューション設定は含まれますか？ 獲得プログラムはマッピングされていますか？ | **はい、または該当なし：** <br>ユーザーをプログラムにインポートする場合、またはプログラムが新しいユーザーを獲得する場合は、獲得プログラム設定を使用する必要があります。 |  |
| 5 | **エンゲージメントプログラム** | スマートな場合 [!DNL Campaign] はエンゲージメントプログラムで使用されています。メンバーの追加、一時停止、再開を適切に行うためのステップはありますか？ これらの手順は他のユーザーによってレビューされていますか？ | **はい、または該当なし：**<br> これがエンゲージメントプログラムで、正当な理由がなく「はい」で答えられない場合は、これが行われるまでアクティブ化しないでください。 | [エンゲージメントプログラムへのユーザーの追加](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-people-to-an-engagement-program.html){target="_blank"} |
| 6 | **購読設定** | 必要なサブスクリプション設定要因がすべて含まれていますか。 | **はい、または該当なし：**<br> よく分からない場合は、 [!DNL Marketo Engage] 管理者。 該当なし（運用上の送信など）で続行するには、正当な理由が必要です。 | [Subscription センターのセットアップおよび管理方法](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/subscription-center-watch.html){target="_blank"} |
| 7 | **プログラムステータス** | プログラムのステータスを更新するためのフローステップはありますか？ | **はい：** <br>「はい」と答えることができない場合は、スマートに追加する必要があります [!DNL Campaign] フローステップ。 | [プログラム状態の変更](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.html){target="_blank"} |
| 8 | **広範な影響** | <li>他のチームやシステムと同期するフィールドにアラートや書き込みを送信するフローステップはありますか？ <li>その場合は、ボリュームを考慮し、それらのチームやシステムの関係者にアドバイスしてもらっていますか。 | **はい、いいえ、該当なし：**<br> どんな答えでも問題ありませんが、マッピングされる場合は、通常、システムを所有するチームに通知する必要があります。 不明な場合は、管理者にお問い合わせください。 |  |
| 9 | **スコアリングの影響** | リード/人物スコアリングへの影響が考慮されていますか？ | **はい、または該当なし：** <br>「はい」または「該当なし」と回答できない場合は、管理者に問い合わせてください。 | [シンプルなスコアリング](https://experienceleague.adobe.com/docs/marketo/using/getting-started-with-marketo/quick-wins/simple-scoring.html){target="_blank"}<br><br>[リードスコアリングプログラムの作成方法](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/lead-scoring-watch.html){target="_blank"} |
| 10 | **収益サイクルモデラー（RCM）の影響** | 人物ライフサイクルモデルへの影響を考慮していますか？ | **はい、または該当なし：** 「はい」または「該当する」と答えることができない場合は、管理者に問い合わせてください。 | [収益サイクルモデラー設定](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.html){target="_blank"} |
| 11 | **エンゲージメントプログラムへの影響** | <li>既存のエンゲージメントプログラムへの影響を考慮しましたか？ <li>複数の通信による爆撃を受けないようにしましたか？ | **はい、または該当なし：**<br>「はい」または「該当なし」と回答できない場合は、管理者に問い合わせてください。 | [重複するコンテンツを送信しない](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/using-engagement-programs/avoid-sending-duplicate-content.html){target="_blank"} <br><br>[スマートへの通信制限の適用 [!DNL Campaign]](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/apply-communication-limits-to-smart-campaign.html){target="_blank"} |
| 12 | **成功のレポート** | プログラムの成功は論理的に測定されていますか？ 成功は合理的ですか？プロセスに近づきすぎませんか？ 達成するには遠すぎない？ 社内コミュニケーションの成功をレポートおよび測定する方法に関する戦略はありますか？ | **はい：** <br>「はい」と答えられない場合は、成功指標の定義を再考します。 | [プログラム変更の成功](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-success.html){target="_blank"} |

>[!TAB リスト]

| # | レビュー領域 | 尋ねる質問 | 合格条件 | その他のリソース |
|---|---|---|---|---|
| 1 | **ロジック** | スマートリストを使用してオーディエンスの一部を識別している場合、ロジックはチェック、レビューおよび正確と見なされていますか？ | **はい：** <br>「はい」と答えることができない場合は、スマートリストの設定を修正し、続行する前にこれらを確認する必要があります。 |  |
| 2 | **インポートプロセスのリスト** | 静的リストを使用してオーディエンスのいずれかの部分を識別している場合、データソースは信頼できるものであり、リストのインポートプロセスに従って正確にインポートされたでしょうか。 | **はい：** <br>「はい」と答えられない場合は、続行する前に、リストデータを修正して確認する必要があります。 | [静的リストからユーザーを追加/削除する方法](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/understanding-static-lists.html){target="_blank"}<br><br>[ユーザーのリストをインポート](https://experienceleague.adobe.com/docs/marketo/using/getting-started-with-marketo/quick-wins/import-a-list-of-people.html#step-import-your-spreadsheet-into-marketo) |
| 3 | **除外数** | ブロックリストに加える含まれている必要な除外（競合他社、登録解除など） | **はい、または該当なし：** <br>非常に優れた、法的に準拠している、そうしない理由がない限り、購読解除を除外する必要があります。 コンテンツ、キャンペーンルールおよび法的根拠が含まれていない場合は、これらを確実に理解する必要があります。 | [購読解除について](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html){target="_blank"}<br><br>[データ値を変更](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html){target="_blank"} |
| 4 | **プライマリリスト** | プライマリリスト/セグメント化は、必要に応じて使用されていますか？ | **はい、または該当なし：** プライマリリスト/セグメント化は、参照する必要があるフィールドの数を減らし、人的エラーのリスクを軽減するように設計されています。 プライマリスト/セグメント化を使用しない場合は、ルールに自信を持っている必要があります。 | [セグメントルールの定義](https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.html) |

>[!TAB オーディエンス]

| # | レビュー領域 | 尋ねる質問 | 合格条件 | その他のリソース |
|---|---|---|---|---|
| 1 | **法的根拠：**<br>&#x200B;オーディエンスに連絡するための適切な法的根拠があります。 | <ul><li>**明示的：** ブランドからのマーケティング通信の受信を明示的にオプトインしましたか？ </li><li>**推測（準拠している場合）:** 問い合わせ先の詳細情報を提供してもらったことがありますか？また、この情報を使用して問い合わせをする可能性は合理的にありますか？ </li><li>**見なされる（準拠している場合）:** 公開元から連絡先の詳細を取得しており、公開元を考慮して、コンテンツが彼らに関連すると合理的に仮定できますか？</li></ul> | **はい、根拠を述べます。** 選択した基準が、コンプライアンス環境で有効であることを確認してください。 イエスと答えることができない場合は、プログラムの立ち上げを延期し、このオーディエンスに連絡するための法的根拠について説明を求めます。 | [プライバシーの管理](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/privacy-management.html){target="_blank"} |
| 2 | **データソース** | インポートリストを使用してオーディエンスを識別した場合、データソースは信頼できますか？ | **はい、または該当なし：**<br> yes と答えることができない場合は、データソースに関する説明を求めます。 | [リストの読み込みによるオーディエンスの定義](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/email-programs/managing-people-in-email-programs/define-an-audience-by-importing-a-list.html){target="_blank"} |
| 3 | **リスト購入** | オーディエンスはリスト購入やスポンサーシップ活動を通じてソース化されていますか。 | **No if source = list purchasing:**<br> リスト購入は悪い方法であり、多くの場所で違法であり、多くの場合、マーケティング自動化プラットフォームとの契約に違反します。<br><br>**はい（ソース = スポンサーシップの場合）** <br>スポンサーシップおよび競争ケースでは、データキャプチャが準拠していることを確認します。 最初のコミュニケーションでは、どのように情報を受け取ったかを明確にし、人々がオプトアウトしやすくすることがベストプラクティスです。 |
| 4 | **関連度** | このオーディエンスに送信する情報は、オーディエンスや、オーディエンスとの関係に関連しています。 | **はい：** <br>「はい」と答えられない場合は、停止して、これらの人物にメールを送信する理由を慎重に検討します。 顧客や顧客との関係に関係のない情報を送信すると、パフォーマンスと配信品質に悪影響を与える可能性が高く、コンプライアンス環境に違反する可能性があります。 |
| 5 | **期待値** | このオーディエンスは、あなたからの連絡を期待しています。 | **はい：** <br>「はい」と答えられない場合は、停止して、これらの人物にメールを送信する理由を慎重に検討します。 オーディエンスが希望しない、または期待しない場合にメールを送信すると、パフォーマンスや配信品質に悪影響を及ぼす可能性が高く、コンプライアンス環境に違反する可能性があります。 |


>[!TAB メールアセット]

| # | レビュー領域 | 尋ねる質問 | 合格条件 | その他のリソース |
|---|---|---|---|---|
| 1 | **送信者のメールアドレス** | ブランドオーナーに確認し、メールアドレスが安全に使用できることを確認しましたか？ | **はい：** <br>「はい」と答えられない場合は、続行する前に送信者のメールを確認する必要があります。 | [メールヘッダーを編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/creating-an-email/edit-your-email-header.html){target="_blank"}<br><br>[デフォルトの「送信元メール」と「送信元ラベル」の変更](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/change-the-default-from-email-and-from-label.html){target="_blank"} |
| 2 | **送信者名** | ブランドオーナーに確認して、名前が安全に使用できることを確認しましたか？ | **はい：** <br>「はい」と答えられない場合は、続行する前に確認する必要があります。 | [メールヘッダーを編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/creating-an-email/edit-your-email-header.html){target="_blank"}<br><br>[デフォルトの「送信元メール」と「送信元ラベル」の変更](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/change-the-default-from-email-and-from-label.html){target="_blank"} |
| 3 | **返信先アドレス** | ブランドオーナーに確認して、安全に使用できることを確認しましたか？ | **はい：** <br> 「はい」と答えられない場合は、続行する前に確認する必要があります。 | [メールヘッダーを編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/creating-an-email/edit-your-email-header.html){target="_blank"} |
| 4 | **プリヘッダー設定** | ベストプラクティスに従ってプリヘッダーを設定していますか（例：min. 80 文字、完全な文、貴重なビットを前に読み込む）? | **はい：** <br><br>「はい」が返されない場合は、続行する前に更新する必要があります。 | [E メール設定](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.html){target="_blank"} |
| 5 | **プルーフのコピー** | スペルや文法の問題はありますか？ <br>トーンはブランドに適しているか？ | **はい：** <br>「はい」と答えられない場合は、続行する前に修正する必要があります。 |  |
| 6 | **スキャン性** | このメールの主な情報を一読して理解できますか。 | **はい、または該当なし：** <br>メールのベストプラクティスでは、メールの重要なメッセージをスキャンで確実に理解できることが重要であると示唆しています。 この方法を適用しない場合、メールのパフォーマンスに影響を与える可能性があることに注意してください。 |  |
| 7 | **購読解除** | メールには、テストした機能上の購読解除リンクがありますか？ | **はい、または該当なし：**<br>&#x200B;適用なしは、電子メールがの場合にのみ有効です [動作](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.html){target="_blank"}. 登録解除が必要ではないと確信してください。疑わしい場合は、包含が安全です。 | [購読解除について](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html){target="_blank"} |  |
| 8 | **テキストバージョン** | <li>メールのテキストバージョンを作成しましたか？ <li>テキスト版のテストを自分で送信しましたか？ | **はい：**<br> 「はい」と答えられない場合は、続行する前にテストする必要があります。 |
| 9 | **テキストバージョンの最適化** | <li>テキストバージョンのレイアウトは最適化されていますか？<li>HTMLコメントが表示されていますか。<li>関連するコンテンツがすべて含まれているか。 | **はい：**<br> 自動生成されたテキストバージョンは読みにくいことがあります。最適化する価値があります。 | [メールのテキストバージョンの編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/creating-an-email/edit-the-text-version-of-an-email.html){target="_blank"} |
| 10 | **テキスト バージョンのハイパーリンクと UTMS** | ハイパーリンクは機能し、これらの領域に UTM が含まれていますか？ ：<ul><li>ヘッダーセクション</li><li>画像領域（含まれる場合）</li><li>本文</li><li>CTA</li>フッター</li></ul> | **はい：**<br> 「はい」と答えられない場合は、続行する前にこれらを修正して確認する必要があります。 自動テキストバージョンでは、変数を確実に取り込めません。 |  |
| 11 | **HTML/メインバージョン** | <li>メールのHTML/メインバージョンを作成しましたか？<li>自分でテストを送信しましたか？ | **はい（プレーンテキストのみの場合を除く）:**<br> 「はい」と答えられない場合は、続行する前に自分でテストを送信する必要があります。 | [メールのHTMLの編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/edit-an-emails-html.html){target="_blank"} |
| 12 | **画像** | <li>すべての画像に代替テキストを使用できますか？ <li>壊れた画像はありますか？ | **はい、または該当なし：**<br>. 「はい」と答えられない場合は、続行する前にこれらを修正して確認する必要があります（画像がない場合を除く）。 |  |
| 13 | **画像圧縮** | <li>画像編集ソフトウェアから Web 用にすべての画像が保存されていますか？ <li>アップロードする前に圧縮されていましたか。 <li>メールの読み込み時間は許容されますか？ | **はい、または該当なし：**<br>&#x200B;読み込み速度を向上させるには、すべての画像（使用されている場合）を圧縮する必要があります。 | hero imagesは 120 KB 未満にし、小さい画像はすべて小さくする必要があります。 読み込み時間が長いと、パフォーマンスに影響します。 |
| 14 | **HTML版のハイパーリンクと UTM** | すべてのハイパーリンクが機能し、これらの領域に UTM が含まれていますか？ ：<ul><li>ヘッダーセクション</li><li>画像領域（含まれる場合）</li><li>本文</li><li>CTA</li>フッター</li></ul> | **はい：**<br> 壊れたリンクを送信しないでください。 「はい」と答えられない場合は、修正してから続行してください。 |  |
| 15 | **動的コンテンツ** | <li>メールには動的コンテンツが含まれていますか？<li>複数のシナリオでテストしましたか？ | **はい：**<br> 「はい」と答えられない場合は、続行する前にこれをテストする必要があります。 | [メールでの動的コンテンツの使用](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.html){target="_blank"}<br><br>[動的コンテンツを含むメールのプレビュー](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.html){target="_blank"} |
| 16 | **法的要件** | <ul><li>何かオファーを誤って伝えましたか？</li><li>コンプライアンス環境に従って、必要な免責事項は含まれていますか。</li></ul> | **はい：**<br> 「はい」と答えられない場合は、続行する前にこれらを修正して確認する必要があります。 |  |
| 17 | **Peer reviewed** | 別の薬を飲んだか [!DNL Marketo Engage] テストメールをピアレビューしますか？ | **はい：**<br> 「はい」と答えられない場合は、送信する前に行う必要があります。 |  |
| 18 | **運用上の送信** | <ul><li>メールを動作可能に設定しましたか（購読解除の設定をバイパスします）?<li>もしそうなら、あなたはこれに対する正当な理由があるのですか？</li> | **はい/いいえ：**<br> 「はい」と答えた場合は、運用用メールとして送信する有効な理由が必要です。 よく分からない場合は、 [!DNL Marketo Engage] 管理者。 | [メールを運用可能にする](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.html){target="_blank"} |
| 19 | **A/B および Champ/Challenger テスト** | メールでチャンピオン/チャレンジャーのテストを実行していますか？ | **はい/いいえ：**<br>&#x200B;テストを行っていない場合は、オーディエンスについて詳しく知る機会を逃していないかどうかを考えてみてください。 | [A/B テストの作成](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/email-marketing/ab-testing-watch.html)<br><br>[メールチャンピオン/挑戦者の追加](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/email-tests-champion-challenger/add-an-email-champion-challenger.html){target="_blank"} |
| 20 | **クライアントテスト** | クライアントテストソフトウェアを使用してメールを実行しましたか？<li>主要なメールクライアントの表示に関する問題を特定しましたか？ <li>緊急ではないテンプレート修正として修正またはログ記録しましたか？ <li>読み込み速度の問題を特定し、改善を試みましたか？<li>件名行/プレビュー行の問題を特定しましたか？ 解決したか？ | **はい、または該当なし：**<br> 「はい」と答えられない場合（テストソフトウェアがない場合を除く）は、送信する前に行う必要があります。 | クライアントテストソフトウェアの例としては、Litmus や Email on Acid などがあります。 [Marketo メール配信品質パワーパック](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/email-deliverability-power-pack-how-to-import-a-seed-list.html)<br><br>[インボックストラッカーTutorials](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/inbox-tracker/inbox-tracker-tutorials.html){target="_blank"} |
| 21 | **スパムテスト** | スパムメール処理を実行しましたか？<li>意識を高めるために掲げられたブロックリストへの登録の旗はありますか？<li>インボックスのプレースメント/メールクライアントフラグを特定していますか？ <li>潜在的な原因を探して解決しようとしましたか？ | **はい、または該当なし：**<br>「はい」と答えられない場合（テストソフトウェアがない場合を除く）は、送信する前に行う必要があります。 | 使用方法 [Marketo インボックストラッカー機能](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/inbox-tracker/inbox-tracker-tutorials.html){target="_blank"} この機能は、契約に含まれている場合や、Litmus や Email on Acid などのツールに含まれている場合に使用します。 |
| 22 | **追加[!DNL Analytics]** | メールには、追加の分析コードが含まれていますか？ | **はい、または該当なし：**<br>       「はい」と答えられない場合は（追加の分析ソフトウェアがない場合を除く）、送信する前に行う必要があります。 |

>[!TAB 最終チェック]

| # | レビュー | 尋ねる質問 | 合格条件 |
|---|---|---|---|
| 1 | **アセットの承認** | 完成したプログラムアセットとチャンピオン/挑戦者テストが完全に承認され、ドラフトモードで最終的に変更されないことを確認します。 | **はい：**<br> 「はい」と答えられない場合は、送信する前に行う必要があります。 |
| 2 | **スマート [!DNL Campaign] 精度** | スマートキャンペーンは適切なアセットを参照しますか？ | **はい：**<br> yes と答えることができない場合は、送信する前に修正する必要があります。 |
| 3 | **チェックリストの手順** | 上記のチェックはすべて完了していますか。 | **はい：**<br> 「はい」と答えられない場合は、送信する前に行う必要があります。 |
| 4 | **関係者の承認** | キャンペーンは関係者から最終的な承認を受けていますか？ | **はい：**<br> 「はい」と答えられない場合は、送信する前に行う必要があります。 |

>[!ENDTABS]

## 次の手順

クリック [こちら]（/help/marketo-tutorial-inherited-instance/_assets/downloads/[!DNL Adobe]_Marketo_Engage_Inherited_Instance_Program_Prelaunch_QA_Checklist.xlsx）を参照して、編集可能なプログラムをダウンロードし、カスタマイズします。 これは、組織のワークフローに合わせて調整する必要があります。 効果的な QA プロセスを開発することで、責任を負い、顧客に対するミスを制限できます。

### 作成者

**グレース ブレブナー**
[!DNL Adobe] Marketo チャンピオン （2021）
*Client Strategy, APAC Region, Digital Pi, LLC のDirector - Merkle 株式会社*

![グレース ブレブナー](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Grace_Brebner.png){width=30%}

**エイミー・チウ**
*導入およびリテンション・マーケティング・マネージャ[!DNL Adobe]*

![エイミー・チウ](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width=30%}
