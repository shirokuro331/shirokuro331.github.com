---
title: "Netlify + Hugo でサイト作る手順"
date: 2018-01-13T11:23:01+09:00

---

[Netlify](https://www.netlify.com/) を使えば GitHub に Hugo のファイル push すれば自動でビルドしてくれる。GitHub Pages でもできるけど Netlify 使ってみる。

## 用意するもの
- [Hugo](https://gohugo.io/) ファイル一式
  参照 : [Quick Start](https://gohugo.io/getting-started/quick-start/)
- [GitHub](https://github.com/) のアカウント
- [Netlify](https://www.netlify.com/) のアカウント
  - GitHub アカウントでサインインできる

## 手順
- 適当な GitHub repository をつくる
- Hugo のファイル一式を push する

        git clone :URL: https://github.com/shirokuro331/netlify-blog.git
        cd :categoryname:
        git add -A
        git commit -m "commitlog"
        git push origin master

- Netlify から GitHub の repository を選択する
- build の設定をする
  - Bransh : master
  - Build command : hugo --theme=hucore --buildDrafts
  - Publish directory : public/
  - うまくいかない場合 : [Netlify 上で使う Hugo のバージョンを指定する](https://monaural.net/post/201707/set-hugo-version-on-netlify/)

## まとめ

パフォーマンスが高い Netlify が簡単に使えるのは魅力的。今年はたくさんブログ書こう。うん。

