# Portfolio

情報科学・データサイエンス領域で、データ分析、ソフトウェア開発、検証可能なシステム設計を学んでいます。

関心領域は、データ分析、説明可能性、学習支援ツール、金融・市場分析、検証プロセスの設計です。

このGitHubプロフィールでは、制作物を以下の観点で整理します。

- 設計意図が説明できること
- 実装済みの範囲と未実装の範囲を分けて示すこと
- 検証手順、ログ設計、再現性を重視すること
- 実際に触れるWebアプリはデモURLを併記すること

## Projects

### trading-ea

研究・検証用の自動売買EAフレームワークです。

売買判断・リスク制御・実行・ログ・評価を分離し、判断過程を後から検証できる分析/検証基盤として設計しています。

主なポイント:

- `Data -> HTFContext -> LTFStructure -> Signal -> RiskFilter -> Execution -> Logger -> Evaluator` の責務分離
- dry-run によるログ整合確認
- no-real-order integrity の確認
- HTF diagnostic comparison
- Lot Sizing shadow comparison
- 実 broker / OANDA API / 実注文送信は未実装

Status:

- 公開準備中
- README / portfolio docs / interview pitch 整備済み
- 公開前に、不要データ・ローカルパス・secret の混入がないか最終確認予定

### English Reader Web

英語長文を読みながら、単語保存・既読管理を行う軽量な学習支援Webアプリです。

外部APIやクラウド同期に依存せず、HTML / CSS / JavaScript + localStorage で、小さく動く教材Webとして成立させることを目的にしています。

主なポイント:

- 英語長文一覧
- 長文詳細表示
- 単語保存
- 単語一覧
- 既読管理
- localStorage によるローカル保存

Status:

- 公開準備中
- Demo URL は GitHub Pages 等で公開後に追加予定
- Source repo は README 整備後に公開判断予定

## Portfolio policy

公開時には、成果を過大に見せないことを重視します。

特に、以下のような表現は使いません。

- 収益性確認済み
- 実運用可能
- 実注文対応済み
- broker接続済み
- OANDA API接続済み
- 完成済みEA

実装済みの範囲、検証済みの範囲、未実装の範囲を分けて説明します。

## Current focus

現在は、以下を優先して整備しています。

1. GitHubプロフィールをポートフォリオ入口として整える
2. `trading-ea` の公開前チェック
3. `English Reader Web` のデモ公開準備
4. 各プロジェクトの Demo / Source / Docs を整理
