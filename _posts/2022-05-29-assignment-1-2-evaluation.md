---
layout: post
title: "Evaluation of Assignment I & II"
author: yusuf
categories: nism
image: assets/images/6040.webp
published: True
date: 2022-05-29
---

Doing the second assignment, where we started to get our hands to do the security audit, we found that it’s not easy to evaluate the site security without having the proper access to the site. Although there are a lot of things that we can check without having authorization to the site, I found that a lot of dangerous vulnerability scanning couldn’t be done without us verifying that we own the site. 

For example, when trying to test for the Cross-Site Request Forgery (CSRF). There are lots of tools that offer to scan for CSRF vulnerabilities, but when we wanted to do the checking, the service will ask us to verify that we own the site by uploading some scripts to the server – similar to Google’s identity verification, otherwise, it won’t be possible without having advanced skillsets.

We were using OWASP Zap, fortunately, we were still checking whether the site is secure from CSRF through another checking method as an alternative. Instead of doing the testing by simulating a CSRF attack, it checked for an anti-CSRF token, whether they exist on the website or not. We found that it is vulnerable to CSRF attacks. A second example is to check whether our data is being kept safely according to the GDPR rules. There is no way to check them without having access to the backend database where sensitive data are stored.

This might explain why many companies are having their security team (insider) hunt for vulnerabilities in their digital products. With greater access, it’s easier to explore every corner and look for anything. Compared to limited access, it’ll take a long time to find vulnerabilities. Although, this doesn’t mean they are closing the door to the outsider to help them find vulnerabilities in their products. 

Many companies are having a bounty program, where the company will pay for the person who finds unknown vulnerabilities. I think this is beneficial for two reasons. The first reason is it makes the possibility of hackers turning into white hat hackers. Rather than being a cybercriminal, I will choose to join the bounty program. I’ll earn the bounty, and the company will have no business impact because I am not exploiting the vulnerabilities. It’s a win-win solution.

The second reason is, that it’s indirectly growing up the manpower a company has to deal with security matters. For the first reason, the bounty program makes it look like the outsider works for the company. Just like in code review, in finding vulnerabilities, the more people involved, the faster a vulnerability will be found. Everyone is having their own set of skills and structure of thinking. 
