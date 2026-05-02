# Personal Site

シンプルな1ページ構成のポートフォリオサイト。

## ファイル

- `index.html` — 本体
- `style.css` — スタイル（ダークモード自動対応）

## ローカルで確認

```bash
open index.html
```

## GitHub Pages にデプロイ

1. GitHub で新しいリポジトリを作成（例: `shuheikusachi.github.io` か任意名）
2. このフォルダの中身を push
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin git@github.com:[username]/[repo].git
   git push -u origin main
   ```
3. リポジトリの `Settings → Pages` で:
   - Source: `Deploy from a branch`
   - Branch: `main` / `/ (root)`
4. 数十秒で `https://[username].github.io/[repo]/` に公開される
   - リポジトリ名を `[username].github.io` にすると `https://[username].github.io/` がそのまま使える

## Private リポジトリで運用したい場合

- リポジトリは Private のまま、Pages だけ Public にできる（無料プランでOK）
- `Settings → Pages` で同じ設定をする

## 編集すべき箇所

`index.html` 内の以下を埋める:

- `[大学名]` `[研究室名]`
- `[username]` (GitHub)
- Google Scholar の `[link]`
- YouTube Downloader の GitHub リンク
- 顔写真: `photo.jpg` を置いて `<div class="photo-placeholder">` を `<img src="photo.jpg" />` に差し替え
