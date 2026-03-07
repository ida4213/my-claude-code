# Git ワークフロー

## コミットメッセージの形式
```
<type>: <description>

<optional body>
```

タイプ: feat, fix, refactor, docs, test, chore, perf, ci

注意: コミットへの帰属表示は `~/.claude/settings.json` でグローバルに無効化されています。

## プルリクエストのワークフロー

**PR 作成時の手順**
1. 最新のコミットだけでなく、コミット履歴全体を分析する
2. `git diff [ベースブランチ]...HEAD` で全変更内容を確認する
3. 包括的な PR サマリーを作成する
4. TODO を含むテスト計画を記載する
5. 新しいブランチの場合は `-u` フラグを付けてプッシュする
