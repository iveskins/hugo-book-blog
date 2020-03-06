+++
title = "How can run forked processes in bash"
author = ["T", "Ivan"]
lastmod = 2020-03-06T15:19:37+09:00
weight = 2031
draft = false
+++

## With gnue parallel {#with-gnue-parallel}

$ parallel -j 4 wget -q {} < list.txt

<https://www.cyberciti.biz/faq/how-to-run-command-or-code-in-parallel-in-bash-shell-under-linux-or-unix/>

like make all the voices of all languages speak at once bable style
parallel -j 40 say -v {} (diceware -n 4 -d ' ') < voices.txt
