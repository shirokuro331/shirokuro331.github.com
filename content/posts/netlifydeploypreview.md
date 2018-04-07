---
title: "HUGO + Netlify 環境で deploy preview やる手順"
date: 2018-04-07T11:23:01+09:00

---

ブランチごとに Preview 用の URL 吐いてくれる deploy preview 使える Netlify まじ便利だ。

- ローカルで branch きる
- GitHub に add して commit して 新たにきった branch に push する
- GitHub で作った branch から pull request 作る  
![](/images/netlifydeploypreview/1.png "")  
![](/images/netlifydeploypreview/2.png "")
- pull request ができたら `Show all checks` というテキストをクリックして `Details` をクリックすれば preview 用がページ開く  
![](/images/netlifydeploypreview/3.png "")
- preview して問題なければ本番 branch  に merge する
- 公開

これだけ。ほんと便利。





