+++
title = "How do I grep in a minified file?"
author = ["T", "Ivan"]
lastmod = 2020-04-10T17:47:12+09:00
weight = 2053
draft = false
+++

when a file has all its text on one big long line, grep is not very
useful. how can i just get the part of a line I want?


## Use regex to match character before and after, and -o to only show match. {#use-regex-to-match-character-before-and-after-and-o-to-only-show-match-dot}

grep -o "\\{0,15\\}search\_string\\{0,20\\}" file
