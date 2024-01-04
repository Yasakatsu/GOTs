# アプリケーション名：GoOnToService（Gots）
### サービス内容
1. 上司側が部下の近況、業務の進捗状況を管理し、入力内容を見える化する事が可能となり、個人個人に合ったマネジメントを行う形をサポート
2. 部下は、日々の自身のタスク内容（日報）を入力し、自身で行ったタスク内容を見える化し、自身の不足している点を確認する形をサポート

###　使用対象者
チーム業務を行っている組織のマネジメントする側（上司）とされる側（部下）。
### こだわりポイント
性格診断（FFS診断等）を行い、チーム内で共有させることにより、メンバー１人１人の個性を尊重し、業務改善の指摘、コミニュケーションが取れる。

### 使用メリット（※利用者目線）

1. 上司側:部下のタスクの内容を可視化した状態で分析できるため、容易に部下の現状のタスク状況を確認可能となる。また、診断結果と現在の状況を組み合わせ、部下１人１人にあった指摘箇所を常に目にする事ができるため、いちいち、部下の進捗状況を都度聞く手間が省け、マネジメント業務の時間短縮が図れる。
2. 部下:日報・週報の作成を行い、自身のタイムマネジメント、業務の優先順位付けをアプリケーション通してを学び、習慣化することが可能となり、生産効率の向上を図ることが可能となる。
また、入力内容の集計結果を可視化する際にUI部分に力を入れ、見てて入力をしたくなる。


### 命名理由
１９９０年代の日本企業が世界的に最強だった時代をもう一度再建し、市場価値の高い人材、組織を育成していくための助けになればとの思いから作成。言葉の意味は、日本古来の言葉、「御恩と奉公」から取りました。

Go on（御恩）To（と）Service（奉公）というダジャレっぽい側面を意味に持たせており、使用いただく方々がこのアプリケーションを通し、楽しさを忘れずに日々の業務（仕事）に取り組んでほしい。という点から言葉遊びの要素を追加し、上司と部下がお互いにサービスし合う（※助け合う）（※思いやりを持って接する）、日本人としての伝統的な価値観を改めて強く認識するきっかけになればと思い、命名。

また、Go on to service　という一文をつなげることにより、「顧客や一般の人々にサービスを提供し続ける。（※社会の貢献をし続ける）」

という意味も持たせ、このアプリを通し、1人では達成できない業務に対し、チーム一丸となって達成に向かい走り続け、社会のために、また、会社の利益の為に貢献（Service）できるようになってほしいという願いも込めました。



# 設計概要
## 共通機能
### ユーザーアカウント管理
上司と部下それぞれのアカウントを作成し、ログイン機能を提供。
### ダッシュボード
上司と部下がホーム画面で直近の進捗やスケジュールを一覧できる。
### チームコラボレーション機能
チーム内でのコミュニケーションを促進する掲示板やコメント機能を導入。メッセージや質問のやりとりができる。
### ファイル共有
重要な資料やファイルをアップロードして、上司と部下で共有できるようにする。
### 目標設定と追跡
上司が部下に対して目標を設定し、進捗をトラッキングする機能を組み込む。進捗に応じてフィードバックを提供できる。


## 上司専用ページ
### 部下の報告一覧
部下が記入した日報・週報を一覧表示。フィルタリング機能を提供し、必要な情報に迅速にアクセスできるようにする。
### タスク分析と可視化
部下のタスクを集計し、円グラフや棒グラフなどで可視化。業務の進捗や課題の特定がしやすくなる。
### スケジュール通知
毎朝、部下のスケジュールやタスク予定をまとめて上司にメール通知。リマインダーとして利用可能。
## 部下専用ページ
### 日報・週報の記入
部下が日報・週報を入力できるフォームを提供。定型文や選択肢の導入で記入の効率向上。

### スケジュール管理
カレンダー形式でスケジュールを管理。重要な日程に関する通知やリマインダーを設定できる。
### 通知機能
今日のスケジュールや重要なタスクに関するメール通知。リアルタイムな情報共有が可能。
### 進捗報告
上司に向けて進捗報告を行うためのフォームを提供。プロジェクトの進行状況や課題点を共有できる。

