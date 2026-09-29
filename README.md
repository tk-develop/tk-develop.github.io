# tk-develop.github.io

アプリの公開ページ（GitHub Pages）。`main` のいちばん上がそのまま https://tk-develop.github.io/ になる。

| ページ | URL |
|---|---|
| 家計予報 利用規約 | https://tk-develop.github.io/kakei-yoho/terms.html |
| 家計予報 プライバシーポリシー | https://tk-develop.github.io/kakei-yoho/privacy.html |

- 家計予報のアプリは、起動時の同意の画面と設定画面からこの 2 つを開く（`kakei-yoho` の KY-112。URL は `src/utils/budgetUtils.ts` の `TERMS_URL` / `PRIVACY_URL`）
- **制定日を変える（大切な変更をする）ときは、アプリ側の `TERMS_VERSION` も同じ日付に上げる。** 上げるとアプリが同意を取り直す
- 広告（AdMob）を入れるときは、このリポジトリのいちばん上に `app-ads.txt` を置く（`kakei-yoho` の KY-021）
- ほかのアプリのページを足すときは、`kakei-yoho/` と同じようにアプリごとのフォルダを作る
- `.nojekyll` は、GitHub Pages に Jekyll の変換をさせずにそのまま出すためのもの
