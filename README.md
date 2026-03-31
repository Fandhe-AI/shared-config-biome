# @fandhe-ai/shared-config-biome

Biome（リンター・フォーマッター）の共有設定。

## エクスポート

| パス | 説明 |
|------|------|
| `@fandhe-ai/shared-config-biome/core` | フォーマッタ設定（EditorConfig 連携） |
| `@fandhe-ai/shared-config-biome/root` | VCS 設定（Git / defaultBranch: main） |
| `@fandhe-ai/shared-config-biome/import` | インポート整理ルール（6 グループ） |

## 使用方法

`biome.jsonc` で `extends` に指定する:

```jsonc
{
  "extends": [
    "@fandhe-ai/shared-config-biome/core",
    "@fandhe-ai/shared-config-biome/root",
    "@fandhe-ai/shared-config-biome/import"
  ]
}
```

## 開発

### セットアップ

```bash
pnpm install
```

### コミット規約

[Conventional Commits](https://www.conventionalcommits.org/ja/) を採用。
[commitlint](https://commitlint.js.org/) + [lefthook](https://github.com/evilmartians/lefthook) により自動検証。

```
<type>: <description>

# 例
feat: 新しいルールを追加
fix: 設定の不具合を修正
chore: 依存関係を更新
```

## ライセンス

Copyright © Fandhe Inc.
