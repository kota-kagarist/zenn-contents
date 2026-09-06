# zenn-contents

Zennの記事をGitHubで管理するためのコンテンツリポジトリです。

## 接続状態

- このリポジトリは、ユーザーのZennアカウントと **Zenn Connectで連携済み**。
- GitHub側で記事を管理し、Zennへの反映はこの連携を前提に運用する。

## 方針

- 記事は `articles/` に置く。
- 新規記事は `published: false` で作成し、レビュー完了までは公開しない。
- ソフトウェアや実験データの正本は各プロジェクトのGitHubリポジトリに置き、このリポジトリには公開用の記事だけを置く。
- 実測値や比較結果は、元プロジェクトの検証済みデータから引用する。
- 記事の編集は原則としてブランチ + PRで行い、ZennのPRプレビューで表示確認してからmainへ反映する。
- コンテンツ全体の役割分担や執筆方針は [`EDITORIAL_POLICY.md`](./EDITORIAL_POLICY.md) にまとめる。

## 現在の下書き

- `articles/codex-japanese-renderer.md` — Codexで意味を確定し、Geminiに日本語の表面だけ整えさせるRendererの設計と実測

## プレビュー

Zenn Connect連携済みのため、記事変更のPRをZenn側の下書きプレビュー確認に使います。

ローカルでZenn CLIを利用できる場合は、リポジトリ直下で次も実行できます。

```bash
npx zenn preview
```

公開時は対象記事のFront Matterを確認したうえで `published: true` に変更します。
