---
layout: post
title:  "Unit 1-3 Discussion Summary"
author: yusuf
categories: ssd
image: assets/images/1785.webp
published: True
date: 2022-03-23
---

Creating proper data management should be an important matter in software development. In the 2017 top ten list, Sensitive Data Exposure (SDE) were included. Although it’s not on the list anymore, sensitive data issues are still happening in my home country Indonesia no matter who owns the application – governments, even modern start-ups.

There are several ways to mitigate this issue, even OWASP detailed a list of actions to prevent SDE from happening. I also received feedback from my peers on my initial post that address this issue. To summarize, the best way to prevent this issue, it’s all about putting attention to the problems and strategising about them.

One of my classmates, Ian Wollof, said to use a technology called row-level security, which will restrict access to sensitive data while keeping the non-sensitive data accessible. My other classmate, Yin Ping, suggested developers should differ queries for different users. On the other hand, my argument is to model the database into different layers (e.g. secured, public) and set up the read or write access properly.

From this discussion, I can conclude that no matter what, putting attention to data is the most important step. About how the strategy is, we can be creative about it, as we all know also there’s no one solution for all. We have to adjust according to our current situation. And it might be different from one place to another.

There are tons of services we can use nowadays. Amazon Macie from AWS, Cloud Data Loss Prevention, or OLS from Oracle is several examples of those tools.

It’s also important to mention that during user testing, cases to test should not only be about making sure the end-user features are working properly, but also security measurements testing.
