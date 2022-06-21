---
title: "BYPASS TWO FACTOR AUTHENTICATION VULNERABILITY ON LOGIN.GOV"
date: 2017-11-14 22:44
category: blog
layout: post
headerImage: true
tag: 
  - bug-bounty
  - bypass
  - bypass-2fa
  - bypass-two-factor-auth
  - bypass-two-factor-authentication
  - hack
  - hackerone
  - login-gov
  - muskecan
  - mustafa-kemal-can
  - vulnerability
image: /assets/posts/Bypass-two-factor-authentication.png
author: muskecan
---

I found a way to **bypass two factor authentication** on login.gov which contains critical informations in it. This vulnerability occurs because of the misconfigurated token.

The account creating process of login.gov is very interesting. You need to confirm your email first, instead of last. I realised that this might cause some security problems. And it has of course...

This is the vulnerable URL( I found this URL thanks to burp)

https://idp.staging.login.gov/sign\_up/enter\_password?confirmation\_token=XXX&request\_id=

All you need to insert your confirmation token you get from your email. It says "This link will expire in 24 hours." but it is not and I can be used multiple times. :)

[![Bypass two factor authentication on login.gov](images/Bypass-two-factor-authentication.png)](http://mustafakemalcan.com/wp-content/uploads/2017/11/Bypass-two-factor-authentication.png)

Because of the structure of this site, when you use vulnerable link, you'll directly in your account. Because server thinks that you didnt add phone information and set password. So how could it ask for a password or 2FA?

You can directly log in and **bypass two factor authentication** and if there is any account lock down.

## **Bypass two factor authentication and account lock down PoC :** 

<iframe width="560" height="315" src="https://www.youtube.com/embed/WkWRjkHrGWM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

You can see the original report on [hackerone in](https://hackerone.com/reports/264090) **[here](https://hackerone.com/reports/264090).**

- Aug 28th 2017 - I reported it on hackerone.
- Aug 30th 2017 - Hackerone said "this is not a vulnerability" ( Yeah, I said what the fuck too.)
- Sep 5th 2017 - After I emailed login.gov security team, hackerone reopened my issue.
- Nov 3rd 2017 - Issue has been fixed.
- Nov 3th 2017 - Waiting for disclose.
- Nov 18th 2017 - Report publicly disclosed.

Special thanks to Yunus YILMAZ
