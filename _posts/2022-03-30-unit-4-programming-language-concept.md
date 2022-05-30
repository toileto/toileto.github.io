---
layout: post
title:  "Programming Language Concepts"
author: yusuf
categories: ssd
image: assets/images/5051.webp
published: True
date: 2022-03-30
---

### What is ReDOS and what part does ‘Evil Regex’ play?

ReDOS is a security issue that exploits the way a system works when processing a regex input. Most regexes are are having an exponential complexity depending on their input (Contrast Security, 2020). Hackers are using this to either hang the system by sending a crafted regex as the input that leads to what is known as catastrophic backtracking. These inputs are what is known as evil regex.

### What are the common problems associated with the use of regex? How can these be mitigated?

The common problem (security issue) relating to RegEx is injection-type of security. Since the use of RegEx is common to validate user inputs, causing this area is vulnerable. Some attacks listed by OWASP on their website related to the use of RegEx are:
1. Overly Permissive Regular Expression,
2. SQL Injection,
3. And, ReDOS.

To mitigate this issue, there is a tool known as ACRE that can help us to check whether the regex we are forming is dangerous or not (Larson, n.d.). Several other ways can be implemented to mitigate regex issues, and the main point is to eliminate the use of regex. But it’s not as easy as it is, and it makes it more of a combination rather than a single solution. For example is by using multithreading and process monitoring and killing (Contrast Security, 2020). Fuzzy testing also can be used to detect problematic regexes (Custodio, 2021).

### How and why could regex be used as part of a security solution?

Yes, regex can be used as a security solution. With the right design, regex can help a system from various kinds of vulnerabilities such as user input validation to avoid SQL injection, creating an access blacklist, and many more (Li, 2020).

#### References

Contrast Security, 2020. Attacking Evil Regex: Understanding Regular Expression Denial of Service Attacks (ReDoS). [Online] 
Available at: https://sec.okta.com/articles/2020/04/attacking-evil-regex-understanding-regular-expression-denial-service
[Accessed 30 March 2022].

Custodio, E., 2021. Finding Issues In Regular Expression Logic Using Differential Fuzzing. [Online] 
Available at: https://defparam.medium.com/finding-issues-in-regular-expression-logic-using-differential-fuzzing-30d78d4cb1d5
[Accessed 30 March 2022].

Larson, E., n.d. Automatic Checking of Regular Expressions. 
Li, V., 2020. Dangerous Regular Expressions. [Online] 
Available at: https://sec.okta.com/articles/2020/07/dangerous-regular-expressions
[Accessed 30 March 2022].


