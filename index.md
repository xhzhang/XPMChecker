---
layout: page
title: Home
weight: 0
---

###  XPMChecker 

#### Abstract
Mobile apps have become the main channel for accessing Web services. Both Android and iOS feature in-app Web browsers that support convenient Web service integration through a set of Web resource manipulation APIs. Previous work have revealed the attack surfaces of Web resource manipulation APIs and proposed several defense mechanisms. However, none of them provides evidence that such attacks indeed happen in the real world, measures their impacts, and evaluates the proposed defensive techniques against real attacks.

This paper seeks to bridge this gap with a large-scale empirical study on Web resource manipulation behaviors in real-world Android apps. To this end, we first define the problem as cross-principal manipulation (XPM) of Web resources, and then design an automated tool named XPMChecker to detect XPM behaviors in apps. Through a study on 80,694 apps from Google Play, we find that 49.2% of manipulation cases are XPM, 4.8% of the apps have XPM behaviors, and more than 70% XPM behaviors aim at top Web sites. More alarmingly, we discover 21 apps with obvious malicious intents, such as stealing and abusing cookies, collecting user credentials and impersonating legitimate parties. For the first time, we show the presence of XPM threats in real-world apps. We also confirm the existence of such threats in iOS apps. Our experiments show that popular Web service providers are largely unaware of such threats. Our measurement results contribute to better understanding of such threats and the development of more effective and usable countermeasures.

---


####  Dataset

The dataset of XPMChecker contains 84,712 Google Play apps downloaded during Jul, 2017.  
These apps are selected with more than 5,000 installations across 48 categories.


Discovered malicious XPM behaviors with different aims: impersonating relying party in OAuth (A1, 2 apps), stealing user credentials (A2, 6 apps), stealing cookies (A3, 14 apps). One app named InstaView exhibits both A1 and A2 behaviors.


Package Name | Installations | Malicious Behavior | Description | APK MD5
---|---|---|---|---|---
com.chatous.chatous | 10M-50M | A3 | steal Facebook cookies and abuse cookies to send spam messages | [d8726437e1f2bbe17257c4eac6707bee]()
com.chatous.plaza | 1M - 5M | A3 | steal Facebook cookies and abuse cookies to send spam messages | [e5c4ec654e6f97a95ec5eed7afdd961d]()
com.melonapps.melon | 5M - 10M | A3 | steal Facebook cookies and abuse cookies to send spam messages | [36513949c9fb8dd2f979354ddd058b60]()
com.chatous.pointblank | 10M - 50M | A3 | steal Facebook cookies and abuse cookies to send spam messages | [a43529aa32363c480abb1cf013d29cdf]()
com.vendiste.app | 100K - 500K | A3 | steal Facebook cookies and abuse cookies to send spam messages | [5a4c48925fd42f6ee2376f088184e925]()
com.litefbwrapper.android | 100K - 500K | A3 | steal Facebook cookies and abuse cookies to receive account’s notifi- cation | [71e290121dddd0099d766685bf89a479]()
com.instaview.app | 1M - 5M | A1 & A2 | Impersonating Tinder in Instagram OAuth & inject JavaScript to steal user’s Instagram credentials | [b354aafb7f86e7ebc629a767d29f886a]()
com.kingsoft.email | 100K - 500K | A2 | inject JavaScript to steal user’s QQ Email credentials | [c3501cbb6f0caa3c2655de2713afad3a]()
co.kr.adkingkong | 500K - 1M | A2 | inject JavaScript to steal user’s google plus credentials | [26fe73ee8a33d2a0112215cf10d97c8b]()
com.dmf.wall. DMFPanoLwpF | 100K - 500K | A3 | steal flickr cookies to login auto- matically | [e85a5e17f96ed57c9eb229234f4abaa2]()
ru.like.vs | 100K - 500K | A3 | steal vk cookies to request user’s information | [33c59b3042acc6ffac59bb7e418f7f85]()
sg.com.singnet .mystorage.android | 100K - 500K | A3 | use Facebook cookie to reconnect when user logouts | [25611dc7d573e43c923f8e51f7835302]()
com.hlpth.molome | 10K - 50K | A2 | inject JavaScript to steal Google access token | [a3ec6a2e3e5f387a53cdb06a3e48c917]()
com.weirdlysocial.videoview | 10K - 50K | A2 | inject JavaScript to steal user’s Instagram credentials | [7ebccfbd85c8f239b122ea31eb0b318a]()
com.wierdlysocial.storyview | 5K - 10K | A2 | inject JavaScript to steal user’s Instagram credentials | [f4f1f6f644bbca4de637c0b19b94ec1f]()
com.deltecs.wipro | 50K - 100K | A3 | use teamgum’s clientId in Google SSO and steal access token from cookies | [45dfd761e11883c0b225f7dc8edb4b14]()
com.snapdealhub | 500K - 1M | A3 | use teamgum’s clientId in Google SSO and steal access token from cookies | [31139b30a4f92f14a8f9707f74c9b60d]()
com.ilgan. GoldenDiskAwards2016 | 100K - 500K | A1 | use fengchuanke’ clientId for Weibo SSO | [78c32007638f64de697dfb473a2a6d0d]()
com.homedev.locationhistory | 100K - 500K | A3 | steal Google cookies and save them into sharedpreference | [78ca09ff3d1367982c5fb084b8f31734]()
com.danielstudio.app.wowtu | 10K - 50K | A3 | steal Weibo cookies and abuse cookie to update photos | [aa3dd94becf64647fdf74e2b2aa7b325]()
com.aol.mobile.aim | 1M - 5M | A3 | steal Facebook cookies and save them into sharedpreference | [80931d076bd5be08e7e1077e31b409e2]()


#### If you want the 21 malicious cases for academic study, please contact me: xh_zhang [AT] fudan.edu.cn


