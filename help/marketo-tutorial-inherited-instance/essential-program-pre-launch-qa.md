---
title: 成功のための基本的なプログラムの事前起動の品質保証 QA プロセス
description: プログラムの開始前の QA プロセスを開発して、社内チームがより正確かつ効率的にプログラムを作成して開始できるようにする方法を説明します。
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
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '5444'
ht-degree: 2%

---

# 成功のための基本的なプログラムの事前起動の品質保証プロセス

のユーザーが [!DNL [!DNL Marketo Engage]] 管理者またはマーケティングオペレーションチームは、お客様に直面するミスを防ぐために、プログラムの設定を適切に確認することが重要です。 間違いを制限する方法に沿って間違いから学ぶことはできますが、それはスケーラブルなプロセスではありません。 ビルダーとパワーユーザー/レビュー担当者の間で、プログラムのプリローンチ品質保証 (QA) プロセスを設計および実行する方法を学び、時間の節約、エラーの防止、内部ユーザーのトレーニングをより迅速におこなえます。

このチュートリアルでは、[!DNL [!DNL Marketo Engage]] 管理者は、プログラムの開始前の QA プロセスを開発して、社内チームのスケールを支援できます。 プログラムの事前起動チェックリスト ( ソース： [!DNL Adobe] Marketoチャンピオン (2021)、 [Grace Brebner のブログ投稿](https://nation.marketo.com/t5/champion-program-blogs/the-ultimate-go-live-checklist/ba-p/245759)を例として使用し、主要な要素と要件を順を追って説明します。

## プログラムの事前起動 QA プロセスを設計する必要があるのはなぜですか？

[!DNL より新しい場合 [!DNL Marketo Engage]] に設定されている場合、プログラムを構築する際に何をチェックすべきか分からない場合があります。 季節の [!DNL] でも [!DNL Marketo Engage]] 管理者は、メモリに基づいてプログラムを確認することは危険です。 これは、プログラムの起動前のチェックリストが機能し始めたときです。 プログラムの QA プロセスをよりスムーズに進めるだけでなく、一般的な落とし穴を見つけるためのビルダーのトレーニングにも役立ちます。

* **時間節約：** 確立された QA プロセスがないと、最終的にはプログラムの構築プロセスに時間がかかり、マーケティングプログラムを市場に導くのに時間がかかります。 独自のプログラム起動前リストを設定し、内部ユーザーに QA プロセスに慣れてもらうと、QA プロセスを使用することで、プログラムの設定がより正確になります。
* **セルフイネーブルメント：** マーケティングチームが作成するプログラムに関連するチェックリストを調べると、社内ユーザーをトレーニングするための構造化されたカリキュラムが提供されます。 チェックリストを通じて自己レビューを行うたびに、筋肉の記憶を作り上げます。 経験豊富な [!DNL [!DNL Marketo Engage]] 管理者は他のユーザーのプログラムを確認し、チェックオフにするチェックリストを設定することで、一般的な落とし穴を見落とすのを防ぐことができます。

## プログラムのプレローンチ QA プロセスの設計を開始します。

### 手順 1:QA プロセスを通じて検討する

次の質問に答えて、QA プロセスを考えます。

* **レビュー担当者と承認者の役割を担えるのは誰ですか？**
より小規模な組織の場合、[!DNL [!DNL Marketo Engage]] 管理者は、マーケティングとマーケティングの運用のハイブリッドな役割を果たす場合があります。 ビルダー以外の [!DNL [!DNL Marketo Engage]] パワー・ユーザーがプログラムを監査することを検討します。 新しい目のペアは、問題を見つけるのに役立ちます。

* **作成者とレビュー担当者は、どのように共同作業し、メモと変更を文書化しますか？**
スプレッドシートで整理した状態、またはプロジェクト管理プラットフォーム内で整理した状態を維持できます。 以下のチェックリストを参照し、お客様の組織に最適な形式にテンプレートを変換します。 チームは、起動用にプログラムを作成およびレビューするたびに、単にテンプレートを複製することができます。

### 手順 2：プログラムのプレローンチを確認する

プログラムの事前起動チェックリスト行を 1 行ずつ調べて、プログラムの QA 範囲に慣れてください。

**覚えておくべき経験則：**

* このプログラムの起動前チェックリストは、1 つのサイズですべてを満たすように設計されていません。 関連するものを使用し、何を無視または削除し、組織のニーズに合わせてカスタマイズします。 また、チェックリストを分割して、プログラムの構築に関連する部分のみを使用することもできます。
* 要件を明確に定義します。 各要素の受け入れ条件を考慮し、オフラインテンプレートで編集します。

### 手順 3：内部チーム向けのガイドラインを作成する

プログラムのプレローンチチェックリストを使用し、より効率化されるまで QA プロセスを実行するためのガイドラインを、社内チーム向けに作成します。

次に例を示します。

* ビルダーは、チェックリストの下に移動したときに、プログラムの事前起動チェックリストを複製して、確認、メモ、および承認を行う必要があります。
* ある列で自己レビューを行い、レビュー担当者に、要件の横にある別の列でメモを文書化してもらいます。
* 「最終確認」セクションには、レビュー担当者のみが入力してもらいます。 このセクションでは、レビュー担当者に対して、QA プロセス全体で変更が正しく行われるかどうかを確認するために、いくつかのキーチェックを繰り返すように依頼します。

### 手順 4：定期的にチェックリストを再訪問する

チームがこの演習を数回実行する際に、欠落している項目や適用できない項目が存在する場合があります。 このチェックリスト（四半期など）を再訪問して、レビュー項目と受け入れ基準を更新し、プログラム QA プロセスを微調整します。

## サンプルテンプレート：プログラムの起動前チェックリスト {#pre-launch-checklist}

>[!NOTE]
>画面が小さい場合は、下のタブをスクロールして詳細を表示できます。

>[!BEGINTABS]

>[!TAB 主な詳細と計画]

| # | レビュー領域 | 質問する質問 | 例 | 受け入れ条件 | その他のリソース |
|---|---|---|---|---|---|
| 1 | **プログラムタイプ** | 適切ですか？ | エンゲージメントプログラムは論理的なものですか？ デフォルトの場合、それは論理的ですか？ | **はい：** <br>この質問に「はい」で答えられない場合は、プログラムの種類を変更する必要が生じる場合があります。 | [プログラムについて](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.html){target="_blank"} |
| 2 | **チャネル** | チャネルは適切ですか？ チャネルステップ/プログラムステータスは、プログラムの成功管理をサポートしていますか？ | ニュースレターとして設定した場合、これは意味を持ち、プログラムのステータスがプログラムの目的をサポートしていますか。それとも、既存の何かをねじりたいが、適切ではないものを作りたいと考えていますか。 | **はい：** <br>「はい」を使用してこの質問に回答できない場合は、チャネルを変更するか、[!DNL [!DNL Marketo Engage]] administrator | [プログラムチャネルの作成](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html){target="_blank"}<br><br> [チャネルについて](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags.html#channel){target="_blank"} |
| 3 | **プログラム命名規則** | これは、命名規則に従って正しく設定されていますか？ 命名規則ツールまたはスプレッドシート（存在する場合）にリンクします。 | 数式： [プログラムタイプ] - [日付] [カテゴリ]: [短い説明] | **はい：** <br>この質問に「はい」で答えられない場合や、確かでない場合は、命名規則を確認し、必要に応じてプログラムの名前を更新します。 | [新しいを整理するためのベストプラクティス [!DNL Marketo Engage] インスタンス](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/fundamentals/best-practices-to-organize-a-new-instance.html){target="_blank"} |
| 4 | **期間原価** | 期間原価タグをプログラムに割り当てましたか？ | 7 月に発売する eBook の制作に$1,000 を費やした場合、7 月には期間原価が 1,000 ドルになります。 | **はい：** <br>この質問に「はい」で回答できない場合は、ゼロでも期間原価を追加します。 | [プログラムでの期間原価の使用](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.html){target="_blank"} |
| 5 | **成功** | プログラムの目標と成功指標は特定されていますか？ プログラムの測定方法を知っていますか？ プログラムのステータスが変更されたとマークしていますか？ | 「チャット」チャネルの場合、ステータスの進行状況は「メンバー」、「エンゲージ済み」、「コンバート済み」の可能性があります。 | **はい：** <br>この質問に「はい」で回答できない場合は、キャンペーンが影響を及ぼしたかどうかを簡単に把握することはできません。 主な目的を特定し、7 日後に手動でリストをインポートした場合でも、それを測定する手段を提供します。 | [プログラムステータス](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.html#program-statuses){target="_blank"} |
| 6 | **オーディエンス** | プログラムのオーディエンスは特定されていますか？ |  | **はい：** <br>この質問に「はい」で答えられない場合は、送信する前に確認してください。 |  |
| 7 | **トークン** | 必要なプログラムトークンをすべて更新したか。 | ウェビナープログラムの場合、イベントの日付、イベントのタイトル、説明、カレンダーファイルなどを更新しているか。 | **該当するかどうか** <br>「はい」で答えられない場合や、該当するかどうかがわからない場合は、「トークン」タブを確認してください。 プログラムに更新が必要なローカルトークンが含まれているかどうかを確認する | [プログラム内のマイトークンについて](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.html){target="_blank"} |

>[!TAB Web パーソナライゼーションキャンペーン]

| # | レビュー領域 | 質問する質問 | 受け入れ条件 | その他のリソース |
|---|---|---|---|---|
| 1 | **デザイン** | デザインはブランドのガイドラインと一致していますか？ | **はい：** <br>「はい」で回答できない場合は、適切な理由が必要です。または、アセットを再設計する必要があります。 |
| 2 | **テスト** | デバイスをまたいでテストされているか。 ブラウザー？ レンダリングはクリーンと機能の両方に適していますか？ | **はい：** <br>「はい」を返さない場合は、デバイスとブラウザーをまたいでテストする必要があります。 |
| 3 | **データ** | キャンペーンにフォームがある場合、そのフォームはテスト済みですか？ すべてのトリガーは期待どおりに流れますか？ すべてのフォームフィールドが正確にマッピングされているか。 フィールドだけでなく、ユーザーレコードのアクティビティログを確認して、これを証明できますか？ | **はい：** <br>「はい」を入力できない場合は、このテストを実施してください。 | [フォームフィールドを非表示に設定する](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.html){target="_blank"}<br><br> [非表示のフォームフィールド値の設定](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/forms/form-fields/set-a-hidden-form-field-value.html){target="_blank"} |
| 4 | **トラッキング** | キャンペーンにフォームがある場合、送信元を追跡するために、非表示の UTM フィールドが配置されていますか。 これらはテスト済みですか？ | **はいまたはいいえ：** 「いいえ」と答えた場合は、どのソースからこのフォームに人を導いたかを追跡する能力が制限されていることを理解してください。 | [リファラーパラメーター](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/forms/form-fields/set-a-hidden-form-field-value.html#referrer-parameter){target="_blank"} |
| 5 | **GDPR/CASL コンプライアンス** | <li>フォームを使用してデータを取り込む場合、オプトインは企業ポリシーに準拠していますか。 <li>機能するプライバシーポリシーリンクを含む収集ステートメントを提供しているか。 | **はい：** <br>関連するコンプライアンス環境を理解する：この質問に「はい」で回答できない場合は、「プライバシーポリシー」セクションを更新して、準拠していることを確認する必要があります。 **不明な場合は、法務チームから適切なアドバイスを受けてください。** | [プライバシー管理](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/privacy-management.html){target="_blank"} |
| 6 | **Google [!DNL Analytics] 統合** | Web パーソナライゼーションとGoogleの統合 [!DNL Analytics]? | **はいまたはいいえ：**<br>「いいえ」と答えた場合は、Web パーソナライゼーションの影響を追跡する機能が制限されていることを理解します。 | [Googleでのパーソナライズされたリマーケティング](https://experienceleague.adobe.com/docs/marketo/using/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.html){target="_blank"} |
| 7 | **Web セグメント** | <li>セグメントは適切に選択されていますか。また、適切なドメインに適用されますか。 <li>セグメントがGoogleに送信されるかどうか [!DNL Analytics]? | **はい：** <br> 「はい」を入力できない場合は、更新する必要があります。 | [Web セグメント](https://experienceleague.adobe.com/docs/marketo/using/product-docs/web-personalization/using-web-segments/web-segments.html){target="_blank"}<br><br>[Find Web [!DNL Campaign]s that are Using a Specific Segment](https://experienceleague.adobe.com/docs/marketo/using/product-docs/web-personalization/using-web-segments/find-web-campaigns-that-are-using-a-specific-segment.html){target="_blank"} |

>[!TAB ランディングページ]

| # | レビュー領域 | 質問する質問 | 受け入れ条件 | その他のリソース |
|---|---|---|---|---|
| 1 | **デザイン** | デザインはブランドと一致していますか？ 適切なテンプレートを使用しているか。 | **はい：** <br> 「はい」で回答できない場合は、正しい理由が必要か、再設計する必要があります。 | [Marketoランディングページテンプレートの編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-templates/edit-a-marketo-landing-page-template.html){target="_blank"} |
| 2 | **テスト** | デバイスやブラウザーをまたいでテストされているか。 レンダリングはクリーンと機能の両方に適していますか？ | **はい：** <br>「はい」を返さない場合は、デバイスとブラウザーをまたいでプレビューリンクをテストする必要があります。 | [ランディングページのプレビュー](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/preview-a-landing-page.html){target="_blank"} |
| 3 | **URL** | ページ URL はカスタマイズされていますか？ これは論理的で、命名規則に従っていますか。 | **はい：** <br>「はい」を入力しても返信できない場合は、ページ URL を更新する必要があります。 | [ランディングページ URL の変更](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/change-the-landing-page-url.html){target="_blank"} |
| 4 | **Meta/OG タグ** | OG タグが設定されているか。 タイトル、説明、画像など。 これらは、ソーシャル共有でのページの表示に影響します。 | **はい：** <br>「はい」を入力できない場合は、すべてのタグを更新する必要があります。 | [ランディングページのタイトルとメタデータを編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/edit-landing-page-title-and-metadata.html){target="_blank"} |
| 5 | **ロボット** | 設定内容 彼らはあなたのニーズに合っていますか？ | **はい：** <br>「はい」で回答できない場合は、更新する必要があります。 | [ロボットとは何か？](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/edit-landing-page-title-and-metadata.html){target="_blank"} |
| 6 | **パーソナライゼーション** | ページにパーソナライズされた要素（動的コンテンツ、スニペットなど）が含まれている場合は、テスト済みですか？ すべて期待どおりに動作しているか。 | **はい/該当なし：** <br>「はい」または「いいえ」と答えられない場合は、テストに行ってください。 | [ランディングページでの動的コンテンツの使用](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/personalizing-landing-pages/use-dynamic-content-in-a-landing-page.html){target="_blank"}<br><br> [動的コンテンツを含むランディングページのプレビュー](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/preview-a-landing-page-with-dynamic-content.html){target="_blank"} |
| 7 | **画像** | 使用する画像はすべて正しく圧縮されていますか？ 画像をオーバーレイするテキストがある場合は、明確に読みやすいですか？ これらの画像を使用する権利はあり、ブランドに登録されていますか？ | **はい/該当なし：** <br> E メールの読み込み速度を向上させるには、すべての画像（使用されている場合）を圧縮する必要があります。 | [アップロードした画像またはファイルの置換](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/images-and-files/replace-an-uploaded-image-or-file.html){target="_blank"} |
| 8 | **コピー** | 文法の誤りがないかコピーを確認しましたか？ あなたのブランドの声のトーンのコピーですか？ あなたのコピーは、ページの目的を明確にしますか？ | **はい/該当なし：** <br> 「はい」または「いいえ」に回答できない場合は、コピーを確認します。 |
| 9 | **フォーム** | ランディングページにフォームが含まれている場合、正しいフォームが参照されているかどうか。 Marketo以外のランディングページを使用している場合は、フォームアセットページの埋め込みコードもチェックし、 [2023 年 8 月に廃止された旧 URL 構造](https://nation.marketo.com/t5/product-documents/upcoming-changes-to-design-studio-urls/ta-p/306632){target="_blank"}. | **はい/該当なし：** <br> 「はい」（または該当なし）と答えられない場合は、修正してください。 | [フォームを含むランディングページ](https://experienceleague.adobe.com/docs/marketo/using/getting-started-with-marketo/quick-wins/landing-page-with-a-form.html){target="_blank"}<br><br> [Web サイトにフォームを埋め込む](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.html){target="_blank"}<br><br>[デザインスタジオ URL の変更](https://nation.marketo.com/t5/product-documents/upcoming-changes-to-design-studio-urls/ta-p/306632)<br> |
| 10 | **ありがとうございます** | ページ上にフォームがある場合、ページには送信時に成功メッセージ/リダイレクトページが適切に表示されますか？ | **はい/該当なし：** <br> 「はい」と答えられない場合（または該当しない場合）は、投稿送信の設定を修正します。 | [ランディングページのリダイレクト](https://experienceleague.adobe.com/docs/marketo/using/getting-started-with-marketo/quick-wins/redirect-a-landing-page.html){target="_blank"} |
| 11 | **GDPR/CASL コンプライアンス** | フォームを通じてデータが取り込まれる場合、オプトインは準拠しており、プライバシーポリシーリンクが機能する収集文を提供しているか。 | **はい：** <br>関連するコンプライアンス環境を把握する：この質問に「はい」で答えられない場合は、準拠していることを確認するためにを更新する必要があります。 わからない場合は、適切なアドバイスを求めてください。 | [プライバシー管理](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/privacy-management.html){target="_blank"} |
| 12 | **トラッキング** | あるか [!DNL Google Analytics]、タグマネージャー、Munchkin の設定を意図したとおりにページに適用しますか？ このランディングページで Munchkins をデフォルトでオンまたはオフにしますか？ | **はい/該当なし：**<br>「はい」と答えられない場合や該当しない場合は、 [!DNL Marketo Engage] 管理者。 | [Munchkin コードが機能しているかどうかをテストする](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.html#test-if-your-munchkin-code-is-working){target="_blank"} |

>[!TAB フォーム]

| # | レビュー領域 | 質問する質問 | 受け入れ条件 | その他のリソース |
|---|---|---|---|---|
| 1 | **レスポンシブ** | フォームデバイスはレスポンシブですか？ | **はい：** <br>これを「はい」で回答できない場合は、CSS を更新してレスポンシブにする必要があります。そうしないと、パフォーマンスに影響を与える可能性があります。 |  |
| 2 | **デザイン** | フォームのデザインは一貫していますか？ | **はい：** <br>「はい」で回答できない場合は、正しい理由が必要です。または、CSS を更新してブランドにする必要があります。 |  |
| 3 | **データフロー** | すべてのデータは意図したとおりにフィールドにマッピングされますか？ テストレコードのアクティビティログを確認して、これを証明しましたか？ | **はい：** <br>「はい」を指定して応答できない場合は、マッピングを修正してテストする必要があります。 | [担当者のアクティビティログの検索](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.html){target="_blank"} |
| 4 | **トラッキング** | このフォームに対する送信ソースを追跡するために、非表示の UTM フィールドが配置されているか。 これらはテスト済みですか？ | **はいまたはいいえ：** <br>「いいえ」と答えた場合は、どのソースからこのフォームに人々を導いたかを追跡する能力が制限されていることを理解します。 | [フォームフィールドを非表示に設定する](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.html){target="_blank"}<br><br>[Set a Hidden Form Field Value](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/forms/form-fields/set-a-hidden-form-field-value.html){target="_blank"} |
| 5 | **GDPR/CASL コンプライアンス** | フォームを通じてデータが取り込まれる場合、オプトインは準拠しており、機能するプライバシーポリシーリンクを含む収集文を提供していますか？ | **はい：** <br>関連するコンプライアンス環境を把握する：この質問に「はい」で答えられない場合は、準拠していることを確認するためにを更新する必要があります。 **わからない場合は、適切なアドバイスを求めてください。** | [プライバシー管理](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/privacy-management.html){target="_blank"} |

>[!TAB スマートキャンペーン]

| # | レビュー領域 | 質問する質問 | 受け入れ条件 | その他のリソース |
|---|---|---|---|---|
| 1 | **精度** | 必要なスマートをすべて揃える [!DNL Campaign]がチェックされ、レビューされ、正確と見なされているか。 | **はい：** <br>「はい」を選択して答えられない場合は、先に進む前に修正して確認する必要があります。 | [スマート [!DNL Campaign] チェックリスト](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/smart-campaign-checklist.html){target="_blank"} |
| 2 | **送信数** | E メール送信キャンペーンがバッチキャンペーン（トリガーされない）の場合は、「スケジュール」タブでリード数を確認します。数字は期待どおりに揃えますか。 中止しきい値を下回っていますか？ | **はい：** <br>「はい」を選択して答えられない場合は、先に進む前に修正して確認する必要があります。 | [メールプログラムのスケジュール設定](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.html){target="_blank"} |
| 3 | **プライマリルール** | 適切な場合は主なセグメント化/リストを使用しているか、適切な場合はどちらですか。 | **該当するかどうか：**<br> プライマリリスト/セグメント化は、参照する必要のあるフィールドの数を減らし、ヒューマンエラーのリスクを減らすように設計されています。 プライマリリスト/セグメント化を使用しない場合は、ルールに自信を持つ必要があります。 |  |
| 4 | **アトリビューション** | プログラムが新しいリード（イベントプログラムなど）を取得している場合、必要に応じて属性設定が含まれますか？ 獲得プログラムはマッピングされていますか？ | **該当するかどうか：** <br>プログラムに担当者をインポートする場合、またはプログラムが新しい担当者を取得する場合は、獲得プログラムの設定を使用する必要があります。 |  |
| 5 | **エンゲージメントプログラム** | スマートが [!DNL Campaign] はエンゲージメントプログラムで使用され、必要に応じてメンバーが追加、一時停止、再開されるようにする手順はありますか？ これらの手順は他のユーザーによってレビューされていますか？ | **該当するかどうか：**<br> これがエンゲージメントプログラムで、正当な理由なしに「はい」を付けて回答できない場合は、これが設定されるまで有効にしないでください。 | [エンゲージメントプログラムに担当者を追加](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-people-to-an-engagement-program.html){target="_blank"} |
| 6 | **購読設定** | 必要なサブスクリプション設定要因がすべて含まれているか。 | **該当するかどうか：**<br> 不明な場合は、[!DNL [!DNL Marketo Engage]] 管理者。 該当なしに進むには、適切な理由が必要です（オペレーショナルの送信など）。 | [サブスクリプションセンターの設定および管理方法](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/subscription-center-watch.html){target="_blank"} |
| 7 | **プログラムステータス** | プログラムのステータスを更新するためのフローステップは含まれていますか？ | **はい：** <br>「はい」で回答できない場合は、スマートに追加する必要があります [!DNL Campaign] フローステップ。 | [プログラムステータスの変更](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.html){target="_blank"} |
| 8 | **より広い影響** | <li>他のチームやシステムと同期するフィールドにアラートや書き込みを送信するフローステップはありますか。 <li>その場合、ボリュームは考慮され、これらのチームやシステムに関する関係者に通知されていますか？ | **はい、いいえ、または適用不可：**<br> 答えは問題ありませんが、マップが表示された場合は、通常、システムを所有するチームに通知する必要があります。 不明な場合は、管理者に問い合わせてください。 |  |
| 9 | **スコアリングの影響** | リード/担当者スコアリングに何らかの影響を与えるかを検討しました。 | **該当するかどうか：** <br>「はい」と答えられない場合や該当しない場合は、管理者に問い合わせてください。 | [単純なスコア](https://experienceleague.adobe.com/docs/marketo/using/getting-started-with-marketo/quick-wins/simple-scoring.html){target="_blank"}<br><br>[How to build a lead scoring program](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/lead-scoring-watch.html){target="_blank"} |
| 10 | **収益サイクルモデラー (RCM) の影響** | 人物のライフサイクルモデルに何らかの影響を与えると考えられているか。 | **該当するかどうか：** 該当するコストやはいに回答できない場合は、管理者にお問い合わせください。 | [収益サイクルモデラー構成](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.html){target="_blank"} |
| 11 | **エンゲージメントプログラムに対する影響** | <li>既存のエンゲージメントプログラムに影響を及ぼすことは考えましたか？ <li>複数の通信が人々に衝撃を与えないように保証したか？ | **該当するかどうか：**<br>「はい」と答えられない場合や該当しない場合は、管理者に問い合わせてください。 | [重複するコンテンツの送信の回避](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/using-engagement-programs/avoid-sending-duplicate-content.html){target="_blank"} <br><br>[Apply Communication Limits to Smart [!DNL Campaign]](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/apply-communication-limits-to-smart-campaign.html){target="_blank"} |
| 12 | **レポート成功** | プログラムの成功は論理的に測定されていますか？ 成功は妥当なものです。プロセスの中であまりに近すぎないのですか。 達成するには遠すぎない？ 内部でのコミュニケーションを成功についてレポートし、測定する方法に関する戦略はありますか？ | **はい：** <br>「はい」と答えられない場合は、成功指標の定義を考え直します。 | [プログラムの変更成功](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-success.html){target="_blank"} |

>[!TAB リスト]

| # | レビュー領域 | 質問する質問 | 受け入れ条件 | その他のリソース |
|---|---|---|---|---|
| 1 | **ロジック** | スマートリストを使用してオーディエンスの一部を特定している場合、ロジックはチェック、レビューおよび正確と見なされていますか？ | **はい：** <br>「はい」で回答できない場合は、スマートリストの設定を修正し、先に進む前にこれらを確認してください。 |  |
| 2 | **インポートプロセスのリスト** | 静的リストを使用してオーディエンスの任意の部分を識別している場合、そのデータソースは信頼でき、リストの読み込みプロセスに従って正確に読み込みがおこなわれたか。 | **はい：** <br>「はい」を入力できない場合は、先に進む前にリストデータを修正し、これらを確認してください。 | [静的リストから人を追加/削除する方法](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/understanding-static-lists.html){target="_blank"}<br><br>[担当者のリストをインポート](https://experienceleague.adobe.com/docs/marketo/using/getting-started-with-marketo/quick-wins/import-a-list-of-people.html#step-import-your-spreadsheet-into-marketo) |
| 3 | **除外** | 必要な除外（競合相手、購読解除など）が含まれブロックリストに加えるるか。 | **該当するかどうか：** <br>非常に良い、法的に準拠している、そうでない理由がない限り、配信停止を除外する必要があります。 これらを含めない場合は、コンテンツ、キャンペーンルール、法的根拠に自信を持つ必要があります。 | [配信停止について](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html){target="_blank"}<br><br>[Change Data Value](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html){target="_blank"} |
| 4 | **プライマリリスト** | プライマリリスト/セグメント化は、適切な場所で使用されていますか。 | **該当するかどうか：** プライマリリスト/セグメント化は、参照する必要のあるフィールドの数を減らし、ヒューマンエラーのリスクを減らすように設計されています。 プライマリリスト/セグメント化を使用しない場合は、ルールに自信を持つ必要があります。 | [セグメントルールの定義](https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.html) |

>[!TAB オーディエンス]

| # | レビュー領域 | 質問する質問 | 受け入れ条件 | その他のリソース |
|---|---|---|---|---|
| 1 | **法的根拠：**<br>&#x200B;オーディエンスに問い合わせるための適切な法的根拠がある。 | <ul><li>**明示的：** ブランドからのマーケティングコムの受け取りを明示的にオプトインしているか。 </li><li>**推測される（準拠している場合）:** 連絡先の詳細をお知らせしており、この情報を使用して連絡を取ることを合理的に期待できますか？ </li><li>**見なす（準拠している場合）:** 公共のソースから連絡先の詳細を取得し、公共のソースから判断した場合、コンテンツが彼らに関連すると合理的に判断できるか。</li></ul> | **はい、基準を示します。** どのような基準を選択しても、コンプライアンス環境で有効であることを確認してください。 「はい」で回答できない場合は、プログラムの開始を控え、このオーディエンスに連絡する法的根拠に関する明確な説明を求めます。 | [プライバシー管理](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/privacy-management.html){target="_blank"} |
| 2 | **データソース** | インポートリストを通じてオーディエンスを特定した場合、データソースは信頼できますか？ | **該当するかどうか：**<br>「はい」で回答できない場合は、データソースに関する明確な説明を求めてください。 | [リストのインポートによるオーディエンスの定義](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/email-programs/managing-people-in-email-programs/define-an-audience-by-importing-a-list.html){target="_blank"} |
| 3 | **リスト購入** | オーディエンスは、リストの購入またはスポンサーシップ活動を通じて提供されていますか？ | **ソース=リスト購入の場合は、次のようになります。**<br> リストの購入は、悪いプラクティスであり、多くの場所で違法であり、多くの場合、マーケティングオートメーションプラットフォームとの契約違反です。<br><br>**はい、source = sponsorship の場合** <br>スポンサーシップと競合他社の場合は、データのキャプチャが準拠していることを確認します。 最初のコミュニケーションでは、情報の受け取り方を明確にし、人々に対して簡単にオプトアウトできるようにすることがベストプラクティスです。 |
| 4 | **関連度** | このオーディエンスを送信しようとしている情報は、オーディエンスに関連し、顧客との関係に関連しています。 | **はい：** <br>「はい」を使用して回答できない場合は、停止して、なぜこれらの担当者に E メールを送信するのかを慎重に検討してください。 顧客との関係に関係のない情報を送信すると、パフォーマンスや配信品質に悪影響を与える可能性があり、コンプライアンス環境に違反する可能性があります。 |
| 5 | **期待値** | この聴衆は、あなたからの連絡を期待しています。 | **はい：** <br>「はい」を使用して回答できない場合は、停止して、なぜこれらの担当者に E メールを送信するのかを慎重に検討してください。 不本意なオーディエンスに E メールを送信したり、今後連絡を受けたりすると、パフォーマンス、配信品質に悪影響を及ぼし、コンプライアンス環境に違反する可能性があります。 |


>[!TAB アセットを電子メールで送信]

| # | レビュー領域 | 質問する質問 | 受け入れ条件 | その他のリソース |
|---|---|---|---|---|
| 1 | **送信者の E メールアドレス** | ブランド所有者に確認し、E メールアドレスが安全に使用できることを確認しましたか？ | **はい：** <br>「はい」で回答できない場合は、先に進む前に送信者の E メールを確認する必要があります。 | [電子メールヘッダーを編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/creating-an-email/edit-your-email-header.html){target="_blank"}<br><br>[Change the Default From Email and From Label](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/change-the-default-from-email-and-from-label.html){target="_blank"} |
| 2 | **送信者名** | ブランド所有者に確認し、その名前が安全に使用できることを確認しましたか？ | **はい：** <br>「はい」を選択できない場合は、先に進む前に確認する必要があります。 | [電子メールヘッダーを編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/creating-an-email/edit-your-email-header.html){target="_blank"}<br><br>[Change the Default From Email and From Label](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/change-the-default-from-email-and-from-label.html){target="_blank"} |
| 3 | **返信先アドレス** | ブランド所有者に確認し、安全に使用できることを確認しましたか？ | **はい：** <br> 「はい」を選択できない場合は、先に進む前に確認する必要があります。 | [電子メールヘッダーを編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/creating-an-email/edit-your-email-header.html){target="_blank"} |
| 4 | **プリヘッダー設定** | ベストプラクティス ( 分 80 文字、全文、貴重なビットを前に読み込む？ | **はい：** <br><br>「はい」を入力できない場合は、先に進む前にを更新する必要があります。 | [電子メール設定](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.html){target="_blank"} |
| 5 | **校正のコピー** | スペルや文法に関する問題はありますか？ <br>そのトーンはブランドに合っていますか。 | **はい：** <br>「はい」を入力して返信できない場合は、修正してから先に進んでください。 |  |
| 6 | **スキャン性** | このメールのキー情報をスキャンで把握できますか？ | **該当するかどうか：** <br>電子メールのベストプラクティスは、スキャン時に電子メールの主要なメッセージを確実に理解できるようにすることが重要であることを示しています。 この方法を適用しない場合は、E メールのパフォーマンスに影響を与える可能性があることに注意してください。 |  |
| 7 | **配信停止** | このメールには、テスト済みの機能停止リンクがありますか？ | **該当するかどうか：**<br> E メールが次の場合にのみ有効である必要があります [操作](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.html){target="_blank"}. 配信停止は不要であることに自信を持ってください。不確かな場合は、配信を停止した方が安全です。 | [配信停止について](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html){target="_blank"} |  |
| 8 | **テキストバージョン** | <li>メールのテキスト版を作成しましたか？ <li>テキスト版のテストを自分に送ったか。 | **はい：**<br> 「はい」を入力できない場合は、先に進む前にテストを行ってください。 |
| 9 | **テキストバージョンの最適化** | <li>テキストバージョンのレイアウトは最適化されていますか？<li>何かのHTMLコメントが表示されますか？<li>関連するコンテンツはすべて含まれていますか？ | **はい：**<br> 自動生成されたテキストバージョンは、読み取るのが難しい場合があります。最適化する価値があります。 | [メールのテキストバージョンの編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/creating-an-email/edit-the-text-version-of-an-email.html){target="_blank"} |
| 10 | **テキストバージョンのハイパーリンクと UTMS** | ハイパーリンクは機能し、UTM を含めますか？ ：<ul><li>ヘッダーセクション</li><li>画像領域（含まれる場合）</li><li>本文</li><li>CTA</li>フッター</li></ul> | **はい：**<br> 「はい」を選択して答えられない場合は、先に進む前に修正して確認する必要があります。 自動テキストバージョンでは、変数を確実に引き抜くことはできません。 |  |
| 11 | **HTML/メインバージョン** | <li>E メールのHTML/メインバージョンを作成しているか。<li>試験を送ったのか？ | **はい（プレーンテキストのみの場合を除く）:**<br> 「はい」を選択して答えられない場合は、先に進む前にテストを送信する必要があります。 | [メールのHTMLの編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/edit-an-emails-html.html){target="_blank"} |
| 12 | **画像** | <li>すべての画像に代替テキストがありますか？ <li>壊れた画像はありますか？ | **該当するかどうか：**<br>. 「はい」を付けて答えられない場合は、修正して確認してから、先に進む必要があります（画像がない場合を除く）。 |  |
| 13 | **画像の圧縮** | <li>すべての画像は、画像編集ソフトウェアから Web 用に保存されましたか？ <li>アップロード前に圧縮されていましたか？ <li>E メールの読み込み時間は許容できますか？ | **該当するかどうか：**<br>&#x200B;読み込み速度を向上させるには、すべての画像（使用されている場合）を圧縮する必要があります。 | hero imagesは 120 KB 未満で、小さい画像はすべて小さくする必要があります。 負荷時間が長いと、パフォーマンスに影響します。 |
| 14 | **HTMLバージョンのハイパーリンクと UTM** | すべてのハイパーリンクが機能し、これらの領域に UTM が含まれているか。 ：<ul><li>ヘッダーセクション</li><li>画像領域（含まれる場合）</li><li>本文</li><li>CTA</li>フッター</li></ul> | **はい：**<br> 壊れたリンクを送信しない。 「はい」と答えられない場合は、修正してから先に進んでください。 |  |
| 15 | **動的コンテンツ** | <li>メールに動的コンテンツが含まれていますか？<li>複数のシナリオでテストしていますか？ | **はい：**<br> 「はい」を入力できない場合は、先に進む前にこのテストを行ってください。 | [E メールでの動的コンテンツの使用](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.html){target="_blank"}<br><br>[Preview an Email with Dynamic Content](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.html){target="_blank"} |
| 16 | **法的要件** | <ul><li>何か申し出を間違えておられましたか？</li><li>お客様のコンプライアンス環境に応じて、必要な免責事項が含まれているか。</li></ul> | **はい：**<br> 「はい」を選択して答えられない場合は、先に進む前に修正して確認する必要があります。 |  |
| 17 | **ピアの確認** | 別の [!DNL [!DNL Marketo Engage]] ユーザーピアがテストメールを確認しますか？ | **はい：**<br> 「はい」で回答できない場合は、送信前に実行する必要があります。 |  |
| 18 | **オペレーショナル送信** | <ul><li>電子メールをオペレーショナルに設定しているか（配信停止設定がスキップされます）?<li>その場合、その理由は何ですか？</li> | **はいまたはいいえ：**<br> 「はい」と回答した場合は、オペレーショナルメールとして送信する有効な理由が必要です。 不明な場合は、[!DNL [!DNL Marketo Engage]] 管理者。 | [メールを運用可能にする](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.html){target="_blank"} |
| 19 | **A/B と Champ/Challenger のテスト** | E メールでチャンピオン/挑戦者のテストを実行していますか？ | **はいまたはいいえ：**<br>&#x200B;テストをおこなっていない場合は、オーディエンスに関する詳細を学ぶ機会がない可能性があるかどうかを検討します。 | [A/B テストの作成](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/email-marketing/ab-testing-watch.html)<br><br>[メールチャンピオン/挑戦者の追加](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/email-tests-champion-challenger/add-an-email-champion-challenger.html){target="_blank"} |
| 20 | **クライアントテスト** | クライアントテストソフトウェアを通じてメールを実行しているか。<li>主要な E メールクライアントでの表示の問題を特定しているか。 <li>緊急度の低いテンプレート修正として修正またはログに記録されているか。 <li>読み込み速度の問題を特定し、改善を試みているか。<li>件名/プレビュー行の問題を特定したか。 解決したの？ | **該当するかどうか：**<br> 「はい」で回答できない場合（テスト用のソフトウェアを持っていない場合を除く）は、送信前にこの処理を行う必要があります。 | クライアントテストソフトウェアの例としては、Litmus や Email on Acid、 [Marketo E メール配信パワーパック](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/email-deliverability-power-pack-how-to-import-a-seed-list.html)<br><br>[インボックストラッカーTutorials](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/inbox-tracker/inbox-tracker-tutorials.html){target="_blank"} |
| 21 | **スパムテスト** | E メールをスパム処理で実行したか。<li>認知のためにブロックリストに加える掲げたの旗はありますか？<li>インボックスに配置/電子メールのクライアントフラグを特定しているか。 <li>潜在的な原因を探し求め、解決を試みたことはありますか？ | **該当するかどうか：**<br>「はい」で回答できない場合（テスト用のソフトウェアを持っていない場合を除く）は、送信前にこの処理を行う必要があります。 | 用途 [Marketoのインボックストラッカー機能](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/inbox-tracker/inbox-tracker-tutorials.html){target="_blank"} これは、契約に含まれている場合、または Litmus や Email on Acid などのツールに含まれている場合に使用します。 |
| 22 | **その他[!DNL Analytics]** | 電子メールには追加の分析コードが含まれていますか？ | **該当するかどうか：**<br>       「はい」で回答できない場合（追加の分析ソフトウェアがない場合を除く）は、送信前におこなう必要があります。 |

>[!TAB 最終チェック]

| # | レビュー | 質問する質問 | 受け入れ条件 |
|---|---|---|---|
| 1 | **アセットの承認** | 確定したプログラムアセットとチャンピオン/挑戦者のテストが完全に承認され、ドラフトモードで最終的な変更がないことを確認します。 | **はい：**<br> 「はい」で回答できない場合は、送信前に実行する必要があります。 |
| 2 | **スマート [!DNL Campaign] 精度** | スマートキャンペーンは適切なアセットを参照していますか？ | **はい：**<br> 「はい」で回答できない場合は、送信前にこの問題を修正する必要があります。 |
| 3 | **チェックリストの手順** | 上記のチェックがすべて完了しているか。 | **はい：**<br> 「はい」で回答できない場合は、送信前に実行する必要があります。 |
| 4 | **関係者の承認** | キャンペーンは、関係者から最終的な承認を受けましたか？ | **はい：**<br> 「はい」で回答できない場合は、送信前に実行する必要があります。 |

>[!ENDTABS]

## 次の手順

クリック [ここ](/help/marketo-tutorial-inherited-instance/_assets/downloads/[!DNL Adobe]_Marketo_Engage_Inherited_Instance_Program_Prelaunch_QA_Checklist.xlsx) を使用して、カスタマイズ可能なプログラムの起動前チェックリストをダウンロードします。 これは、組織のワークフローに合わせて調整する必要があります。 効果的な QA プロセスを開発すると、責任を問い、顧客に直面するミスを制限できます。

### 作成者

**グレースブレバーナー**
[!DNL Adobe] Marketoチャンピオン (2021)
*Director of Client Strategy, APAC Region, Digital Pi, LLC - A Merkle Company*

![グレースブレバーナー](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Grace_Brebner.png){width=30%}

**エイミーチウ**
*導入とリテンションマーケティングマネージャ[!DNL Adobe]*

![エイミーチウ](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width=30%}
