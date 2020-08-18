+++
title = "reduce gitlab memory for docker"
author = ["T", "Ivan"]
lastmod = 2020-08-07T12:01:08+09:00
weight = 2017
draft = false
+++

-   omnibus
    unicorn['worker\_processes'] = 3
    postgresql['shared\_buffers'] = "256MB"
    gitlab\_rails['db\_prepared\_statements'] = false
    sidekiq['concurrency'] = 15 #25 is the default
    prometheus\_monitoring['enable'] = false

    2.2 -> 1.7 G
