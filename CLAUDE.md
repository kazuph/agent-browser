# agent-browser (fork)

## 最重要ルール

> **絶対に本家（vercel-labs/agent-browser）にPRを作成しないこと**

このリポジトリは vercel-labs/agent-browser のフォークです。
WebClass操作に必要なポップアップ追跡・iframe対応の改造を加えています。

## 改造内容

1. **ポップアップ自動追跡**: launch/newWindow時に `context.on('page')` を登録し、`window.open()` で開いたページを自動追跡・自動切り替え
2. **iframe内eval対応**: `evaluate` コマンドが `activeFrame` 内で実行されるように修正
