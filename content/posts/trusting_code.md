+++
title = "How can I trust any code?"
author = ["T", "Ivan"]
lastmod = 2020-04-10T17:46:58+09:00
weight = 2024
draft = false
+++

[This](https://security.stackexchange.com/questions/222457/how-am-i-ever-going-to-be-able-to-vet-120-000-lines-of-composer-php-code-not) discussion on security.stackexchange talks about the use of
other people libraries in your code and what to do about the fact
that you didnt write it yorself.. and there is too mush code to
review it line by line.. how can you be sure of secuiriy

-   you can't, but you have to think about how sensitive your data /
    system is.
-   if you can't audit the code, you can audit the people releasing
    it, and their release methods, and their past action about
    security issues.. in short you can assess how trust worthy they
    might be
-   writing everythign yourself and reviewing it yourself isn't a way
    to manufacture security anyway.. because you can make
    mistakes.. isn't it better to use a popular library that lots of
    people use, and experts in the minutia of that field have
    written?
-   There is a [book](https://dl.acm.org/citation.cfm?id=358210) _Reflections on trusting trust_ - Ken Thompson
    (1984) that is some of the though on this issue from the early
    days of software
