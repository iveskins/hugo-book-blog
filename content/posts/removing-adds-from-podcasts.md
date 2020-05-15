+++
title = "Removing adds from podcasts"
author = ["T", "Ivan"]
lastmod = 2020-05-15T17:35:37+09:00
weight = 2066
draft = false
+++

I am sick of the psyops of advertising. I want to detox. but I still
want to listen to podcasts. I need strip out the adds from them


## How can I programatically remove adds from podcasts {#how-can-i-programatically-remove-adds-from-podcasts}

-   most podcasts have an add role at the beginning, end or middle
-   the Beginning and end are easy enough to skip, it's built into
    my podcast player, to skip X seconds. I use this to avoid
    annoying jingles and "brought to you by" messages.
-   middle bits might have silence or a tune to signal their coming.
-   would want a way to identify the timestamps of the beginning and
    end of this, and then, skip it real time (hard without modifying
    a player app)
    -   or clip it out and re-save the podcast.
        -   if I save it it raises the question. Where to, and for how
            long
-   I am thinking I could make this a lambda function, feed by the
    rss of my podcasts, that resaves to an object storage provider,
    and makes a new rss feed, that I can subscrice to with my app.
-   First I have to research about how to detect middle bits.
    -   it could be that they are always at the same time in the more
        reliable podcats.
-   sometime there is info in the middle bit I want to hear too, so
    maybe .. ASR it to text, and add the text to the feed
    description. It is not so invasive to see the text.. then I can
    also regex out square space and blue apron and things.
