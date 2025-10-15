---
title: 新しいMarketo Engageの導入を計画する
description: 新しいMarketo Engageインスタンスを適切に実装するための基本的な計画および部門横断的なチームの共同作業について説明します。 このチュートリアルでは、シームレスなMarketo Engage実装のためのサンプルマイルストーン、チームエンゲージメント、リソース割り当てを提供します。
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last: substantial-update- 2024-05-01
jira: KT-14808
thumbnail: KT-14808.jpeg
exl-id: 65119abd-6f13-4acc-9e99-09843369ad28
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '1098'
ht-degree: 5%

---

# 新しいMarketo Engageの導入を計画する

新しいMarketo Engageインスタンスを導入するには、綿密な計画、チーム間のコラボレーション、継続的な最適化が必要です。 新しいインスタンスを導入するための完璧な方法はありませんが、事前に計画を立てることでプロセスがはるかにスムーズになることにご同意いただけるMarketo Engage管理者がほとんどです。

このチュートリアルでは、Marketo Engageのロールアウトを成功させるために重要な具体的なマイルストーン、チームエンゲージメント、リソース割り当てを詳しく説明します。

## 新しいMarketo Engageを導入する際の重要なマイルストーン

### フェーズ 1 – 検出と計画

- マーケティングおよび販売ニーズ評価の実施
- 目標または主要業績評価指標（KPI）の定義

### フェーズ 2 – 技術的なセットアップと設定

- CNAME や Munchkin コードなどの管理設定の指定。
- リード管理プロセスの設定
- 自動化ワークフローとデータ同期のテスト

### フェーズ 3 - プログラムライブラリの作成とキャンペーンの設定

