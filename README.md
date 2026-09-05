# zenn-content-

Zennの記事をGitHubで管理するための公開用コンテンツリポジトリです。

## 方針

- 記事は `articles/` に置く。
- 新規記事は `published: false` で作成し、レビュー完了までは公開しない。
- ソフトウェアや実験データの正本は各プロジェクトのGitHubリポジトリに置き、このリポジトリには公開用の記事だけを置く。
- 実測値や比較結果は、元プロジェクトの検証済みデータから引用する。

## 現在の下書き

- `articles/codex-japanese-renderer.md` — Codexで意味を確定し、Geminiに日本語の表面だけ整えさせるRendererの設計と実測

## プレビュー

Zenn CLIを利用できる環境では、リポジトリ直下で次を実行します。

```bash
npx zenn preview
```

公開時は対象記事のFront Matterを確認したうえで `published: true` に変更します。
