# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

GitHub Pages個人サイト（yuki3738.github.io）。Jekyll + jekyll-theme-tactile テーマで構築。

## Commands

```bash
# ローカルサーバー起動
bundle exec jekyll serve

# 依存関係インストール
bundle install

# 依存関係更新
bundle update
```

`_config.yml` を変更した場合はサーバーの再起動が必要。

## Architecture

- **テーマ**: `jekyll-theme-tactile`（`_layouts/default.html` でオーバーライド済み）
- **レイアウト**: `_layouts/default.html` がベースレイアウト。GitHub Pages の View on GitHub ボタンやフッターの一部をコメントアウトでカスタマイズ
- **フッター**: `_includes/footer.html` にSNSアイコンリンク集（GitHub, Facebook, Twitter, Instagram, はてなブログ）
- **スタイル**: `assets/css/style.scss` でテーマをインポートし、SNSアイコンのスタイルを追加
- **ブランチ**: `master`（GitHub Pages のデプロイブランチ）
