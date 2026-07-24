# Preset: creative-vivid

**用途**：カジュアル案件・エンタメ系・若年層向け訴求
**印象**：明るい、遊び心、親しみやすい

## CSS変数（ライトモード）
```css
--main-color: #2D1B4E;      /* ディープパープル */
--accent-color: #FF6B6B;    /* コーラル */
--bg-color: #FFF9F0;        /* クリーム */
--text-color: #2D1B4E;
--card-bg: #FFFFFF;
--header-bg: rgba(255, 249, 240, 0.95);
```

## CSS変数（ダークモード）
```css
--main-color: #FFF9F0;
--bg-color: #1A0F2E;
--text-color: #FFF9F0;
--card-bg: #2D1B4E;
--header-bg: rgba(26, 15, 46, 0.95);
```

## フォント
```html
<link href="https://fonts.googleapis.com/css2?family=M+PLUS+Rounded+1c:wght@400;500;700&family=Poppins:wght@500;700&display=swap" rel="stylesheet">
```
```css
--font-jp: 'M PLUS Rounded 1c', sans-serif;
--font-en: 'Poppins', sans-serif;
```

## Hero
- **画像URL**：`https://images.unsplash.com/photo-1541701494587-cb58502866ab?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80`（カラフルなアート）
- **Overlayカラー**：`rgba(45, 27, 78, 0.75)`
- **見出し**：
  ```html
  <h1>Ideas that<br>Move Hearts</h1>
  ```

## アクセント色補足
- ホバー時の濃色版：`#FF5252`
- `.strong-point` 背景：`rgba(255, 107, 107, 0.1)`
