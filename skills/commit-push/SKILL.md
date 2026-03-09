---
name: commit-push
description: ステージ済みのコード変更をgit commitし、pushします。実装完了時やユーザーがgit commitを依頼した時に使用します。
model: haiku
---

# コードの変更をコミットしてプッシュする

すべての出力・確認メッセージは日本語で行ってください。

# 手順

### ステップ1: 現在の状態を確認

```bash
git status
```

- ステージ済みの変更（`Changes to be committed`）がコミット対象です
- 未ステージの変更（`Changes not staged for commit`）がある場合は、ユーザーにそのまま続けるか確認してください

### ステップ2: コミット

```bash
git commit -m "..."
```

**コミットメッセージの形式：**

```
<type>: <subject>
```

- `feat` / `fix` / `refactor` / `test` / `docs` / `chore`
- subject は日本語、50文字以内、末尾ピリオドなし

### ステップ3: 確認

```bash
git log -1 --stat
```

### ステップ4: Push

```bash
git push origin HEAD
```
