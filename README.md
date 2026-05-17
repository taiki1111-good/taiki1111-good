# Portfolio

情報科学・データサイエンス領域で、データ分析、ソフトウェア開発、検証可能なシステム設計を学んでいます。

関心領域は、データ分析、金融・市場分析、システム設計です。

このGitHubプロフィールでは、制作物を以下の観点で整理します。

- 何を目的に設計したのかを説明できること
- 実装済みの範囲と、まだ実装していない範囲を分けて示すこと
- 検証手順、ログ設計、再現性を重視すること
- 成果を過大に見せず、現在の到達点を明確にすること

## Main project

### trading-ea

研究・検証用の自動売買EAフレームワークです。

売買判断・リスク制御・実行・ログ・評価を分離し、判断過程を後から検証できる分析/検証基盤として設計しています。

このプロジェクトでは、収益性や実運用可能性を成果として主張するのではなく、設計、検証手順、ログ追跡、説明可能性を重視しています。

Links:

- Repository: https://github.com/taiki1111-good/trading-ea-portfolio
- Overview: https://github.com/taiki1111-good/trading-ea-portfolio/blob/main/docs/portfolio/portfolio_overview.md
- Architecture: https://github.com/taiki1111-good/trading-ea-portfolio/blob/main/docs/portfolio/architecture_for_portfolio.md

主なポイント:

- 売買判断、リスク制御、実行、ログ記録、評価を役割ごとに分離
- 実注文なしの模擬実行（dry-run）によるログ整合確認
- 実注文が送信されていないことの確認（no-real-order integrity）
- 上位足条件やロット計算を、本体に組み込む前に診断・比較する設計
- 実際のブローカー接続、実注文送信は未実装

Status:

- 公開用 repository 作成済み
- README と `docs/portfolio/*` を主な説明導線として整理済み
- 現段階においては研究・検証用フレームワークであり、実運用を目的とした完成済みEAではありません

## Other projects

### English Reader Web

英語長文を読みながら、単語保存・既読管理・復習を行う軽量な学習支援Webアプリです。

外部APIやクラウド同期に依存せず、HTML / CSS / JavaScript と `localStorage` を使って、ブラウザ上で動く学習ツールとして作成しています。

Links:

- Demo: https://taiki1111-good.github.io/english-reader-web-portfolio/
- Repository: https://github.com/taiki1111-good/english-reader-web-portfolio

主なポイント:

- 英語長文一覧と読解画面
- 単語・語句の保存
- 単語帳、復習、フラッシュカード
- 文型・文法ラベルの確認機能
- `localStorage` によるローカル保存

Status:

- GitHub Pages で公開済み
- 静的Webアプリとして動作
- 今後も教材・UI・復習機能を段階的に改善予定

## Public description policy

公開時には、実装済みの範囲、検証済みの範囲、未実装の範囲を分けて説明します。

特に、まだ実装していない機能を、実装済みのように表現しないことを重視します。

例:

- 収益性を確認した段階ではないため、収益性を成果として主張しない
- 実注文送信は未実装のため、実運用可能なEAとしては表現しない

## Current focus

現在は、以下を優先して整備しています。

1. `trading-ea` の公開用repositoryと説明導線の最終確認
2. `English Reader Web` の公開デモと説明導線の整備
3. 各プロジェクトの公開向け説明を、実装範囲と未実装範囲が分かる形に整理
