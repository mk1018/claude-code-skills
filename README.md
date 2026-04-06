# Claude Code Skills

Claude Code で使用するカスタムスキル集です。

## スキル一覧

| スキル | コマンド | 説明 |
|--------|----------|------|
| [commit-push](skills/commit-push/SKILL.md) | `/commit-push` | 新しいブランチを作成し、変更をコミットしてプッシュし、PRを作成する |
| [review-and-push](skills/review-and-push/SKILL.md) | `/review-and-push` | Codex CLIでレビューし、問題なければcommit-pushする |
| [codex-review](skills/codex-review/SKILL.md) | `/codex-review` | Codex CLIで現在の変更をレビューし、指摘事項があれば修正する |
| [create-issues](skills/create-issues/SKILL.md) | `/create-issues` | 指示されたタスクからGitHub Issuesを作成する |

## セットアップ

```bash
# スキルをインストール
npx skills add mk1018/claude-code-skills
```

## 使い方

Claude Code のチャットで各スキルのコマンドを入力して実行します。

```text
/commit-push
/review-and-push
/codex-review
/create-issues
```
