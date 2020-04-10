+++
title = "How do I stop chrome going back when i two finger swipe on trackpad?"
author = ["T", "Ivan"]
lastmod = 2020-04-10T17:47:00+09:00
weight = 2028
draft = false
+++

## Problem {#problem}

I keep losing data in forms and the like, by accidentially
trigging the browser to go back with a two finger swipe. this iis
because three finger swipe is the way to change desktops, so its
easy to misregister a finger and get a back.


## solutions {#solutions}

-   Turn it off with a flag: Some places said to set a flag at
    "chrome://flags/#overscroll-history-navigation". but this doesn't
     seem to exist anymore.

-   Turn if off with osx defaults
    -   <https://support.google.com/chrome/thread/5616407?hl=en&msgid=24668853>
        For mac os x:defaults write com.google.Chrome AppleEnableSwipeNavigateWithScrolls -bool FALSE
