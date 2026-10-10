# 「この子、大丈夫？」無料オンラインセミナーLP

2026年10月14日・24日開催のセミナー向けランディングページを、Canva AIの公開ページから軽量な静的サイトへ移植したものです。

## ファイル構成

- `index.html`：元のLPの見出し・文章・セクション順・3か所の申込み導線を再現。
- `style.css`：スマートフォン中心のレスポンシブデザイン。
- `images/hero.webp`：親子のヒーロー写真。
- `images/gift-book.webp`：申込み特典BOOK画像。
- `images/instructor.webp`：講師プロフィール画像。

画像は、利用者が提供した保存済みHTML内に記録されていた元Canva公開サイトの画像から自動取得し、GitHub上にWebP画像として保存したものです。

## 軽量化

Canvaの表示用iframe、編集SDK、巨大なJavaScriptバンドルを廃止。表示はHTML/CSSのみです。画像3点の合計サイズは約148KBです。日本語Webフォントは必要なウエイトだけGoogle Fonts経由で取得します。端末・ネットワーク別の表示速度は公開後に実測してください。

## 公開手順

GitHubのリポジトリ設定画面で `Settings → Pages → Build and deployment` の `Source` を `Deploy from a branch` にし、`main` ブランチ、`/(root)` を選択してSave。

Pagesが有効になれば通常 `https://twinkbaby-lang.github.io/konoko-daijobu-lp/` に公開されます。ただし、公開が完了するまではこのURLが有効とは限りません。

## 申込み導線：公開前の重要な確認

3か所のボタンは保存済みCanva AI本体のHTMLから取得した同一LIFF URLを使用しています。**URLの形式が存在することと、初めてアクセスする人が友だち追加・希望日選択・申込み完了まで到達できることは別です。**

Instagram内ブラウザ、LINE内ブラウザ、Safari/Chrome、未登録スマートフォンで実機検証してください。LINEアプリを開けない事象は、ホスティングだけの問題ではない可能性があります。

広告の遷移先はテスト完了後に変更してください。

元Canva LPと英語教室とぅいんくのリポジトリは変更していません。
