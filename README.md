# zenn-contents

Zennの記事をGitHubで管理するためのリポジトリです。

## 方針

- 記事は `articles/` に置く。
- 新規記事は `published: false` で作成し、レビュー完了までは公開しない。
- ソフトウェアや実験データの正本は各プロジェクトのGitHubリポジトリに置き、このリポジトリには公開用の記事だけを置く。
- 実測値や比較結果は、元プロジェクトの検証済みデータから引用する。
- 本文は短く書き、必要のない英語ラベルや専門用語を増やさない。

## 現在の下書き

- `articles/codex-japanese-renderer.md` — Codexで内容を確定し、Geminiに日本語だけ整えさせる仕組みの設計と実測

## プレビュー

Zenn CLIを利用できる環境では、リポジトリ直下で次を実行します。

```bash
npx zenn preview
```

GitHub連携では、main向けPRの下書きデプロイを使って表示を確認します。

公開時は対象記事のFront Matterを確認したうえで `published: true` に変更します。
