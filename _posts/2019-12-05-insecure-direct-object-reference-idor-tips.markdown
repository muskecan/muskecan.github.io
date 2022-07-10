---
title: "Make IDOR great again!"
date: "2019-12-05"
category: blog
headerImage: true
tags: 
  - "bug-bounty-tips"
  - "critical-idor"
  - "how-to-make-idor-as-p1"
  - "idor"
  - "owasp"
  - "p1-idor"
image: /assets/posts/idor-tips-and-tricks-insecure-direct-object-reference.png
---

Hello folks, today I'll be sharing some important IDOR tips and tricks with you. This articled prepared in the lights of my past experiences, I hope it will be useful for the community!

## What the hell is IDOR?

Our friends at **OWASP** explained it for us long time ago. Here is the [full statement](https://www.owasp.org/index.php/Testing_for_Insecure_Direct_Object_References_(OTG-AUTHZ-004))

"Insecure Direct Object References occur when an application provides direct access to objects based on user-supplied input. As a result of this vulnerability attackers can bypass authorization and access resources in the system directly, for example database records or files.

**Insecure Direct Object References** allow attackers to bypass authorization and access resources directly by modifying the value of a parameter used to directly point to an object. Such resources can be database entries belonging to other users, files in the system, and more. This is caused by the fact that the application takes user supplied input and uses it to retrieve an object without performing sufficient authorization checks."

## Here is the IDOR tips and tricks!

Everybody say that IDOR vulnerability is kinda easy to exploit and has low or medium impacts. That means you are not gonna earn a lot of money from IDOR. **Totally Wrong.**

I guess almost everyone know that move function of the systems are perfect structure to find an **IDOR.** How about copy function? In almost every system, there is some file/folder move and copy function for some different purposes.

What i recommend is, you should go after from copy and move functions. If you can not be able to find IDOR on move function, try to copy some restricted content into your directory. For example pay checks, addresses, phone numbers, credentials almost every personal data is going to make it more valuable thanks to **GPDR.**

I want to share 2 IDOR adventures of my past experiences occured on copy function;

1. Accessing locked folders and contents of it. **PoC** :
    
    <iframe src="https://www.youtube.com/embed/HNZTT49IHkY" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe>
    
    As you can see, I can bypass locked folders by simply creating a copy of this folder.
2. Accessing all uploaded documents in the subdomain.I can say that this one is accepted as critical issue because everyone can access lots of personal data via simple **GET** requests. I can not share the full URL or detail about product but it was looking like this;  www.redacted.com/move.php?move=1&ID=XXXXXXXI tried to change ID parameter for random numbers but it didnt work. But I realised that Move parameter is also crucial. If I set it as 0, moving process turning into copying process and you can simply create a copy any file you want inside of your personal diskspace.

As a result, you should take a look copy functions for IDOR. I believe that you are gonna find lots of issues with my IDOR tips and tricks blogpost.
