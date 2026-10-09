# TJA Zip Converter

zipをアップロードすると、以下を行って再zip化するサイトです(すべてブラウザ内で処理)。

- 画像ファイル(png / jpg / gif / bmp / webp / svg など)を全て削除
- `.tja` の `COURSE:` を `COURSE:Dan` に変更(なければ `SCOREMODE:` 行の下に追加。`SCOREMODE:` がなければ最初の `#START` の前)

## GitHub Pages で公開する手順

1. このフォルダの中身(`index.html` など)をリポジトリのルートにアップロード
2. リポジトリの **Settings → Pages** を開く
3. **Source** を `Deploy from a branch`、Branch を `main` / `/ (root)` にして Save
4. 数分後に `https://<ユーザー名>.github.io/<リポジトリ名>/` で公開されます

## 補足

- zip処理には [JSZip](https://stuk.github.io/jszip/) をCDN(cdnjs)から読み込みます。
