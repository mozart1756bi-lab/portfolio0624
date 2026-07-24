# SKILL.md — ポートフォリオデザインプリセット

このファイルは、ポートフォリオページ（`index.html`）の見た目を「プリセット名」で切り替えるための定義集です。
Claudeはユーザーから「プリセット XXX を適用して」と依頼された時、このファイルとpresets/配下の該当ファイルを参照して `index.html` を書き換えます。

---

## 使い方（ユーザー向け）

```
「プリセット business-blue を適用して」
「プリセット warm-earth を適用して」
「プリセット minimal-mono を適用して」
「プリセット creative-vivid を適用して」
```

とClaudeに伝えるだけで、CSS変数・フォント・Hero画像・Hero見出しトーンが一括で切り替わります。

---

## プリセット一覧（サマリー）

| プリセット名     | 用途                     | 印象                     |
|----------------|-------------------------|--------------------------|
| business-blue  | BtoB向け・信頼感重視     | ネイビー×レッド×若葉、知的で爽やか |
| warm-earth     | note読者・エッセイ執筆   | ベージュ×モスグリーン、優しい |
| minimal-mono   | 作品を主役にしたい時     | 白黒モノトーン、洗練     |
| creative-vivid | カジュアル案件向け       | 紫×コーラル、遊び心      |

詳細は `presets/` 配下の各ファイル参照。

---

## プリセット定義（詳細）

### business-blue（現在の初期状態）
- **用途**：BtoB向け・信頼感重視・技術職アピール
- **CSS変数**：
  - `--main-color: #2C3E50`（ダークブルー）
  - `--accent-color: #E74C3C`（レッド）
  - `--bg-color: #F0F7EA`（若葉系ペールグリーン）
  - `--text-color: #2C3E50`
  - `--card-bg: #FFFFFF`
  - `--header-bg: rgba(240, 247, 234, 0.95)`
- **ダークモード**：
  - `--main-color: #ECF0F1`
  - `--bg-color: #1a252f`
  - `--text-color: #ECF0F1`
  - `--card-bg: #2C3E50`
  - `--header-bg: rgba(26, 37, 47, 0.95)`
- **フォント**：
  - Google Fonts: `Noto+Sans+JP:wght@400;500;700&family=Montserrat:wght@500;700`
  - `--font-jp: 'Noto Sans JP', sans-serif`
  - `--font-en: 'Montserrat', sans-serif`
- **Hero画像URL**：`https://images.unsplash.com/photo-1455390582262-044cdead277a?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80`（万年筆写真）
- **Hero見出し**：`Research, Logical and<br>Correct Writing`
- **Hero overlayカラー**：`rgba(44, 62, 80, 0.8)`

---

### warm-earth
- **用途**：note読者・エッセイ執筆者・旅行/メンタル系記事アピール
- **CSS変数**：
  - `--main-color: #4A3F35`（ダークブラウン）
  - `--accent-color: #8B7355`（モスグリーン系ブラウン）
  - `--bg-color: #F5F0E8`（ベージュ）
  - `--text-color: #4A3F35`
  - `--card-bg: #FFFDF9`
  - `--header-bg: rgba(245, 240, 232, 0.95)`
- **ダークモード**：
  - `--main-color: #F5F0E8`
  - `--bg-color: #2A241E`
  - `--text-color: #F5F0E8`
  - `--card-bg: #4A3F35`
  - `--header-bg: rgba(42, 36, 30, 0.95)`
- **フォント**：
  - Google Fonts: `Noto+Serif+JP:wght@400;500;700&family=Cormorant+Garamond:wght@500;700`
  - `--font-jp: 'Noto Serif JP', serif`
  - `--font-en: 'Cormorant Garamond', serif`
- **Hero画像URL**：`https://images.unsplash.com/photo-1523712999610-f77fbcfc3843?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80`（森の木漏れ日）
- **Hero見出し**：`Warm Words,<br>Real Stories`
- **Hero overlayカラー**：`rgba(74, 63, 53, 0.75)`

