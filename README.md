# Portfolio Workspace

森下学のポートフォリオページ制作ワークスペース。
公開先：https://mozart1756bi-lab.github.io/portfolio0624/

---

## フォルダ構成

```
Portfolio/
├── CLAUDE.md              # Claude Code作業ルール（Claudeが最初に読む）
├── SKILL.md               # デザインプリセット定義集
├── README.md              # このファイル（人間向け）
├── index.html             # ポートフォリオページ本体
├── images/
│   └── profile.jpg        # プロフィール画像（差し替えはここを上書き）
└── presets/
    ├── business-blue.md   # ビジネス風（初期状態）
    ├── warm-earth.md      # 温かみ系
    ├── minimal-mono.md    # モノトーン
    └── creative-vivid.md  # クリエイティブ
```

---

## よくある操作の手順

### ① プロフィール画像を変更したい

1. 新しい画像を用意（できれば正方形、500px以上推奨）
2. `images/profile.jpg` を新しい画像で上書き（ファイル名は必ず `profile.jpg`）
3. ブラウザで確認 → GitHubリポジトリにも同じ `images/profile.jpg` をアップロード

**Claudeに依頼する場合の言い方**：
> 「profile.jpgを差し替えて、新しい画像は C:\Users\mozar\Desktop\新しい写真.jpg にあります」

---

### ② デザインを変えたい（プリセット切替）

Claudeに以下のように伝えるだけで、色・フォント・Hero画像・見出しトーンが一括で切り替わります：

```
プリセット warm-earth を適用して
```

利用可能なプリセット：
- `business-blue`（現在の初期状態・ネイビー×レッド）
- `warm-earth`（ベージュ×モスグリーン・エッセイ系向け）
- `minimal-mono`（白黒モノトーン・作品重視）
- `creative-vivid`（紫×コーラル・カジュアル案件向け）

---

### ③ 新しいデザインテーマを作りたい

Claudeに以下のように伝えれば、新規プリセットを作成してくれます：

```
「和モダン」の雰囲気の新しいプリセットを作ってください
```

`SKILL.md` の「プリセット追加ルール」に従って、Claudeが必要な項目を全部埋めて `presets/` にファイルを作ります。

---

### ④ ローカルで表示確認したい

コマンドプロンプトまたはPowerShellで以下を実行：

```bash
python -m http.server 3000 --directory "C:\Users\mozar\.claude\Portfolio"
```

ブラウザで http://localhost:3000/ にアクセス。
（サーバを止める時は `Ctrl+C`）

---

### ⑤ GitHubに反映したい

1. https://github.com/mozart1756bi-lab/portfolio0624 を開く
2. 変更したファイル（`index.html` や `images/profile.jpg`）をアップロード
   - GitHub上のファイルをクリック → 鉛筆マーク（Edit）→ 内容を書き換えて Commit
   - もしくは、Upload files でドラッグ＆ドロップして既存ファイルを上書き
3. 数十秒〜1分で https://mozart1756bi-lab.github.io/portfolio0624/ に反映

---

## Claudeへの依頼時のコツ

- **プリセット適用**：「プリセット XXX を適用して」
- **プロフィール画像変更**：「profile.jpgを C:\... の画像に差し替えて」
- **本文の書き換え**：「Introductionの2段落目を〇〇に変えて」など具体的に
- **新規プリセット**：「〇〇な雰囲気のプリセットを作って」

Claudeは `CLAUDE.md` のルールに従うため、勝手にリンクURLやプロフィール情報を変更したりはしません。

---

## 注意事項

- `images/profile.jpg` のファイル名は変えないこと（HTMLが参照しているため）
- GitHub Pages公開版とローカルの内容は自動同期されないため、ローカルで変更したら手動でGitHubへアップロードが必要
- Claudeが直接GitHubにPushやCommitをすることはありません（手動運用が前提）
