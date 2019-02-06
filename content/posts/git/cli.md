---
title: "CLIでのGitの実行"
date: 2019-02-06T15:58:35+09:00
draft: false
---
CLIを使って以下の操作を行います。

* プロジェクトのクローン
* ブランチ作成
* ファイル修正
* コミット
* プッシュ

## インストール
homebrewとgitをインストールします。

### homebrewのインストール
[公式ドキュメント](https://brew.sh/)
```
// インストール
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

### homebrewを使ってgitをインストール
```
brew install git
```

## プロジェクトのクローン
Github上のプロジェクトをローカルにダウンロードします。

```
// 任意のフォルダに移動
cd {任意のパス}

// プロジェクトのクローン
git clone {レポジトリのURL}

// プロジェクトに移動
cd kintone-manual
```

## ブランチ作成
```
// 任意のブランチ作成
git checkout -b {任意のブランチ名}

// 新しく作成したブランチに移動していることを確認
git branch
```

## コミット
```
// 記事を作成（Markdown）
// VSCodeなどのを使って記事を作成する

// add
git add .

// コミット
git commit -m "{任意のメッセージ}"

// プッシュ
git push origin {先ほど自身で作成したブランチ名}
```
