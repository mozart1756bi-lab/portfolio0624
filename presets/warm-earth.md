# Preset: warm-earth

**用途**：note読者・エッセイ執筆者・旅行/メンタル系記事アピール
**印象**：優しい、温かい、思索的

## CSS変数（ライトモード）
```css
--main-color: #4A3F35;      /* ダークブラウン */
--accent-color: #8B7355;    /* モスグリーン系ブラウン */
--bg-color: #F5F0E8;        /* ベージュ */
--text-color: #4A3F35;
--card-bg: #FFFDF9;
--header-bg: rgba(245, 240, 232, 0.95);
```

## CSS変数（ダークモード）
```css
--main-color: #F5F0E8;
--bg-color: #2A241E;
--text-color: #F5F0E8;
--card-bg: #4A3F35;
--header-bg: rgba(42, 36, 30, 0.95);
```

## フォント
```html
<link href="https://fonts.googleapis.com/css2?family=Noto+Serif+JP:wght@400;500;700&family=Cormorant+Garamond:wght@500;700&display=swap" rel="stylesheet">
```
```css
--font-jp: 'Noto Serif JP', serif;
--font-en: 'Cormorant Garamond', serif;
```

## Hero
- **画像URL**：`https://images.unsplash.com/photo-1523712999610-f77fbcfc3843?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80`（森の木漏れ日）
- **Overlayカラー**：`rgba(74, 63, 53, 0.75)`
- **見出し**：
  ```html
  <h1>Warm Words,<br>Real Stories</h1>
  ```

## アクセント色補足
- ホバー時の濃色版：`#6B5A44`（`.btn-submit:hover`など、現状の `#c0392b` を置換）
- `.strong-point` 背景：`rgba(139, 115, 85, 0.1)`
