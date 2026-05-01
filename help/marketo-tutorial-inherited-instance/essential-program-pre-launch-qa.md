---
title: AssuranceのQA プロセスを成功に導くための基本的なプログラムの導入前
description: 社内チームがより正確かつ効率的にプログラムを構築してローンチできるように、プログラムのローンチ前のQA プロセスを開発する方法を説明します。
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-13888
thumbnail: KT-13888.jpeg
exl-id: c377fe5f-2d77-4fd0-9ac4-5ad65506f582
source-git-commit: d78210c6d6f5ec22430770c752495959303a9519
workflow-type: tm+mt
source-wordcount: '6045'
ht-degree: 2%

---

# 成功のための基本的なプログラム立ち上げ前の品質保証プロセス

[!DNL Marketo Engage]管理者またはマーケティング運用チームのメンバーである場合は、顧客が直面する間違いを避けるために、プログラムの設定を適切に確認することが重要です。 失敗から学び、ミスを制限することもできますが、それは拡張可能なプロセスではありません。 ビルダーとパワーユーザー/レビューアーの間でプログラムの起動前の品質保証（QA）プロセスを設計および実行する方法を学ぶことで、時間を節約し、エラーを防ぎ、内部ユーザーをより迅速にトレーニングできます。

このチュートリアルでは、[!DNL Marketo Engage]管理者がプログラムの起動前のQA プロセスを開発して、社内チームの拡張を支援する方法について説明します。 [!DNL Adobe]Marketo Champion （2021）の[Grace Brebner氏のブログ記事](https://nation.marketo.com/t5/champion-program-blogs/the-ultimate-go-live-checklist/ba-p/245759)から入手したプログラム事前起動チェックリストは、主要な要素と要件を説明する例として使用されています。

## なぜ、プログラムを立ち上げる前にQA プロセスを設計する必要があるのですか？

[!DNL Marketo Engage]より新しい場合は、プログラムの作成時に何を確認すればよいかわからない場合があります。 季節的な[!DNL Marketo Engage]管理者であっても、メモリに基づいてプログラムを確認することはリスクがあります。 そこで、ローンチ前のプログラムのチェックリストを出番です。 プログラムのQA プロセスをよりスムーズに進めることができるだけでなく、ビルダーが陥りやすい落とし穴を見逃さないように訓練することもできます。

* **時間節約：**&#x200B;確立されたQA プロセスを確立していない場合、最終的にプログラム構築プロセスに時間を追加し、マーケティングプログラムを市場に投入するのにより多くの時間を要します。 独自のプログラム事前起動リストを設定し、社内ユーザーにQA プロセスを理解してもらうことで、プログラム設定の精度が向上します。
* **自己啓発：** マーケティング部門が構築しているプログラムに関連するチェックリストを通過できるようにすることで、社内ユーザーをトレーニングするための構造化されたカリキュラムを提供します。 チェックリストを通してセルフレビューを実行するたびに、筋肉の記憶が蓄積されます。 経験豊富な[!DNL Marketo Engage]管理者が他のユーザーのプログラムを確認している場合でも、チェックリストを作成して確認すれば、よくある落とし穴を見落とさないようにすることができます。

## プログラムの起動前のQA プロセスの設計を開始します。

### ステップ 1:QA プロセスについて考える

次の質問に答えて、QA プロセスについて考えてみましょう。

* **審査担当者と承認者の役割を果たすことができるのは誰ですか？**
小規模な組織の場合、[!DNL Marketo Engage]人の管理者は、マーケティングとマーケティング業務のハイブリッドの役割を果たすことができます。 ビルダー以外の[!DNL Marketo Engage]を使用することをお勧めします。パワーユーザーがプログラムを監査することを検討してください。 新しい新鮮な目のペアは、問題を見つけるのに役立ちます。

* **作成者とレビュー担当者はどのように共同作業を行い、メモや変更点を文書化しますか？**
スプレッドシートやプロジェクト管理プラットフォームで整理しておくことができます。 以下のチェックリストを参照し、自社に最適な形式にテンプレートを変換してください。 チームは、プログラムを構築およびレビューするたびにテンプレートを複製して起動できます。

### ステップ 2：プログラムの事前起動を実行する

プログラムのQA範囲を理解するために、プログラムの起動前のチェックリストを行ごとに確認します。

**考慮すべき経験則：**

* このローンチ前のチェックリストは、万人に合うように設計されていません。 関連性の高いコンテンツを使用し、そうでないコンテンツを無視または削除して、組織のニーズに合わせてカスタマイズできます。 また、チェックリストを分割し、プログラムの構築に関連する部分のみを使用することもできます。
* 要件の明確な定義。 各要素の承認基準を検討し、オフラインテンプレートで編集します。

### ステップ 3：社内チームのガイドラインを策定する

社内チームがプログラムの起動前のチェックリストを使用するためのガイドラインを策定し、より合理的になるまでQA プロセスをテストして実行します。

例を次に示します。

* ビルダーは、プログラムの起動前のチェックリストを複製して、チェックリストを確認、メモ、承認する必要があります。
* ビルダーに1列でセルフレビューを実施させ、レビュー担当者に要件の横にある別の列にメモを文書化させます。
* レビュー担当者のみが「最終チェック」セクションに入力します。 このセクションでは、レビュー担当者に対して、QA プロセス全体を通じて変更が適切に行われることを確認するために、いくつかの重要なチェックを繰り返すように求めます。

### ステップ 4：定期的にチェックリストを見直す

チームがこの演習を数回実行する際に、欠落しているか適用できない項目がある可能性があります。 このチェックリスト（四半期など）を見直して、レビュー項目と承認基準を更新し、プログラムのQA プロセスを調整します。

## テンプレートの例：プログラム導入前のチェックリスト {#pre-launch-checklist}

>[!NOTE]
>小さい画面の場合は、下のタブをスクロールしてさらに表示できることに注意してください。

>[!BEGINTABS]

>[!TAB  キーの詳細と計画]

| # | レビューエリア | ベンダーへの質問 | 例 | 受け入れ基準 | その他のリソース |
|---|---|---|---|---|---|
| 1 | **プログラムの種類** | 適切か？ | エンゲージメントプログラムは論理的ですか？ デフォルトの場合、それは論理的ですか？ | **はい：** <br>この質問に「はい」で回答できない場合は、プログラムの種類を変更する必要がある場合があります。 | [&#x200B; プログラムについて](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.html?lang=ja){target="_blank"} |
| 2 | **チャネル** | チャネルは適切か？ チャネルの手順/プログラムのステータスは、プログラムのサクセス管理をサポートしていますか？ | ニュースレターとして設定された場合、これは意味があり、プログラムのステータスがプログラムの目的をサポートしているか、既存のものをねじって適切ではないものを作成しようとしていますか？ | **はい：** <br>この質問に「はい」で回答できない場合は、チャネルを変更するか、新しいチャネルの作成について[!DNL Marketo Engage]管理者と話し合う必要があります | [&#x200B; プログラムチャネルの作成](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html?lang=ja){target="_blank"}<br><br> [&#x200B; チャネルについて](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags.html?lang=ja#channel){target="_blank"} |
| 3 | **プログラム命名規則** | これは、命名規則に従って設定されていますか？ 命名規則ツールまたはスプレッドシートがある場合は、そのツールまたはスプレッドシートにリンクします。 | 式：[ プログラムタイプ ] - [日付] [ カテゴリ ]: [簡単な説明] | **はい：** <br>この質問に「はい」で回答できない場合、または不明な場合は、命名規則を確認し、必要に応じてプログラムの名前を更新してください。 | [新しい [!DNL Marketo Engage]  インスタンスを整理するためのベストプラクティス &#x200B;](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/fundamentals/best-practices-to-organize-a-new-instance.html?lang=ja){target="_blank"} |
| 4 | **期間原価** | プログラムに「期間原価」タグを割り当てましたか？ | 7月に発売される電子書籍を作成するために1000 ドルを費やした場合、プログラムのコストは7月に1000 ドルとなります。 | **はい：** <br>この質問に「はい」で回答できない場合は、期間コストを追加します。期間コストはゼロの場合でも追加できます。 | [&#x200B; プログラムでの期間コストの使用](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.html?lang=ja){target="_blank"} |
| 5 | **成功** | プログラムの目的と成功指標を特定しましたか？ プログラムの測定方法を知っていますか？ プログラムステータスの変更など？ | 「チャット」チャネルの場合、ステータスの昇格は、「メンバー」、「エンゲージメント」、「コンバージョン」になる可能性があります。 | **はい：** <br>この質問に「はい」で回答できない場合、キャンペーンが影響を与えたかどうかを簡単に把握することはできません。 主要な目標を特定し、その目標を測定する方法を決定します。7日後に手作業でリストをインポートする場合でも同様です。 | [&#x200B; プログラムのステータス &#x200B;](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.html?lang=ja#program-statuses){target="_blank"} |
| 6 | **オーディエンス** | プログラムのオーディエンスを特定しましたか？ |  | **はい：** <br>この質問に「はい」で回答できない場合は、送信する前に確認してください。 |  |
| 7 | **トークン** | 必要なプログラムトークンをすべて更新しましたか？ | ウェビナープログラムの場合、イベントの日付、イベントのタイトル、説明、カレンダーファイルなどを更新しましたか？ | **はい/該当しない** <br>はい/回答できない場合、または該当するかどうかわからない場合は、プログラムの「トークン」タブを確認してください。 更新が必要なローカルトークンがプログラムに含まれているかどうかを確認します | [&#x200B; プログラムのトークンについて](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.html?lang=ja){target="_blank"} |

>[!TAB Web Personalization キャンペーン ]

| # | レビューエリア | ベンダーへの質問 | 受け入れ基準 | その他のリソース |
|---|---|---|---|---|
| 1 | **デザイン** | デザインはブランドガイドラインと一致していますか？ | **はい：** <br>この質問に「はい」で回答できない場合は、その理由が必要か、アセットを再設計する必要があります。 |  |
| 2 | **テスト** | デバイス間でテストされているか？ ブラウザーは？ 果たして両方ともクリーンに機能しているのだろうか。 | **はい：** <br>はい付きで回答できない場合は、デバイスとブラウザーでテストする必要があります。 |  |
| 3 | **データ** | キャンペーンにフォームがある場合、フォームはテストされていますか？ すべてのトリガーは期待どおりに流れますか？ すべてのフォームフィールドを正確にマッピングできるか？ フィールドだけでなく、個人レコードのアクティビティログを確認して、これを証明できますか？ | **はい：** <br>はい付きで回答できない場合は、テストする必要があります。 | [&#x200B; フォームフィールドを非表示に設定](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.html?lang=ja){target="_blank"}<br><br> [非表示フォームフィールド値を設定](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/forms/form-fields/set-a-hidden-form-field-value.html?lang=ja){target="_blank"} |
| 4 | **トラッキング** | キャンペーンにフォームがある場合、送信のソースを追跡するための非表示のUTM フィールドが配置されていますか？ これらはテストされていますか？ | **はい、またはいいえ：**&#x200B;いいえ回答した場合は、このフォームにユーザーを送信したソースを追跡する機能が制限されていることを理解してください。 | [&#x200B; リファラーパラメーター](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/forms/form-fields/set-a-hidden-form-field-value.html?lang=ja#referrer-parameter){target="_blank"} |
| 5 | **GDPR/CASL準拠** | <li>フォームを通じてデータが取得された場合、オプトインは自社のポリシーに準拠していますか？ <li>プライバシーポリシーリンクが機能するコレクション文を提供していますか？ | **はい：** <br>関連するコンプライアンス環境について：この質問に「はい」で回答できない場合は、プライバシーポリシーの節を更新してコンプライアンスを確認する必要があります。 **不明な場合は、法務部門に適切なアドバイスを求めてください。** | [&#x200B; プライバシー管理](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/privacy-management.html?lang=ja){target="_blank"} |
| 6 | **Google [!DNL Analytics]統合** | お使いのWeb PersonalizationはGoogle [!DNL Analytics]と統合されていますか？ | **はい、またはいいえ：**<br>&#x200B;いいえ回答する場合は、web パーソナライゼーションの影響を追跡する機能が制限されていることを理解してください。 | [Googleでのパーソナライズされたリマーケティング &#x200B;](https://experienceleague.adobe.com/docs/marketo/using/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.html?lang=ja){target="_blank"} |
| 7 | **Web セグメント** | <li>選択したセグメントは適切で、適切なドメインに適用されますか？ <li>セグメントはGoogle [!DNL Analytics]に送信されますか？ | **はい：** <br> 「はい」で回答できない場合は、更新する必要があります。 | [Web セグメント &#x200B;](https://experienceleague.adobe.com/docs/marketo/using/product-docs/web-personalization/using-web-segments/web-segments.html?lang=ja){target="_blank"}<br><br>[特定のセグメントを使用しているWeb [!DNL Campaign]を検索](https://experienceleague.adobe.com/docs/marketo/using/product-docs/web-personalization/using-web-segments/find-web-campaigns-that-are-using-a-specific-segment.html?lang=ja){target="_blank"} |

>[!TAB ランディングページ]

| # | レビューエリア | ベンダーへの質問 | 受け入れ基準 | その他のリソース |
|---|---|---|---|---|
| 1 | **デザイン** | デザインはブランドと一致していますか？ 適切なテンプレートを使用しているか？ | **はい：** <br> 「はい」で回答できない場合は、その理由が必要か、再設計する必要があります。 | [Marketo ランディングページテンプレートの編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-templates/edit-a-marketo-landing-page-template.html?lang=ja){target="_blank"} |
| 2 | **テスト** | デバイスやブラウザーでテストされているか？ 果たして両方ともクリーンに機能しているのだろうか。 | **はい：** <br>回答できない場合は、デバイスとブラウザー間でプレビューリンクをテストする必要があります。 | [&#x200B; ランディングページのプレビュー](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/preview-a-landing-page.html?lang=ja){target="_blank"} |
| 3 | **URL** | ページ URLはカスタマイズされていますか？ それは論理的ですか、それとも命名規則に従っていますか？ | **はい：** <br>はい付きで回答できない場合は、ページ URLを更新してください。 | [&#x200B; ランディングページ URLを変更](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/change-the-landing-page-url.html?lang=ja){target="_blank"} |
| 4 | **Meta/OG タグ** | OG タグが設定されていますか？ タイトル、説明、画像などを入力します。 これらは、ソーシャル共有でのページの表示方法に影響します。 | **はい：** <br>回答できない場合は、すべてのタグを更新する必要があります。 | [&#x200B; ランディングページのタイトルとメタデータの編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/edit-landing-page-title-and-metadata.html?lang=ja){target="_blank"} |
| 5 | **ロボット** | 設定は何ですか？ ニーズを考慮しつつ、有意義なコンテンツを提供できているか、 | **はい：** <br>これを「はい」で回答できない場合は、更新してください。 | [&#x200B; ロボットとはどういう意味ですか？](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/edit-landing-page-title-and-metadata.html?lang=ja){target="_blank"} |
| 6 | **パーソナライゼーション** | ページにパーソナライズされた要素（動的コンテンツ、スニペットなど）が含まれている場合、テストしたことがありますか？ みなさん、期待通り働いていますか？ | **はい/該当しません：** <br>はい、またはn/aに答えられない場合は、テストを行ってください。 | [&#x200B; ランディングページで動的コンテンツを使用](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/personalizing-landing-pages/use-dynamic-content-in-a-landing-page.html?lang=ja){target="_blank"}<br><br> [動的コンテンツを含むランディングページのプレビュー](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/preview-a-landing-page-with-dynamic-content.html?lang=ja){target="_blank"} |
| 7 | **画像** | すべての画像が正しく圧縮されていますか？ 画像にテキストが重なっている場合、明確に読み取れますか？ これらの画像を使用する権利があり、ブランド基準に準拠しているか？ | **はい/該当しません：** <br>すべての画像（使用されている画像がある場合）を圧縮して、メールの読み込み速度を向上させる必要があります。 | [&#x200B; アップロードした画像またはファイルを置き換える](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/images-and-files/replace-an-uploaded-image-or-file.html?lang=ja){target="_blank"} |
| 8 | **コピー** | 文法の誤りがないかコピーを確認しましたか。 自社のブランドボイスに即したコピーを制作していますか？ そのコピーは、ページの目的が何かを明確にしていますか？ | **はい/該当しません：** <br> 「はい」または「該当なし」に回答できない場合は、コピーを確認してください。 |  |
| 9 | **フォーム** | ランディングページにフォームが配置されている場合、適切なフォームが参照されていますか？ Marketo以外のランディングページを使用している場合は、フォームアセットページの埋め込みコードも確認して、[2023年8月に廃止された古いURL構造](https://nation.marketo.com/t5/product-documents/upcoming-changes-to-design-studio-urls/ta-p/306632){target="_blank"}の影響を受けないようにする必要があります。 | **はい/該当しません：** <br> 「はい」に回答できない（または該当しない）場合は、修正してください。 | [&#x200B; フォームを含むランディングページ &#x200B;](https://experienceleague.adobe.com/docs/marketo/using/getting-started-with-marketo/quick-wins/landing-page-with-a-form.html?lang=ja){target="_blank"}<br><br> [Web サイトにフォームを埋め込む](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.html?lang=ja){target="_blank"}<br><br>[&#x200B; デザインスタジオ URLの変更](https://nation.marketo.com/t5/product-documents/upcoming-changes-to-design-studio-urls/ta-p/306632)<br> |
| 10 | **ありがとうございます** | ページにフォームがある場合、送信時に必要に応じて、成功メッセージ/感謝ページへのリダイレクトがページに表示されますか？ | **はい/該当しません：** <br> 「はい」に回答できない（または該当しない）場合は、送信後の設定を修正します。 | [&#x200B; ランディングページのリダイレクト &#x200B;](https://experienceleague.adobe.com/docs/marketo/using/getting-started-with-marketo/quick-wins/redirect-a-landing-page.html?lang=ja){target="_blank"} |
| 11 | **GDPR/CASL準拠** | データがフォームを通じて取得された場合、オプトインは準拠していますか？また、プライバシーポリシーリンクを機能させながら、コレクションに関する声明を提供していますか？ | **はい：** <br>関連するコンプライアンス環境について：この質問に「はい」で回答できない場合は、更新してコンプライアンスを確認する必要があります。 知らない場合は、適切なアドバイスを求めてください。 | [&#x200B; プライバシー管理](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/privacy-management.html?lang=ja){target="_blank"} |
| 12 | **トラッキング** | [!DNL Google Analytics]、タグマネージャー、および/またはMunchkinの設定が意図したとおりにページに適用されていますか？ このランディングページでは、デフォルトでMunchkinsのオンとオフを切り替えるべきですか？ | **はい/該当しません：**<br>&#x200B;はい、または該当しない場合は、[!DNL Marketo Engage]管理者に確認してください。 | [Munchkin コードが機能しているかどうかをテストします](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.html?lang=ja#test-if-your-munchkin-code-is-working){target="_blank"} |

>[!TAB フォーム]

| # | レビューエリア | ベンダーへの質問 | 受け入れ基準 | その他のリソース |
|---|---|---|---|---|
| 1 | **レスポンシブ** | フォームデバイスはレスポンシブですか？ | **はい：** <br>はい付きで回答できない場合は、CSSを更新してレスポンシブにする必要があります。そうしないと、パフォーマンスに影響を与える可能性があります。 |  |
| 2 | **デザイン** | フォームブランドのデザインは一貫していますか？ | **はい：** <br>この質問に「はい」で回答できない場合は、理由が必要か、CSSを更新してブランドに準拠させる必要があります。 |  |
| 3 | **データフロー** | すべてのデータは意図したとおりにフィールドにマッピングされますか？ テストレコードのアクティビティログを確認して、これを証明しましたか？ | **はい：** <br>はい付きで回答できない場合は、マッピングを修正してテストする必要があります。 | [人物のアクティビティ ログを探す](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.html?lang=ja){target="_blank"} |
| 4 | **トラッキング** | このフォームへの送信のソースを追跡するために、非表示のUTM フィールドを配置していますか？ これらはテストされていますか？ | **はい、またはいいえ：** <br>いいえ回答する場合は、このフォームにユーザーが送信したソースを追跡する機能が制限されていることを理解してください。 | [&#x200B; フォームフィールドを非表示に設定](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.html?lang=ja){target="_blank"}<br><br>[非表示フォームフィールド値を設定](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/forms/form-fields/set-a-hidden-form-field-value.html?lang=ja){target="_blank"} |
| 5 | **GDPR/CASL準拠** | データがフォームを通じて取得された場合、オプトインは準拠しており、機能するプライバシーポリシーのリンクを使用してコレクション文を提供しますか？ | **はい：** <br>関連するコンプライアンス環境について：この質問に「はい」で回答できない場合は、更新してコンプライアンスを確認する必要があります。 **分からない場合は、適切なアドバイスを求めてください。** | [&#x200B; プライバシー管理](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/privacy-management.html?lang=ja){target="_blank"} |

>[!TAB  スマートキャンペーン ]

| # | レビューエリア | ベンダーへの質問 | 受け入れ基準 | その他のリソース |
|---|---|---|---|---|
| 1 | **正確性** | 必要なスマート [!DNL Campaign]がすべてチェックされ、レビューされ、正確であると見なされましたか？ | **はい：** <br>はい付きで回答できない場合は、修正して確認してから続行してください。 | [&#x200B; スマート  [!DNL Campaign]  チェックリスト &#x200B;](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/smart-campaign-checklist.html?lang=ja){target="_blank"} |
| 2 | **送信回数** | メール送信キャンペーンがバッチキャンペーンの場合（トリガーされない場合）、「スケジュール」タブのリード数を確認します。この数は、期待するものと一致していますか？ 中止閾値を下回っていますか？ | **はい：** <br>はい付きで回答できない場合は、修正して確認してから続行してください。 | [&#x200B; メールプログラムのスケジュール &#x200B;](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.html?lang=ja){target="_blank"} |
| 3 | **プライマリルール** | プライマリセグメンテーション/リストは、適切な場合または適切な場合に使用していますか？ | **はい、または該当しません：**<br>&#x200B;プライマリリスト/セグメンテーションは、参照する必要があるフィールドの数を減らし、人為的なミスのリスクを減らすように設計されています。 プライマリリスト/セグメンテーションを使用しない場合は、ルールを確実に実行する必要があります。 |  |
| 4 | **アトリビューション** | プログラムが新しいリード（イベントプログラムなど）を獲得する場合、必要に応じてアトリビューション設定を含めますか？ 獲得プログラムはマッピングされていますか？ | **はい、または該当しません：** <br> プログラムにユーザーをインポートする場合、またはプログラムが新しいユーザーを獲得する場合は、獲得プログラムの設定を使用する必要があります。 |  |
| 5 | **エンゲージメントプログラム** | スマート [!DNL Campaign]をエンゲージメント プログラムで使用する場合、メンバーを適切に追加、一時停止、再起動するための手順はありますか？ これらの手順は他の人によってレビューされていますか？ | **はい、または該当しない：**<br>&#x200B;これがエンゲージメントプログラムであり、正当な理由なしに「はい」と回答できない場合は、これが有効になるまでアクティブにしないでください。 | [&#x200B; エンゲージメントプログラムにユーザーを追加](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-people-to-an-engagement-program.html?lang=ja){target="_blank"} |
| 6 | **サブスクリプションの環境設定** | 必要なサブスクリプション環境設定をすべて含んでいますか？ | **はい、または該当しません：**<br>&#x200B;不明な場合は、[!DNL Marketo Engage]管理者にお問い合わせください。 N/Aを進めるには適切な理由が必要です（例えば、運用上の送信）。 | [&#x200B; サブスクリプションセンターの設定と管理方法](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/subscription-center-watch.html?lang=ja){target="_blank"} |
| 7 | **プログラムの状態** | プログラムステータスを更新するために含まれるフローステップはありますか？ | **はい：** <br>はい付きで回答できない場合は、スマート [!DNL Campaign] フローステップにこれらを追加する必要があります。 | [&#x200B; プログラムステータスの変更](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.html?lang=ja){target="_blank"} |
| 8 | **より大きな影響** | <li>他のチームやシステムと同期するフィールドにアラートや書き込みを送信するフローステップはありますか？ <li>その場合、その数を考慮し、それらのチーム/システムの関係者にアドバイスを提供していますか？ | **はい、いいえ、該当しません：**<br>&#x200B;回答は問題ありませんが、マップを作成する場合は、通常、システムを所有するチームに通知する必要があります。 不明な場合は、管理者に問い合わせてください。 |  |
| 9 | **影響のスコア付け** | リード/個人のスコアリングへの影響を考慮していますか？ | **はい、または該当しません：** <br>はい、または該当しない場合は、管理者にお問い合わせください。 | [&#x200B; シンプルなスコアリング &#x200B;](https://experienceleague.adobe.com/docs/marketo/using/getting-started-with-marketo/quick-wins/simple-scoring.html?lang=ja){target="_blank"}<br><br>[&#x200B; リードスコアリングプログラムの構築方法](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/lead-scoring-watch.html?lang=ja){target="_blank"} |
| 10 | **レベニューサイクルModeler（RCM）の影響** | 個人のライフサイクルモデルへの影響を考慮していますか？ | **はい、または該当しません：** 「はい」に回答できない、または該当しない場合は、管理者にお問い合わせください。 | [収益サイクル Modelerの設定](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.html?lang=ja){target="_blank"} |
| 11 | **エンゲージメントプログラムへの影響** | <li>既存のエンゲージメントプログラムへの影響を考慮しましたか？ <li>人々が複数の通信に襲われないようにしましたか？ | **はい、または該当しません：**<br>&#x200B;はい、または該当しない場合は、管理者にお問い合わせください。 | [重複したコンテンツの送信を避ける](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/using-engagement-programs/avoid-sending-duplicate-content.html?lang=ja){target="_blank"} <br><br>[通信制限をSmart [!DNL Campaign]](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/apply-communication-limits-to-smart-campaign.html?lang=ja){target="_blank"}に適用する |
| 12 | **成功の報告** | プログラムの成功は論理的に測定されているか？ 成功は合理的ですか – プロセスに近すぎませんか？ 達成するには遠すぎませんか？ 成功に関するレポートを作成し、成果を測定するための戦略を策定していますか？ | **はい：** <br>はい回答できない場合は、成功指標の定義を見直してください。 | [&#x200B; プログラムの成功の変更](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-success.html?lang=ja){target="_blank"} |

>[!TAB リスト]

| # | レビューエリア | ベンダーへの質問 | 受け入れ基準 | その他のリソース |
|---|---|---|---|---|
| 1 | **ロジック** | スマートリストを使用してオーディエンスのいずれかの部分を識別している場合、ロジックはチェックされ、レビューされ、正確であると見なされますか？ | **はい：** <br>はい付きで回答できない場合は、スマートリストの設定を修正し、確認してから続行する必要があります。 |  |
| 2 | **インポートプロセスを一覧表示** | 静的リストを使用してオーディエンスの一部を識別している場合、データソースは信頼でき、リストのインポートプロセスに従って正確かつ正確にインポートが実行されていますか？ | **はい：** <br>はい付きで回答できない場合は、先に進む前にリスト データを修正し、これらのチェックを行う必要があります。 | [静的リストからユーザーを追加または削除する方法](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/understanding-static-lists.html?lang=ja){target="_blank"}<br><br>[&#x200B; ユーザーのリストを読み込む](https://experienceleague.adobe.com/docs/marketo/using/getting-started-with-marketo/quick-wins/import-a-list-of-people.html?lang=ja#step-import-your-spreadsheet-into-marketo) |
| 3 | **除外** | 必要な除外事項が含まれているか（例：競合他社、登録解除の制限に関するブロックリスト） | **はい、または該当しません：** <br>お客様が法的に準拠している非常に優れた理由がない限り、購読解除をフィルタリングする必要があります。 自社のコンテンツ、キャンペーンのルール、法的根拠が含まれていない場合は、それらを確認する必要があります。 | [登録解除について](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html?lang=ja){target="_blank"}<br><br>[&#x200B; データ値の変更](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html?lang=ja){target="_blank"} |
| 4 | **プライマリリスト** | プライマリリスト/セグメンテーションは適切な場所で使用されていますか？ | **はい、または該当しません：**&#x200B;プライマリリスト/セグメンテーションは、参照する必要があるフィールドの数を減らし、人為的なミスのリスクを減らすように設計されています。 プライマリリスト/セグメンテーションを使用していない場合は、ルールに自信を持って対処する必要があります。 | [&#x200B; セグメントルールの定義](https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.html?lang=ja) |

>[!TAB オーディエンス]

| # | レビューエリア | ベンダーへの質問 | 受け入れ基準 | その他のリソース |
|---|---|---|---|---|
| 1 | **法的根拠：**<br> オーディエンスへの連絡に適した法的根拠があります。 | <ul><li>**明示的：**&#x200B;顧客は、企業からのマーケティングコミュニケーションの受信を明示的にオプトインしていますか？ </li><li>**推測値（準拠している場合）:**&#x200B;担当者が連絡先情報を提供しており、この情報を使用して連絡することを合理的に期待できますか？ </li><li>**認定（準拠している場合）:**&#x200B;公開されているソースから連絡先の詳細を取得しており、公開されているソースからコンテンツが関連していると合理的に判断できますか？</li></ul> | **はい、基準を明記します：**&#x200B;選択した基準がコンプライアンス環境で有効であることを確認してください。 「はい」で回答できない場合は、プログラムの立ち上げを延期し、このオーディエンスに連絡するための法的根拠について説明を求めます。 | [&#x200B; プライバシー管理](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/privacy-management.html?lang=ja){target="_blank"} |
| 2 | **データソース** | インポートリストを通じてオーディエンスを特定した場合、データソースは信頼できますか？ | **はい、または該当しません：**<br>&#x200B;はい付きで回答できない場合は、データソースに関する説明を求めます。 | [&#x200B; リストを読み込んでオーディエンスを定義](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/email-programs/managing-people-in-email-programs/define-an-audience-by-importing-a-list.html?lang=ja){target="_blank"} |
| 3 | **購入リスト** | オーディエンスは、リストの購入やスポンサーシップの活動を通じて獲得したか？ | **ソース = リスト購入：**<br> リスト購入が悪い慣行であり、多くの場所で違法であり、多くの場合、マーケティングオートメーションプラットフォームとの契約違反です。<br><br>**はい、ソース = スポンサーシップ** <br> スポンサーシップと競合の場合、データキャプチャが準拠していることを確認してください。 最初のコミュニケーションでは、情報をどのように受け取ったかを明確にし、オプトアウトを容易にすることがベストプラクティスです。 |  |
| 4 | **関連性** | このオーディエンスに送信しようとしている情報は、そのオーディエンスと、そのオーディエンスとの関係に関連しています。 | **はい：** <br>あなたが「はい」で答えられない場合は、立ち止まって、なぜこれらの人にメールを送信するのかを慎重に検討してください。 顧客や顧客との関係に関係のない情報を送信すると、パフォーマンスや配信品質に悪影響を及ぼす可能性があり、コンプライアンス環境に違反している可能性があります。 |  |
| 5 | **期待値** | このオーディエンスは、皆さんからの便りを期待しています。 | **はい：** <br>あなたが「はい」で答えられない場合は、立ち止まって、なぜこれらの人にメールを送信するのかを慎重に検討してください。 自社からのメール配信を希望しない、または希望しないオーディエンスに電子メールを送信すると、パフォーマンス、配信品質に悪影響を与え、コンプライアンス環境に違反する可能性があります。 |  |

>[!TAB 電子メールアセット ]

| # | レビューエリア | ベンダーへの質問 | 受け入れ基準 | その他のリソース |
|---|---|---|---|---|
| 1 | **送信者の電子メールアドレス** | ブランドオーナーに確認し、メールアドレスが安全に使用できることを確認しましたか？ | **はい：** <br>はい付きで回答できない場合は、先に進む前に送信者の電子メールを確認してください。 | [電子メールヘッダーを編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/creating-an-email/edit-your-email-header.html?lang=ja){target="_blank"}<br><br>[電子メールからのデフォルトとラベルからのデフォルトの変更](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/change-the-default-from-email-and-from-label.html?lang=ja){target="_blank"} |
| 2 | **送信者名** | ブランドオーナーに確認し、名前が安全に使用できることを確認しましたか？ | **はい：** <br>はい付きで回答できない場合は、先に進む前に確認する必要があります。 | [電子メールヘッダーを編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/creating-an-email/edit-your-email-header.html?lang=ja){target="_blank"}<br><br>[電子メールからのデフォルトとラベルからのデフォルトの変更](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/change-the-default-from-email-and-from-label.html?lang=ja){target="_blank"} |
| 3 | **返信先アドレス** | ブランドオーナーに確認し、安全に使用できることを確認しましたか？ | **はい：** <br> 「はい」で回答できない場合は、先に進む前に確認する必要があります。 | [&#x200B; メールヘッダーを編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/creating-an-email/edit-your-email-header.html?lang=ja){target="_blank"} |
| 4 | **プリヘッダー設定** | ベストプラクティス（min）に従ってプリヘッダーを設定していますか？ 80文字、全文、フロントロード（貴重なビット）? | **はい：** <br><br>はい付きで回答できない場合は、先に進む前に更新する必要があります。 | [&#x200B; メール設定](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.html?lang=ja){target="_blank"} |
| 5 | **プルーフをコピー** | スペルや文法の問題はありますか？ <br> トーンはブランドに適していますか？ | **はい：** <br>はい付きで回答できない場合は、先に進む前に修正する必要があります。 |  |
| 6 | **スキャン可能性** | このメールの重要な情報をスキャンで理解できますか？ | **はい、または該当しません：** <br>電子メールのベストプラクティスでは、電子メールの主要メッセージをスキャンで確実に理解することが重要であることを示しています。 この方法を適用しないことを選択した場合、メールのパフォーマンスに影響を与える可能性があることに注意してください。 |  |
| 7 | **登録解除** | そのメールには、テストした登録解除リンクが含まれていますか？ | **はい、または該当しません：**<br>&#x200B;該当しない電子メールは、[operational](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.html?lang=ja){target="_blank"}の場合にのみ有効である必要があります。 登録解除は必要ないと確信してください。疑わしい場合は、その旨を記載した方が安全です。 | [登録解除について](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html?lang=ja){target="_blank"} |
| 8 | **テキストバージョン** | <li>メールのテキストバージョンを作成しましたか？ <li>テキスト版のテストを自分に送信しましたか？ | **はい：**<br> 「はい」で回答できない場合は、続行する前にテストする必要があります。 |  |
| 9 | **テキストバージョンの最適化** | <li>テキスト版のレイアウトは最適化されていますか？<li>HTMLのコメントは表示されていますか？<li>関連するコンテンツはすべて含まれていますか？ | **はい：**<br>&#x200B;自動生成されたテキスト バージョンは、読みにくいため、最適化する価値があります。 | [&#x200B; メールのテキストバージョンの編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/creating-an-email/edit-the-text-version-of-an-email.html?lang=ja){target="_blank"} |
| 10 | **テキスト バージョン ハイパーリンクとUTMS** | ハイパーリンクは、これらの領域で動作し、UTMを含めますか？ ：<ul><li>ヘッダーセクション</li><li>画像領域（含まれる場合）</li><li>本文</li><li>CTA</li>フッター</li></ul> | **はい：**<br> 「はい」で回答できない場合は、修正して確認してから続行してください。 自動テキストバージョンでは、変数が確実に読み込まれません。 |  |
| 11 | **HTML/メインバージョン** | <li>HTML/メイン版のメールを作成しましたか？<li>テストを送りましたか？ | **はい（プレーンテキストのみを除く）:**<br>&#x200B;はい付きで回答できない場合は、続行する前にテストを送信する必要があります。 | [電子メールのHTMLを編集](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/edit-an-emails-html.html?lang=ja){target="_blank"} |
| 12 | **画像** | <li>すべての画像に代替テキストはありますか？ <li>壊れた画像はありますか？ | **はい、または該当しません：**<br>。 はい付きで回答できない場合は、続行する前に修正して確認する必要があります（画像がない場合を除く）。 |  |
| 13 | **画像の圧縮** | <li>すべての画像は、画像編集ソフトウェアからweb用に保存されましたか？ <li>アップロード前に圧縮されていたか？ <li>メールの読み込み時間は許容可能ですか？ | **はい、または適用できません：**<br>&#x200B;すべての画像（使用されている場合）は、読み込み速度を向上させるために圧縮する必要があります。 | ヒーロー画像は120 kb以下にし、小さい画像はすべて小さくする必要があります。 読み込み時間が長いと、パフォーマンスに影響を及ぼす。 |
| 14 | **HTML バージョンのハイパーリンクとUTM** | すべてのハイパーリンクが機能し、これらの領域にUTMが含まれていますか？ ：<ul><li>ヘッダーセクション</li><li>画像領域（含まれる場合）</li><li>本文</li><li>CTA</li>フッター</li></ul> | **はい：**<br>&#x200B;壊れたリンクは送信しないでください。 「はい」と答えられない場合は、続行する前に修正してください。 |  |
| 15 | **動的コンテンツ** | <li>メールには動的コンテンツが含まれていますか？<li>複数のシナリオでテストしましたか？ | **はい：**<br> 「はい」で回答できない場合は、続行する前にテストする必要があります。 | [&#x200B; メールで動的コンテンツを使用](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.html?lang=ja){target="_blank"}<br><br>[動的コンテンツを含むメールをプレビュー](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.html?lang=ja){target="_blank"} |
| 16 | **法的要件** | <ul><li>何かオファーを間違えていませんか？</li><li>コンプライアンス環境に従って必要な免責事項は含まれていますか？</li></ul> | **はい：**<br> 「はい」で回答できない場合は、修正して確認してから続行してください。 |  |
| 17 | **同僚がレビューしました** | 別の[!DNL Marketo Engage]人のユーザーがテストメールをレビューしましたか？ | **はい：**<br> 「はい」で回答できない場合は、送信する前に行う必要があります。 |  |
| 18 | **運用上の送信** | <ul><li>メールを運用中（つまり、配信停止の設定をバイパス）に設定していますか？<li>その場合は、正当な理由があるのでしょうか。</li> | **はい/いいえ：**<br> 「はい」で回答する場合は、有効な理由を確認してメールを送信してください。 不明な点がある場合は、管理者に問い合わせてください。[!DNL Marketo Engage] | [電子メールを運用中にする](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.html?lang=ja){target="_blank"} |
| 19 | **A/B テストとチャンプ/チャレンジャーテスト** | 電子メールでチャンピオン/チャレンジャーテストを実施していますか？ | **はい/いいえ：**<br> テストを実施していない場合は、オーディエンスの詳細を確認する機会を逃している可能性があるかどうかを考えます。 | [A/B テストの作成](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/email-marketing/ab-testing-watch.html?lang=ja)<br><br>[電子メールチャンピオン/チャレンジャーの追加](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/email-tests-champion-challenger/add-an-email-champion-challenger.html?lang=ja){target="_blank"} |
| 20 | **クライアントテスト** | クライアントテストソフトウェアでメールを実行しましたか？<li>主要なメールクライアントのディスプレイに関する問題を特定しましたか？ <li>緊急でないテンプレートの修正として修正またはログに記録していますか？ <li>読み込み速度の問題を特定し、改善しようとしましたか？<li>件名/プレビュー行の問題を特定しましたか？ 解決したか？ | **はい、または該当しません：**<br> 「はい」で回答できない場合（テストソフトウェアがない場合を除く）、送信する前に行う必要があります。 | クライアントテストソフトウェアの例としては、LitmusまたはEmail on Acidまたは[Marketo Email Deliverability Power Pack](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/email-deliverability-power-pack-how-to-import-a-seed-list.html?lang=ja)<br><br>[受信トレイのトラッカーチュートリアル &#x200B;](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/inbox-tracker/inbox-tracker-tutorials.html?lang=ja){target="_blank"}があります |
| 21 | **スパムテスト** | スパムメールを送信したことがありますか？<li>認識のために掲げられた旗をブロックリストに加えるする旗はありますか？<li>受信トレイの配置/メールクライアントフラグを特定しましたか？ <li>潜在的な原因を探し、解決しようとしましたか？ | **はい、または該当しません：**<br>&#x200B;はい（テストソフトウェアがない場合を除く）で回答できない場合は、送信前に行う必要があります。 | 契約に含まれている場合、またはLitmusやEmail on Acidなどのツールがある場合は、[Marketoの受信トレイ トラッカー機能](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/inbox-tracker/inbox-tracker-tutorials.html?lang=ja){target="_blank"}を使用してください。 |
| 22 | **追加[!DNL Analytics]** | そのメールには追加の分析コードが含まれていますか？ | **はい、または該当しません：**<br> 「はい」で回答できない場合（追加の分析ソフトウェアがない場合を除く）、送信する前に行う必要があります。 |  |

>[!TAB 最終チェック ]

| # | レビュー | ベンダーへの質問 | 受け入れ基準 |
|---|---|---|---|
| 1 | **アセットの承認** | 最終版のプログラムアセットとチャンピオン/チャレンジャーテストが完全に承認され、ドラフトモードが最終的に変更されないことを確認します。 | **はい：**<br> 「はい」で回答できない場合は、送信前に行う必要があります。 |
| 2 | **スマート [!DNL Campaign]の精度** | スマートキャンペーンは適切なアセットを参照しているか？ | **はい：**<br> 「はい」で回答できない場合は、送信前に修正する必要があります。 |
| 3 | **チェックリストの手順** | 上記のチェックは完了しましたか？ | **はい：**<br> 「はい」で回答できない場合は、送信する前に行う必要があります。 |
| 4 | **関係者の承認** | このキャンペーンは、関係者から最終的な承認を得ていますか？ | **はい：**<br> 「はい」で回答できない場合は、送信する前に行う必要があります。 |

>[!ENDTABS]

## 次の手順

[ここ](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe_Marketo_Engage_Inherited_Instance_Program_Prelaunch_QA_Checklist.xlsx)をクリックして、編集可能なプログラムの起動前のチェックリストをダウンロードし、カスタマイズします。 このルールは、組織のワークフローに合わせて調整する必要があります。 効果的なQA プロセスを構築することで、説明責任を果たし、顧客と接する際のミスを減らすことができます。

### 制作者

**グレース・ブレブナー**
[!DNL Adobe] Marketo Champion （2021年）
*Merkle Company、APAC Region, Digital Pi, LLC、クライアント戦略担当ディレクター*

![&#x200B; グレース ブレブナー](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Grace_Brebner.png){width=30%}

**Amy Chiu**
*導入および維持マーケティングマネージャー、[!DNL Adobe]*

![Amy Chiu](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width=30%}
