# PayNote アイコンセット

クレジットカード利用記録 PWA「PayNote」用のアイコン一式。

## ファイル構成

**SVG ソース**
- `icon.svg` — ベース（140×140、角丸 rx=32）
- `icon-maskable.svg` — Android 適応アイコン用（175×175、フルブリード）

**PWA / モバイル PNG**
- `icon-192.png`, `icon-512.png` — manifest.json の標準アイコン
- `icon-maskable-192.png`, `icon-maskable-512.png` — Android maskable 用
- `apple-touch-icon.png` — iOS ホーム画面追加用（180×180）

**Favicon**
- `favicon-16.png`, `favicon-32.png`, `favicon-48.png`
- `favicon.ico` — 16/32/48 のマルチ解像度

**設定ファイル**
- `manifest.json` — PWA マニフェスト（theme_color, icons 設定済み）
- `head-snippet.html` — `<head>` に貼り付けるリンクタグ集

## カラーパレット
- 背景 / アクセント: `#1E3A8A`
- 後方カード（奥）: `#3B82F6`
- 後方カード（中）: `#60A5FA`
- 前面カード: `#FFFFFF`

## 組み込み手順
1. ファイルをサイトのルート（または任意の `/icons/` 配下）に配置
2. `head-snippet.html` の内容を HTML の `<head>` 内に挿入
3. ルート以外に置く場合は `manifest.json` 内の `src` パスとリンクタグの `href` を調整
