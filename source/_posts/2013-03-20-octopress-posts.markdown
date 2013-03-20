---
layout: post
title: "Octopress 普段やること"
date: 2013-03-20 18:31
comments: true
categories: 
---
##記事の更新方法
  普段の更新方法のメモ書き

* 新規記事の作成
```
$ rake new_post["Title"] # URLになる
mkdir -p source/_posts
Creating new post: source/_posts/2013-03-20-xxxxx.markdown
```

* ローカルでプレビューしながら
```
$ rake generate
$ rake preview
```
  http://localhost:4000で確認しながら編集できる。

* デプロイ
```
$ rake gen_deploy
```

* たまにはソースをプッシュしておく
```
$ git add .
$ git commit -m 'commit'
$ git push origin source #最初はこれ
$ git push # 次回以降
```
