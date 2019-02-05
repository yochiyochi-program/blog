## 概要
よちよちプログラミング部のブログ
* [url](https://yochiyochi-program.github.io/blog/)
* [github](https://github.com/yochiyochi-program/blog)

## 記事の作成方法
```
// hugo インストール
brew install hugo

// レポジトリ のクローン
git clone https://github.com/yochiyochi-program/blog.git

// クローンしたフォルダに移動
cd blog

// 記事作成
hugo new posts/{任意のファイル名}.md

// 上記で作成したファイルに記事を書く。
// 他の既存の記事なども参考にしながら書いてみてください。

// ローカルで確認
hugo serve -D

// 以下にブラウザでアクセスして確認してみてください。
http://localhost:1313/blog/

// Ctrl + D でサーバー停止

// デプロイ準備
// 以下のコマンドでhugoファイルがdocフォルダ配下に生成されます。
hugo

// デプロイ
git add .
git commit -m "hugo"
git push

// サイトを確認
// 以下の本番のサイトにアクセスして確認してください。
// 反映まで少し時間がかかることがあります。
// https://yochiyochi-program.github.io/blog/
```