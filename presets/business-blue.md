# Preset: business-blue

**用途**：BtoB向け・信頼感重視・技術職アピール（現在の初期状態）
**印象**：知的、堅実、爽やか

## CSS変数（ライトモード）
```css
--main-color: #2C3E50;      /* ダークブルー */
--accent-color: #E74C3C;    /* レッド */
--bg-color: #F0F7EA;        /* 若葉系ペールグリーン */
--text-color: #2C3E50;
--card-bg: #FFFFFF;
--header-bg: rgba(240, 247, 234, 0.95);
```

## CSS変数（ダークモード）
```css
--main-color: #ECF0F1;
--bg-color: #1a252f;
--text-color: #ECF0F1;
--card-bg: #2C3E50;
--header-bg: rgba(26, 37, 47, 0.95);
```

## フォント
```html
<link href="https://fonts.googleapis.com/css2?family=Noto+Sans+JP:wght@400;500;700&family=Montserrat:wght@500;700&display=swap" rel="stylesheet">
```
```css
--font-jp: 'Noto Sans JP', sans-serif;
--font-en: 'Montserrat', sans-serif;
```

## Hero
- **画像URL**：`https://images.unsplash.com/photo-1455390582262-044cdead277a?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80`（万年筆写真）
- **Overlayカラー**：`rgba(44, 62, 80, 0.8)`
- **見出し**：
  ```html
  <h1>Research, Logical and<br>Correct Writing</h1>
  ```
