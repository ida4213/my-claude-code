# my-claude-code

自分用の Claude Code 設定をまとめたリポジトリです。

## ファイル構成

| ファイル | 説明 |
|---|---|
| `.mcp.json.example` | MCP サーバー設定のサンプル |

## セットアップ

### MCP サーバー設定

`.mcp.json.example` をコピーして `.mcp.json` を作成し、必要に応じて設定を編集します。

```bash
cp .mcp.json.example .mcp.json
```

`.mcp.json` は `.gitignore` に追加してシークレット情報を管理します。

### 利用可能な MCP サーバー（例）

| サーバー | 用途 |
|---|---|
| `terraform` | Terraform IaC の plan・validate・インフラ管理 |
| `figma` | Figma デザインデータの参照 |

## 注意事項

- MCP サーバーは有効にしすぎるとコンテキストウィンドウを圧迫します。10 個以内に抑えることを推奨します。
- プロジェクト単位で無効化する場合は `disabledMcpServers` を使用します。
