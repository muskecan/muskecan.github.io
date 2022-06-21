---
title: "First Touch Games database information leak"
date: "2018-02-09"
categories: 
  - "articles"
tags: 
  - "database-information-leak"
  - "first-touch-games-vulnerability"
  - "fts"
  - "fts-2017"
  - "fts-2018"
  - "muskecan"
  - "mustafa-kemal-can"
  - "vulnerability"
coverImage: "first-touch-games-database-leak.jpg"
---

Hi everyone in this post I'll show you how I find out **[First Touch Games](http://www.firsttouchgames.com) database information**. It is actually happens because of a common mistake. Let's see.

**FTS** is a **populer football game** which is available on Android and iOS platforms. I dont know why but they are still using very old version of **Wordpress** regularly. I used **WpScan** tool in **kali linux**. Actually this vulnerability revealed too easy to me. But I want to let you know.

In my opinion they forgot this file when they are in upgrading their website. But **wp-config** is crucial file that no one should see. I hope they will remove it and won't do that again.

[![first touch games database 2](images/first-touch-games-database-268x300.jpg)](https://mustafakemalcan.com/wp-content/uploads/2018/02/first-touch-games-database.jpg)

Here is the proof of file. I blurred all of the valuable informations.

## Status : 

1 January 2018 - I reported the issue, but there is **no response.**