---

### minimal-mono
- **用途**：作品を主役にしたい時、洗練された印象を出したい時
- **CSS変数**：
  - `--main-color: #1A1A1A`
  - `--accent-color: #666666`
  - `--bg-color: #FFFFFF`
  - `--text-color: #1A1A1A`
  - `--card-bg: #FAFAFA`
  - `--header-bg: rgba(255, 255, 255, 0.95)`
- **ダークモード**：
  - `--main-color: #FFFFFF`
  - `--bg-color: #0A0A0A`
  - `--text-color: #FFFFFF`
  - `--card-bg: #1A1A1A`
  - `--header-bg: rgba(10, 10, 10, 0.95)`
- **フォント**：
  - Google Fonts: `Noto+Sans+JP:wght@300;400;700&family=Inter:wght@400;700`
  - `--font-jp: 'Noto Sans JP', sans-serif`
  - `--font-en: 'Inter', sans-serif`
- **Hero画像URL**：`https://images.unsplash.com/photo-1557683316-973673baf926?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80`（グラデーショングレー）
- **Hero見出し**：`Craft. Words.<br>Clarity.`
- **Hero overlayカラー**：`rgba(26, 26, 26, 0.7)`

---

### creative-vivid
- **用途**：カジュアル案件・エンタメ系・若年層向け訴求
- **CSS変数**：
  - `--main-color: #2D1B4E`（ディープパープル）
  - `--accent-color: #FF6B6B`（コーラル）
  - `--bg-color: #FFF9F0`（クリーム）
  - `--text-color: #2D1B4E`
  - `--card-bg: #FFFFFF`
  - `--header-bg: rgba(255, 249, 240, 0.95)`
- **ダークモード**：
  - `--main-color: #FFF9F0`
  - `--bg-color: #1A0F2E`
  - `--text-color: #FFF9F0`
  - `--card-bg: #2D1B4E`
  - `--header-bg: rgba(26, 15, 46, 0.95)`
- **フォント**：
  - Google Fonts: `M+PLUS+Rounded+1c:wght@400;500;700&family=Poppins:wght@500;700`
  - `--font-jp: 'M PLUS Rounded 1c', sans-serif`
  - `--font-en: 'Poppins', sans-serif`
- **Hero画像URL**：`https://images.unsplash.com/photo-1541701494587-cb58502866ab?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80`（カラフルなアート）
- **Hero見出し**：`Ideas that<br>Move Hearts`
- **Hero overlayカラー**：`rgba(45, 27, 78, 0.75)`

---

## プリセット追加ルール

新規プリセットを追加する時は、以下の項目を必ず埋めてから `presets/新プリセット名.md` を作成し、`SKILL.md` にも追記：

- **用途**（1行）
- **CSS変数 6つ**：--main-color, --accent-color, --bg-color, --text-color, --card-bg, --header-bg
- **ダークモード用 5つ**：--main-color, --bg-color, --text-color, --card-bg, --header-bg
- **フォント**：Google Fontsのファミリ指定文字列 + --font-jp, --font-en
- **Hero画像URL**：UnsplashなどのCDN URL（1920x1080程度）
- **Hero見出し**：`<h1>` タグ内のトーン語（`<br>` 改行込み）
- **Hero overlayカラー**：`rgba(R, G, B, 0.7〜0.85)` で背景写真の視認性を確保

---

## プリセット適用時のClaude作業手順

1. `SKILL.md` と `presets/対象プリセット.md` を読む
2. `index.html` の以下を書き換え：
   - `<link href="https://fonts.googleapis.com/css2?family=...">` のファミリ指定
   - `:root { ... }` 内の CSS変数6つ + フォント2つ
   - `[data-theme="dark"] { ... }` 内のダークモード用値5つ
   - `.hero { background-image: linear-gradient(...), url('...'); }` の overlay色とURL
   - `<h1>...</h1>` 内のHero見出しトーン語
3. 変更後、CLAUDE.md「5. プリセット適用時の報告フォーマット」の形式でチャット報告
