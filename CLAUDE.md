# CLAUDE.md — Portfolio作業ルール

このフォルダは、ユーザー（森下学）のポートフォリオページ制作用ワークスペースです。
公開先：https://mozart1756bi-lab.github.io/portfolio0624/
Claude Codeは、このフォルダで作業する際、以下のルールを必ず守ってください。

---

## 1. 作業前に必ず読むべきファイル

1. このファイル（`CLAUDE.md`）
2. `SKILL.md`（デザインプリセットの定義集）
3. 対象プリセットのファイル（例：`presets/business-blue.md`）

---

## 2. 編集対象の原則

- **編集していいのは原則 `index.html` のみ**
- プリセット適用時に書き換える箇所は、次の3つに限定：
  1. `<link href="https://fonts.googleapis.com/css2?family=...">` の Google Fonts 指定
  2. `<style>` セクション内の `:root { ... }` の CSS変数（--main-color, --accent-color, --bg-color, --text-color, --card-bg, --header-bg, --font-jp, --font-en）
  3. `<style>` セクション内の `.hero { background-image: ... }` の Hero画像URL
  4. Hero部分の見出し（`<h1>` タグ内のトーン語）
  5. `[data-theme="dark"]` のダークモード対応値

**上記以外のHTML構造・スクリプト・リンク先URL・本文コンテンツは、明示的な依頼がない限り触らない**

---

## 3. プロフィール画像の扱い

- 画像パスは `images/profile.jpg` 固定
- **HTMLの `<img src="images/profile.jpg" ...>` は絶対に変更しない**
- 画像を変えたい時は、ユーザーが `images/profile.jpg` を上書きする運用
- Claudeが別のファイル名を提案してはいけない

---

## 4. リンク先URLの扱い

以下のリンクは実案件・実プロフィールに紐づくため、勝手に変更しない：
- クラウドワークス プロフィール
- note 記事
- Google Docs / Slides の共有URL
- Twitter/X アカウント

これらを更新する場合は、ユーザーから明示的なURLの提示を受けてから修正。

---

## 5. プリセット適用時の報告フォーマット

プリセットを適用したら、必ずチャットで以下を報告：

```
プリセット「XXX」を適用しました。
変更点：
- CSS変数：--main-color を #XXX → #YYY へ変更（他N箇所）
- フォント：AAA → BBB へ変更
- Hero画像：既存URL → 新URL
- Hero見出し：「旧トーン語」→「新トーン語」
```

---

## 6. GitHub Pages 公開版との整合性

- ユーザーはローカル変更後、手動でGitHubにアップロードする
- ファイル分割（例：CSS外部化、JS外部化）は原則しない。単一 `index.html` を維持
- 相対パスは `images/profile.jpg` のようにルート相対の書き方はせず、そのまま相対で
- Claudeが直接GitHubへPushやCommitを行うことはしない

---

## 7. 新規プリセット追加の依頼を受けたら

1. `SKILL.md` の「プリセット追加ルール」に従って必要項目を定義
2. `presets/新プリセット名.md` を新規作成
3. `SKILL.md` の「プリセット一覧」にも追記
4. ユーザーが「適用して」と言うまで、`index.html` は書き換えない

---

## 8. 変更前後の確認

大きな変更（プリセット切替・レイアウト調整）を行った場合は、ユーザーに「ブラウザで確認してください」と促し、必要ならローカルhttpサーバの起動コマンドを案内：

```bash
python -m http.server 3000 --directory "C:\Users\mozar\.claude\Portfolio"
```

→ http://localhost:3000/ で確認

---

## 9. やってはいけないこと

- `images/profile.jpg` のファイル名変更
- HTML内の実リンクURL（案件先）の書き換え
- 単一index.htmlの複数ファイル分割
- Claudeが勝手にGitHub Pushや外部への公開作業を行うこと
- ユーザーの経歴・プロフィール情報（25年、18件、稼働時間等）の勝手な変更
