---
name: review-and-push
description: Codex CLIでレビューし、問題なければcommit-pushする
---

# Review and Push

Codex CLIでレビューし、問題なければcommit-pushする。

## Steps

1. `/codex-review` スキルを実行
2. レビュー結果を確認:
   - 指摘あり → 修正してから再度 `/codex-review` を実行（指摘が解消されるまで繰り返す）
   - 指摘なし or 対応不要 → 次のステップへ
3. 未コミットの変更がある場合のみ `/commit-push` スキルを実行
