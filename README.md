# Girls Bar no.18 ホームページ

池袋西口のガールズバー「no.18」の公式サイトです。HTML / CSS だけの静的サイトで、ビルドは不要です。

## ファイル構成

```
index.html        ページ本体（文章・料金表・求人・店舗情報など）
css/style.css     デザイン
img/              写真・ロゴ・求人バナー
netlify.toml      Netlify の公開設定
```

## よくある編集

| やりたいこと | 編集するファイル |
| --- | --- |
| 料金・営業時間・電話・SNS を入れる | `index.html` の「要確認」「入力」と書かれた箇所（`class="tbd"`） |
| 求人条件を変える | `index.html` の `id="recruit"` のセクション |
| 写真を差し替える | `img/` の同じファイル名で上書き |
| 色や文字の大きさ | `css/style.css` 冒頭の `:root` |

## 公開の仕組み

GitHub の `main` ブランチに変更を push すると、Netlify が自動で公開を更新します（ビルドコマンドなし、公開ディレクトリはリポジトリ直下）。

## 手元で確認する

```
python3 -m http.server 8000
```
を実行して http://localhost:8000 を開きます。
