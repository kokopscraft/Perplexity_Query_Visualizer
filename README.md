# Perplexity Query Visualizer

> **日本語** | [English](#english)

Perplexity のレート制限 API レスポンス（JSON）を貼り付けるだけで、クエリ残数・データソース使用状況をビジュアルで確認できる、ブラウザで完結する静的 Web アプリです。

## 機能

- **プラン自動判別** — JSON の内容から Pro / Free を自動判定
- **KPI カード** — Pro クエリ / Labs クエリ / Research クエリ / Agentic Research の残数を一覧表示
- **ゲージチャート** — 半円ゲージで各クエリ残数を視覚化
- **データソース一覧** — `sources.source_to_limit` に含まれる全ソースの残数・上限をバー付きで表示
- **ダーク / ライトテーマ** — OS 設定に追従し、ボタンで手動切替も可能
- **日本語 / 英語 UI** — ヘッダーのボタンで即時切替
- **サーバー不要** — `index.html` 1 ファイルのみ、外部サーバーなしで動作

## 使い方

1. [perplexity.ai](https://www.perplexity.ai/) にログインした状態で以下の URL を開く
   ```
   https://www.perplexity.ai/rest/rate-limit/all
   ```
2. `Ctrl+A` → `Ctrl+C` でページのテキスト（JSON）を全選択コピー
3. `index.html` をブラウザで開き、テキストエリアに貼り付けて **「解析する」** をクリック

## 動作環境

- モダンブラウザ（Chrome / Firefox / Edge / Safari 最新版）
- サーバー不要・インストール不要

## ファイル構成

```
Perplexity_Query_Visualizer/
└── index.html   # アプリ本体（HTML + CSS + JavaScript をすべて含む）
```

## ライセンス

This project is provided as-is. See the repository for details.

---

<a name="english"></a>

# Perplexity Query Visualizer

> [日本語](#top) | **English**

A single-file static web app that visualizes your Perplexity rate-limit data. Just paste the JSON response from the rate-limit API endpoint and instantly see your remaining queries and data-source usage.

## Features

- **Automatic plan detection** — detects Pro / Free plan from the JSON content
- **KPI cards** — displays remaining counts for Pro queries, Labs queries, Research queries, and Agentic Research
- **Gauge charts** — semicircular gauges for each query type
- **Data source list** — shows all sources in `sources.source_to_limit` with remaining/limit bars
- **Dark / Light theme** — follows OS preference with a manual toggle button
- **Japanese / English UI** — switch languages instantly via the header button
- **No server required** — runs entirely in the browser from a single `index.html` file

## How to Use

1. While logged into [perplexity.ai](https://www.perplexity.ai/), open the following URL:
   ```
   https://www.perplexity.ai/rest/rate-limit/all
   ```
2. Press `Ctrl+A` then `Ctrl+C` to select and copy all the JSON text
3. Open `index.html` in your browser, paste the text into the textarea, and click **"Analyze"**

## Requirements

- Any modern browser (latest Chrome / Firefox / Edge / Safari)
- No server or installation needed

## File Structure

```
Perplexity_Query_Visualizer/
└── index.html   # Entire app (HTML + CSS + JavaScript in one file)
```

## License

This project is provided as-is. See the repository for details.
