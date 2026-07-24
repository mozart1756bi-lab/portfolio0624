# Preset: minimal-mono

**用途**：作品を主役にしたい時、洗練された印象を出したい時
**印象**：シンプル、洗練、モダン

## CSS変数（ライトモード）
```css
--main-color: #1A1A1A;
--accent-color: #666666;
--bg-color: #FFFFFF;
--text-color: #1A1A1A;
--card-bg: #FAFAFA;
--header-bg: rgba(255, 255, 255, 0.95);
```

## CSS変数（ダークモード）
```css
--main-color: #FFFFFF;
--bg-color: #0A0A0A;
--text-color: #FFFFFF;
--card-bg: #1A1A1A;
--header-bg: rgba(10, 10, 10, 0.95);
```

## フォント
```html
<link href="https://fonts.googleapis.com/css2?family=Noto+Sans+JP:wght@300;400;700&family=Inter:wght@400;700&display=swap" rel="stylesheet">
```
```css
--font-jp: 'Noto Sans JP', sans-serif;
--font-en: 'Inter', sans-serif;
```

## Hero
- **画像URL**：`https://images.unsplash.com/photo-1557683316-973673baf926?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80`（グラデーショングレー）
- **Overlayカラー**：`rgba(26, 26, 26, 0.7)`
- **見出し**：
  ```html
  <h1>Craft. Words.<br>Clarity.</h1>
  ```

## アクセント色補足
- ホバー時の濃色版：`#333333`
- `.strong-point` 背景：`rgba(102, 102, 102, 0.08)`
