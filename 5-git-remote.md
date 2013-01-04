---
layout: default
permalink: remote.html
title: ihower 的 Git 教室
---

## Git 團隊協同開發指令

上一章介紹了在本地端用`git init`初始了一個*Repository*。不過，比較常的情況是你是從拷貝一個已經存在的 Repository 開始開發。Git 有以下四種方法來存取遠端的*Git*伺服器：

* SSH 安全性最佳


[GitHub](http://github.com) 是基於 Git 這套分散式版本控制系統的 Repository hosting 應用，只要是開放原始碼軟體，都可以免費的使用這個服務。這裡就使用*Github*來進行練習：

### 在 Github 上建立一個專案

編輯專案的 Settings，加入別人成為你專案的 Collaborators。這樣別人就可以用 SSH 協定來 clone 你的專案。


以筆者的專案 [Sandbox](https://github.com/ihower/sandbox) 為例，如果你有寫入權限的話(被加入成Collaborators)，就可以用 SSH 協定 Clone 下來：

	git clone git@github.com:ihower/sandbox.git

如果有防火牆問題，改用 HTTPS 協定：

	git clone https://github.com/ihower/sandbox.git
### Pull - 從遠端更新	


> 所謂的"遠端"預設叫做*origin*，當你有多個不同遠端伺服器時，就會取不同名子了。
  
### Push - 將 Commit 送出去

	git push 或 git push origin master
	


### 列出和取出遠端 branch

	git branch -r



### git push --tags	

	預設不會 push tags 資訊


