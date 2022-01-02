---
title: "Markdown Common Elements"
layout: post
date: 2016-02-24 22:44
image: /assets/images/markdown.jpg
headerImage: false
tag:
- markdown
- elements
star: true
category: blog
author: johndoe
description: Markdown summary with different options
---

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
## Basic formatting
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
This note **demonstrates** some of what [Markdown][1] is *capable of doing*.
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
And that's how to do it.
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% highlight html %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
This note **demonstrates** some of what [Markdown][some/link] is *capable of doing*.
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% endhighlight %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
---
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
## Headings
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
There are six levels of headings. They correspond with the six levels of HTML headings. You've probably noticed them already in the page. Each level down uses one more hash character. But we are using just 4 of them.
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
# Headings can be small
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
## Headings can be small
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
### Headings can be small
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
#### Headings can be small
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% highlight raw %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
# Heading
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
## Heading
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
### Heading
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
#### Heading
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% endhighlight %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
---
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
## Lists
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
### Ordered list
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
1. Item 1
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
2. A second item
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
3. Number 3
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% highlight raw %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
1. Item 1
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
2. A second item
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
3. Number 3
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% endhighlight %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
### Unordered list
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
* An item
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
* Another item
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
* Yet another item
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
* And there's more...
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% highlight raw %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
* An item
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
* Another item
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
* Yet another item
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
* And there's more...
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% endhighlight %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
---
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
## Paragraph modifiers
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
### Quote
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
> Here is a quote. What this is should be self explanatory. Quotes are automatically indented when they are used.
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% highlight raw %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
> Here is a quote. What this is should be self explanatory.
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% endhighlight raw %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
---
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
## URLs
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
URLs can be made in a handful of ways:
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
* A named link to [Mark It Down][3].
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
* Another named link to [Mark It Down](https://google.com/)
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
* Sometimes you just want a URL like <https://google.com/>.
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% highlight raw %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
* A named link to [MarkItDown][3].
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
* Another named link to [MarkItDown](https://google.com/)
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
* Sometimes you just want a URL like <https://google.com/>.
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% endhighlight %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
---
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
## Horizontal rule
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
A horizontal rule is a line that goes across the middle of the page.
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
It's sometimes handy for breaking things up.
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% highlight raw %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
---
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% endhighlight %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
---
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
## Images
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
Markdown can also contain images. I'll need to add something here sometime.
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% highlight raw %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
![Markdowm Image][/image/url]
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% endhighlight %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
![Markdowm Image][5]
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
*Figure Caption*?
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% highlight raw %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
![Markdowm Image][/image/url]
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
<figcaption class="caption">Photo by John Doe</figcaption>
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% endhighlight %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
![Markdowm Image][5]
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
<figcaption class="caption">Photo by John Doe</figcaption>
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
*Bigger Images*?
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% highlight raw %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
![Markdowm Image][/image/url]{: class="bigger-image" }
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% endhighlight %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
![Markdowm Image][5]{: class="bigger-image" }
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
---
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
## Code
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
A HTML Example:
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% highlight html %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
<!DOCTYPE html>
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
<html lang="en">
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
<head>
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
    <meta charset="UTF-8">
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
    <title>Document</title>
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
</head>
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
<body>
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
    <h1>Just a test</h1>
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
</body>
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
</html>
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% endhighlight %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
A CSS Example:
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% highlight css %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
pre {
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
    padding: 10px;
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
    font-size: .8em;
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
    white-space: pre;
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
pre, table {
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
    width: 100%;
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
code, pre, tt {
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
    font-family: Monaco, Consolas, Inconsolata, monospace, sans-serif;
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
    background: rgba(0,0,0,.05);
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% endhighlight %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
A JS Example:
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% highlight js %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
// Sticky Header
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
$(window).scroll(function() {
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
    if ($(window).scrollTop() > 900 && !$("body").hasClass('show-menu')) {
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
        $('#hamburguer__open').fadeOut('fast');
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
    } else if (!$("body").hasClass('show-menu')) {
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
        $('#hamburguer__open').fadeIn('fast');
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
    }
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
});
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
{% endhighlight %}
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.

Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
[1]: https://daringfireball.net/projects/markdown/
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
[2]: https://www.fileformat.info/info/unicode/char/2163/index.htm
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
[3]: https://daringfireball.net/projects/markdown/basics
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
[4]: https://daringfireball.net/projects/markdown/syntax
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
[5]: https://kune.fr/wp-content/uploads/2013/10/ghost-blog.jpg
Hello everyone, today I'll be showing you very bad encrypted method that you shouldn't use for any kind of app/program.

## What is \[REDACTED\]?

It is a mobile game and is very popular especially in here, Turkey. As you can see the picture below, it is widely known word game. It is very similar to the scrabble game.

[![](images/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-10_26_52-1024x825-1.png)It has over 5 million downloads on Android side and ~100K ratings on iOS side.[![](images/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)](https://mustafakemalcan.com/wp-content/uploads/2020/03/Screen-Shot-2020-02-26-at-11_37_35-1024x726-1.png)

This app is on the market since 2013. It is an online game and you need to be online to use this app. I guess everyone thinks that their server is very secure, because they are managing tons of users.

## Who needs to access the servers?

Let's look at what is going on with the local storage. I have a jailbroken iPhone.

I noticed gameconfig.dat on this path -> /var/mobile/Containers/Data/Application/2F4D5AC7-000F-4D86-8C52-177C6162FB75/Documents . Let's have a look. -Please make sure that \[REDACTED\] Application is closed completely.-

> \==QflNHbhZmOiQWZ0ZWaH52bpNnclZ1byBnIsU2csFmZ6ICZld3boNFbhlmcvRXdUdWasJCLlVnc0pjIkV2chh2YyVHUy9GdhxWdjxWYjJCLlVnc0pjIkV2dvh2UsFWay9Gd1RVZtF2RulEdzJXamJCLlNHbhZmOiQWZzFGajJXdQV2ZkFmQlVmc0JCLlNHbhZmOiIXZtlGVlxGZpJCLlNHbhZmOiQWZzFGajJXdQR3cpxEZuVWayZmIsU2csFmZ6ICZlRnZpdEdzlGTk5WZpJnZiwSZzxWYmpjIkV2chh2YyVHUyVGduV3bDJXZ0RXZsJCLlNHbhZmOiQWZ0ZWaHJ3b0FGb1NGbhNmIs03M0QjOiQncvBnIsISbvNmLzBHchJTZo5iclZnclN3apxWZtlGbltmI6ICdz9GaisnOiIXZ2JXZTRHb1FmZlRmIsU2csFmZ6ICZlNXYoNmc1Blcvx2bDVWbhJnZiwSZzxWYmpjIkV2Yy9mRkJXYvJ0N4dzcpJCLlNHbhZmOiQWZ0ZWaHJ3bs92Ql1WYyZmIsAjOiAXbhR3cl1WaU5Wan9GTiZEdzFGbiwCM4cjN3AzM4UTM6ISZtlGVlh2YhN0b09GaQt2bvJWZjFmZiwSZzxWYmpjIkVGdml2Rl1WYHRWawFmciwSZ1JHd6ICZlxmYh5WRvR3boBnIsUWdyRnOiQWZ39GaTxWYpJ3b0VHVuVnU0NncpZmIsUWdyRnOi4WZlJ3YT9mZulUZtF2R39GazJCLlNHbhZmOic2bsFWaE1mclBlbvlGdhNWamlGdv50dvh2ciwSZ1JHd6ICZlxmYh5WR0FGaDVWbhdUbvRmbhJnIsUWdyRnOiQWZsJWYuVEdhh2Ql1WYH52bpRXY0lmdulmIsUWdyRnOiQWZsJWYuVEZuV3bzJCLlVnc0pjIzRHUklGbhZlbv5mIsU2csFmZ6ICZlRnZpdkclRnb192QyVGd0VGbiwSZ1JHd6IiblVmcjN1clxWdSVWbhdEdzFmR39GazJCLlVnc0pjIkVGbiFmbFlnch52bpR3YpRmIsIiI6Iiblt2bU52bpRXYjlmZpR3bOh2c1BnIsU2csFmZ6ICZlNXYoNmc1BVZtF2RklGchJnIsU2csFmZ6ICZlxmYh5WRkJXYvJEbsVnZiwCMwEjOiQnb19WbBFmchBnIsUWdyRnOiQWZzFGajJXdQ52bpNnclZ1byBnIsUWdyRnOiQWZsJWYuVUZnRWYiJye

Hmm. Let's write it backwards and apply base64decode and boom.

> {"badgeEnabled":true,"proVersionPurchased":true,"paraAmount":100,"fullBoardEnabled":false,"rapidGamePurchased":false,"pushNotificationToken":"","dictionaryEnabled":true,"showFastGameRulesScreen":true,"letterCounterGifted":false,"nonValidPts":true,"soundEnabled":true,"invitationGameChatEnabled":true,"randomGameChatEnabled":true,"showNotificationPermDialog":false,"showGameInfoScreen":true,"firstRunTutorialShowed":true,"photoEnabled":true,"rapidGameGifted":false,"facebookPhotoCacheTime":1583076780,"lastFbLoginTimestamp":0,"frameColorGifted":false,"is7x7BoardForced":false,"frameColorPurchased":false,"defaultServer":{"host":"redactedserver.he2apps.com","port":443},"calculatorGifted":false,"letterCounterPurchased":false,"friendListGifted":false,"friendListPurchased":false,"idleTimer":false,"treeBadgePurchased":false,"firstInGameTutorialShowed":true,"calculatorPurchased":true,"ligTutorialShowed":false,"proVersionGifted":false}

Everything is clear as crystal! Let's change the false values to true. Now it is time to see the magic, let's Base64Encode->spell it backwards->paste it into gameconfig.dat

Open the application and check the market tab inside of the game.

[![](images/IMG_A85EC742D897-1-650x1024-1.jpg)](https://mustafakemalcan.com/wp-content/uploads/2020/03/IMG_A85EC742D897-1-650x1024-1.jpg)

## How about Android?

Whole process is completely same. Root required. Gameconfig.dat is located under /data/data/com.he2apps.REDACTED/app\_data/

See ya!

NOTE : I know that, most probably REDACTED doesnt mean anything for you, but I need to do it :) You can still find the application if you want to see everything with your own eyes.
