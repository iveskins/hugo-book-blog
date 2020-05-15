+++
title = "How do i make Gnu/Screen multi-user"
author = ["T", "Ivan"]
lastmod = 2020-05-15T13:19:10+09:00
weight = 2060
draft = false
+++

## [Follow instructions here](https://www.mfitzp.com/article/collaborate-in-the-shell-with-screen-multiuser/) {#follow-instructions-here}

-   sudo chmod +s /usr/bin/screen  # Make screen suid root
-   sudo chmod 755 /var/run/screen # Make the screen dir more open
    "Note that if you want to share a screen between two sessions of
    the same user on a system you can skip this step entirely. This
    is useful for example if you have a shared login on a system."
-   screen -d -m -S multi

-   :multiuser on
-   :acladd <username>

    -You can save yourself some time by putting these commands in
    the .screenrc configuration file.