- メールテンプレートとランディングページの開発。 [&#x200B; プログラムのインポート ライブラリ &#x200B;](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program) から [&#x200B; スタータープログラムのインポート &#x200B;](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-library/program-import-library-overview) を開始します。
- セグメント化ルールとPersonalization ルールの設定
- リードジェネレーションと育成のための初期キャンペーンの作成

### フェーズ 4 - トレーニングとユーザーの採用

- ユーザー向けのトレーニングセッションや資料の実施
- インスタンスのガバナンスポリシーとベストプラクティスの確立
- ユーザー採用指標と関係者のフィードバックの監視

### フェーズ 5 – 運用開始と最適化

- 最終的なシステムテストと品質保証
- 最初のキャンペーンの開始とパフォーマンスの監視
- レポートと分析に基づく反復的な改善の実装

## 関係者のエンゲージメントと必要なリソース

新しいインスタンスを実装する場合は、最大限のメリットを得るために入念な計画と実行が必要です。 適切な関係者を最初に巻き込むことで、組織全体のニーズに合わせて実装を調整できます。 Marketo Engageを実装する適切な内部パートナーを見つけるのに役立つ、以下のプロジェクトの主な関係者のサンプルとその潜在的な役割を参照してください。

<table>
 <thead>
    <tr>
        <th>関係者</th>
        <th>考えられる役割と責務  </th>
    </tr>
 </thead>    
 <tbody>
    <tr>
        <td>マーケティング業務Director/マネージャー</td>
        <td>
        <li>プロジェクトの主要連絡窓口</li>
        <li>インスタンスガバナンスルール</li> 
        <li>レポートおよび分析用のデータ分析 </li> 
        </td>
    </tr>
    <tr>
        <td>CRM 管理者</td>
        <td>
        <li>CRM 同期 </li>
        <li>リードフロー</li> 
        </td>
    </tr>
     <tr>
        <td>IT 管理者</td>
        <td>
        <li>マンチキン</li>
        <li>SPF/DKIM </li> 
        <li>Web ドメインの設定</li> 
        <li>CNAME</li> 
        <li>メールの配信品質</li>
        </td>
    </tr>
    <tr>
        <td>エンジニアリング</td>
        <td>
        <li>カスタムサービス統合作業の開発 </li>
        <li>データのマッピングと移行のためのデータエンジニアリング</li> 
        </td>
    </tr>
     <tr>
        <td>マーケティング </td>
        <td>
        <li>プログラムテンプレートの作成とデザイン</li>
        <li>チャネル </li>
        <li>リード/人物のスコアリングとライフサイクル</li> 
        <li>プログラムの有効性に関するレポートとフィードバック</li> 
        </td>
    </tr>
     <tr>
        <td>売上</td>
        <td>
        <li>リード/人物スコアリングモデリング</li>
        <li>リードフロー/ルーティング</li>  
        <li>ライフサイクルサービスレベルアグリーメント（SLA）</li> 
        </td>
    </tr>
     <tr>
        <td>C-Suite</td>
        <td>
        <li>プロジェクト全体の方向性  </li>
        <li>実装の大まかな目標</li> 
        </td>
    </tr>
</table>

## ピアの観点 – Marketo Engageの実装

Marketo Engageチャンピオン（2019）の Kyle McCormick が、Palotos Networks でのオンボーディングと実装の経験について説明します。 彼が直面した課題と、オンボーディングプロセスを成功かつ効率的に推進する方法に関するアドバイスを学びます。

>[!VIDEO](https://video.tv.adobe.com/v/3428771/?quality=12&learn=on)

## 次の手順

新しい実装プロジェクトの計画とタイムラインを作成します。 以下は、サンプルマイルストーン、タスク、担当チーム、期限、依存関係のセクションを含む、サンプルプロジェクトタイムラインです。 これを使用すると、Marketo Engage導入ジャーニーを合理化し、組織全体でロールアウトを成功に導くことができます。

また、特定のマイルストーンタスクの編集と追跡の例をダウンロードすることもできます [&#x200B; こちら &#x200B;](/help/marketo-tutorial-implementing-new-instance/assets/adobe-marketo-engage-implementation-milestones-project-management-template.xlsx)。

<table>
 <thead>
    <tr>
        <th>トピック</th>
        <th>マイルストーン</th>
        <th>ステータス</th>
        <th>予定日</th>
        <th>実際の日付</th>
        <th>必要なリソース</th>
    </tr>
 </thead>    
 <tbody>
    <tr>
        <td><em>これらの一般的なオンボーディングのトピックを使用して、マイルストーンの段階を整理します。</em></td>
        <td><em>特定のマイルストーンタスクを書き出します。</em></td>
        <td><em>タスクの現在のステータスを教えてください。</em></td>
        <td><em>このタスクのアニメーション化された完了日を指定してください。</em></td>
        <td><em>このタスクが実際に完了したのはいつですか？</em></td>
        <td><em>このタスクを完了するために必要なリソースと、必要なチームは何ですか？</em></td>
    </tr>
    <tr>
        <td rowspan="2">技術的セットアップ</td>
        <td><em> 例 </em> – 会社の web サイトに MunchkinID をインストールします</td>
        <td bgcolor="c6f0cf">Complete</td>
        <td>9/5/24</td>
        <td>9/12/24</td>
        <td>Web 開発チーム</td>
    </tr>
    <tr>
        <td><em> 例 </em> 配信品質とメールトラッキングリンク用に、Domain Keys Identified Mail （DKIM）と 2 つの個別の CNAME を設定します。</td>
        <td bgcolor="c6f0cf">Complete</td>
        <td>9/15/24</td>
        <td>9/18/24</td>
        <td>IT チームによるサポートとセットアップ</td>
    </tr>
    <tr>
        <td rowspan="4">Adobe Admin Consoleと管理設定</td>
        <td><em> 例 – </em> Marketo Engageのユーザーとロールを作成する</td>
        <td bgcolor="c6f0cf">Complete</td>
        <td>8/27/24</td>
        <td>9/15/24</td>
        <td>Marketo Engageへのアクセスが必要なユーザーに関するマーケティングチームからの情報。</td>
    </tr>
    <tr>
        <td><em> 例 – </em> Adobe Admin ConsoleでMarketo Engageの Product Admin を追加します。</td>
        <td bgcolor="c6f0cf">Complete</td>
        <td>8/27/24</td>
        <td>9/15/24</td>
        <td>Marketo Engageに対する管理者アクセス権を必要とするユーザーに関する、マーケティング運営チームからの情報。</td>
    </tr>
    <tr>
        <td><em> 例 – </em> サポート管理者の設定</td>
        <td bgcolor="c6f0cf">Complete</td>
        <td>8/27/24</td>
        <td>9/15/24</td>
        <td>サポートの主要連絡先を確認するためのマーケティング運営チームからの情報。 サポート管理者ユーザーを割り当てるためのシステム管理者からのサポート。</td>
    </tr>
    <tr>
        <td><em> 例 – </em> フォルダー構造と命名規則の定義</td>
        <td bgcolor="c6f0cf">Complete</td>
        <td>9/7/24</td>
        <td>9/12/24</td>
        <td>プログラムの種類や組織のニーズに関するMarketo Engageを使用して、各チームから入力します。</td>
    </tr>
    <tr>
        <td rowspan="2">CRM 統合（該当する場合）</td>
        <td><em> 例 – </em> 同期前のフィールドマッピングの特定</td>
        <td bgcolor="ffeb9c">処理中</td>
        <td>10/22/24</td>
        <td>なし</td>
        <td>CRM 管理者のサポートにより、使用可能なフィールドを把握できます。</td>
    </tr>
    <tr>
        <td><em> 例 </em> データ監査の実施</td>
        <td bgcolor="ffeb9c">処理中</td>
        <td>10/26/24</td>
        <td>なし</td>
        <td>CRM 管理者または予算からのサポート。</td>
    </tr>
    <tr>
        <td rowspan="2">運用プログラム ビルド</td>
        <td><em> 例 </em> 受信データを標準化するプログラムを作成する</td>
        <td bgcolor="ffc7cf">開始されていません</td>
        <td>11/9/24</td>
        <td>なし</td>
        <td>営業運用チームおよび CRM チームによるデータ管理戦略の決定のサポート。</td>
    </tr>
    <tr>
        <td><em> 例 – </em> メールサブスクリプションセンターの作成</td>
        <td bgcolor="ffc7cf">開始されていません</td>
        <td>11/19/24</td>
        <td>なし</td>
        <td>マーケティングチームからの、メーリングリストのコンテンツタイプとセグメント化に関する入力。</td>
    <tr>
        <td rowspan="2">最初のマーケティングプログラムビルド</td>
        <td><em> 例 – </em> 基本的な電子メールプログラムの設定</td>
        <td bgcolor="ffeb9c">処理中</td>
        <td>11/12/24</td>
        <td>なし</td>
        <td>メールおよびランディングページ用のデジタルチームのクリエイティブアセット。</td>
    </tr>
    <tr>    
        <td><em> 例 – </em> 四半期ニュースレター用のプログラムを作成する</td>
        <td bgcolor="ffc7cf">開始されていません</td>
        <td>11/30/24</td>
        <td>なし</td>
        <td>ニュースレターのメール用のマーケティングチームのコンテンツや、デザインチームのクリエイティブアセット/コンテンツ。</td>
    </tr>
    <tr>
        <td rowspan="2">LaunchPoint 統合のセットアップ</td>
        <td><em> 例 </em> API のみのユーザーと役割を作成する</td>
        <td bgcolor="ffc7cf">開始されていません</td>
        <td>11/23/24</td>
        <td>   </td>
        <td>マーケティングチームを使用して、新しいインスタンスに必要なサービスの範囲を設定します。</td>
    </tr>
    <tr>
        <td><em> 例 </em> Google Ads のカスタムサービスを作成する</td>
        <td bgcolor="ffc7cf">開始されていません</td>
        <td>12/7/24</td>
        <td>   </td>
        <td>Web チームおよび有料メディアチームによる、Google Ads にアクセスするためのMarketo Engageの認証のサポート。</td>
        <td>
    </tr>
    <tr>
        <td rowspan="2">ユーザートレーニングとドキュメント</td>
        <td><em> 例 </em> 内部ユーザー用のガバナンスガイドの作成</td>
        <td bgcolor="ffc7cf">開始されていません</td>
        <td>12/2/24</td>
        <td>なし</td>
        <td>Marketo Engageガバナンスチームを作成して、ガバナンスに関する補助的なドキュメントを作成したり、ガバナンスプロジェクトを縮小するための予算を編成したりします。</td>
    <tr>
        <td><em> 例 </em> 4 人のユーザーのトレーニングと、標準のMarketo ユーザーアクセスの提供</td>
        <td bgcolor="ffc7cf">開始されていません</td>
        <td>12/13/24</td>
        <td>なし</td>
        <td>Marketo Engageへのアクセスにトレーニングを必須にするマーケティング担当副社長のサポート。</td>
    <tr>
        <td rowspan="2">Go-Live</td>
        <td><em> 例 – </em> 最初のニュースレターを送信する</td>
        <td bgcolor="ffc7cf">開始されていません</td>
        <td>12/9/24</td>
        <td>なし</td>
        <td>マーケティングオペレーションチームは、QA、スケジュール設定および送信をおこないます。</td>
    </tr>
    <tr>
        <td><em> 例 – </em> 最初のメールのパフォーマンスレポートを取り込みます。</td>
        <td bgcolor="ffc7cf">開始されていません</td>
        <td>12/16/24</td>
        <td>なし</td>
        <td>マーケティングオペレーションチームは、QA、スケジュール設定および送信をおこないます。</td>
    </tr>
 </tbody>    
</table>

>[!NOTE]
>ここで示す例は、実際の実装タイムラインに基づいたものではありません。 実装はすべて、組織のニーズに応じて異なるマイルストーンと要件を持つため、Marketo Engageを使用したオンボーディングの標準タイムラインとしてこれらに依存しないでください。

インスタンスにMarketo Engageを実装およびカスタマイズする際の手がかりとなる支援については、Adobeアカウントチームに問い合わせるか、[Adobe Professional Services](https://business.adobe.com/jp/customers/consulting-services/main.html){target="_blank"} にお問い合わせください。

### 作成者

{{amy-chiu}}
