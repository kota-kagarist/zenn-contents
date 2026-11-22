# zenn-contents

Zennの記事をGitHubで管理するためのコンテンツリポジトリです。

## 方針

- 記事は `articles/` に置く。
- 新規記事は `published: false` で作成し、レビュー完了までは公開しない。
- ソフトウェアや実験データの正本は各プロジェクトのGitHubリポジトリに置き、このリポジトリには公開用の記事だけを置く。
- 実測値や比較結果は、元プロジェクトの検証済みデータから引用する。
- 記事の編集は原則としてブランチ + PRで行い、ZennのPRプレビューで表示確認してからmainへ反映する。

## 現在の下書き

記事ごとの編集判断とレビューの残件は[編集中のプルリクエスト](https://github.com/kota-kagarist/zenn-contents/pulls)で確認できます。作業を引き継ぐときは、対象記事のプルリクエストに、採用した修正と次に確認する箇所を残します。

- [CodexとGeminiを使った日本語編集の下書き](articles/codex-japanese-renderer.md) — Codexで意味を確定し、Geminiに日本語の表面だけ整えさせるRendererの設計と実測

## プレビュー

GitHub連携後は、記事変更のPRをZenn側の下書きプレビュー確認に使います。

ローカルでZenn CLIを利用できる場合は、リポジトリ直下で次も実行できます。

```bash
npx zenn preview
```

公開時は対象記事のFront Matterを確認したうえで `published: true` に変更します。
