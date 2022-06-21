---
title: "SMARTSHEET XSS VIA FILE UPLOAD"
date: "2017-12-26"
category: blog
headerImage: true
tags: 
  - "bug-bounty"
  - "cyber-security"
  - "file-upload-xss"
  - "muskecan"
  - "mustafa-kemal-can"
  - "smartsheet-xss"
  - "unathorized-xss"
  - "vulnerability"
  - "xss"
  - "xss-vulnerability"
coverImage: /assets/posts/smartsheet-xss.png
---

Hi, today I want to explain **XSS vulnerability** that I found on **Smartsheet.com**. **Smartsheet XSS vulnerability** is an interesting vulnerability because it occurs via **file upload**!

By the way I want to clarify that, this **XSS** works with or without authorization, so it is dangerous vulnerability as well as interesting.

## What is Smartsheet and more details about XSS!

[Smartsheet](https://www.smartsheet.com) is used to collaborate on project timelines, documents, calendars, tasks and other work. As of 2016, there were **10 million users in 85,000 organizations**. They have bug bounty program on bugcrowd. 

#### **How is happening Smartsheet XSS via file upload?**

Actually they have quite good program, it is easy to use and safe. But not too much :) We can trigger **XSS** vulnerability via upload an svg file with js codes in it.

They decided this [vulnerability](https://muskecan.github.io/bypass-two-factor-authentication-on-login-gov/) is out of scope because file goes to server and works at here. So **XSS** works on server, not on **Smartsheet.com**. Although they fixed the issue and I want you to know about this **vulnerability**.

Here is PoC;

<iframe width="560" height="315" src="https://www.youtube.com/embed/yQa32QNy9rY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
