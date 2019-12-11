+++
title = "reduce gitlab memory for docker"
author = ["T", "Ivan"]
lastmod = 2019-12-11T12:00:42+09:00
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
