---
title: "Do not trust on what comes as default"
layout: post
date: 2022-09-24 22:44
headerImage: false
tag:
- markdown
- elements
category: blog
author: muskecan
---

I'd like to share an interesting research with you. It is related to one of the biggest ISPs in Estonia and Finland. I am one of the customers of this company and pretty happy with their services.

## What is the issue?

The issue is related to the default configuration of the router firmware which is left unchanged by most people. By default, the SSID is composed of 6 alphanumeric characters. So, it is pretty easy to point customers of the ISP who use the default configuration. I will talk about this later.

How about the default password? Well, this is where the story begins. By default, the password comes with a length of 9 characters. BUT, it is onlycomposed of numbers.

This means that it takes approximately 30 mins to crack it up. All you need to do is to create a wordlist for all the combinations. The size of the wordlist is only 9GB.

Default configurations are not the most security-oriented thing in the universe but they should comewith at least a decent level of security to protect customers from potential attacks. In this case, unfortunately, there is a big security hole and to be honest, the impact is huge

## How about the possible impact?

If a user uses the default SSID and password, it is highly likely that the login credentials of the router management panel are also left on default settings. Basically, an attacker can have administrator privileges on the customer's router. What is going to happen if the attacker changes the DNS settings of the router or adds a VPN configuration for your default connection? Oh, this seems bad.

I used my awesome(?) Python skills and created a tool to demonstrate the number of potentially vulnerable routers. Unfortunately I can not share the source code.

The code does not do any harmful activities. I used 2 basic regexes to detect default SSIDs and the script prints it out with the percentage information.

 <img class="image" src="{{ site.url }}/assets/posts/python-script.png">

I have conducted my tests in seven different and random streets in the city. I will not share the nameof the streets, nor SSIDs. But I can share the overall percentage of the results.

The results were shocking even for me. I was expecting to see something around 20% but in the end, the reality was much higher than that.

 <img class="image" src="{{ site.url }}/assets/posts/graph.png">

37% of the routers in random 7 different streets in the city were vulnerable due to the insufficient default firmware that ISP routers have.

## Mitigation?

Well, mitigation recommendations are pretty obvious. Default passwords should not be composed of only numbers. Instead, alphanumeric default passwords with a longer length would be enough for a default configuration. But changing the password for every user with a new firmware update? Noone will install such an update in the end...

How about the usage of ISP's remote configuration capabilities? This is something that can only be done by the ISP. But the ISP should contact their customers before such an operation. Otherwise, the customers would not be able to access the Internet.

In my opinion, considering both of the options, the mitigation process will take quite a bit of time.