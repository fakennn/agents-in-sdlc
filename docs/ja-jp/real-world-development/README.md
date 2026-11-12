---
title: "実践的な開発"
slug: ja-jp/real-world-development
authors:
  - geektrainer
lastUpdated: 2026-09-16
---

現実的なシナリオ、完全なアプリケーション、共有バックログを使って、ソフトウェア開発ライフサイクル全体で GitHub Copilot を活用します。変更の計画、コードの作成、動作のテスト、プルリクエストのレビュー、エージェントを使った作業管理を繰り返し行います。

## シナリオ

架空の企業 Tailspin Toys に入社したばかりの開発者です。同社は開発者をテーマにしたボードゲームのクラウドファンディングを提供しています。チームのバックログは GitHub issue として登録済みで、すぐに着手できます。フィルターやページネーションなどの機能開発に加え、アクセシビリティやコーディング標準などの品質向上も含まれています。

## 環境を選択する

GitHub Copilot は、どこで作業していても利用できます。自分の開発スタイルに合った環境を選択してください。各ワークショップは独自のセットアップから始まり、共通の Tailspin Toys シナリオを使用します。

### [GitHub Copilot CLI][cli]

ターミナルでエージェント型アシスタントを使います。Plan モードと Autopilot モード、指示、スキル、カスタム エージェント、Playwright MCP、Agent Merge、便利なスラッシュ コマンドを活用します。

### [GitHub Copilot アプリ][app]

エージェント セッションを並行して実行し、セッション モードを切り替え、Canvas で共同作業し、デスクトップ アプリで GitHub issue とプルリクエストを管理します。

### [GitHub Copilot クラウド エージェント][cloud]

GitHub issue を非同期エージェントに割り当て、その作業を導き、進捗を監視し、エージェントが作成したプルリクエストをレビューします。

### [Visual Studio Code][vscode]

Visual Studio Code と GitHub Codespaces で GitHub Copilot を使います。エディターを離れずに、Copilot Chat のエージェント モード、MCP サーバー、カスタム エージェントを活用します。

[cli]: cli/
[app]: app/
[cloud]: cloud/
[vscode]: vscode/
