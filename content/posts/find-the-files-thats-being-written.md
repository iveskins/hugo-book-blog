+++
title = "find the files thats being written"
author = ["T", "Ivan"]
lastmod = 2020-08-07T12:01:08+09:00
weight = 2019
draft = false
+++

## How do you find which file recursively is the most recent modified in a folder? {#how-do-you-find-which-file-recursively-is-the-most-recent-modified-in-a-folder}

\#BEGIN\_SRC bash
find $DIR -type f -printf "%T@ %p\n" | sort -n | cut -d' ' -f 2- | tail -n 1
\#END\_SRC
from [here](https://stackoverflow.com/questions/1015678/get-most-recent-file-in-a-directory-on-linux)
