+++
title = "How do I make gnu screen look better?"
author = ["T", "Ivan"]
lastmod = 2020-04-21T13:56:55+09:00
weight = 2055
draft = false
+++

## How do I remove the white dividers between splits? {#how-do-i-remove-the-white-dividers-between-splits}

-   Q: I want to center my vim in the middle of the screen and have a
    big black border on each side(to look like iA writer). I think I
    can do this with gnu/screen. just make two vertical splits and
    have thin panes on either side of the vim pane. But the split
    divider is a bid white bar, hardly no distractions.
-   A: ctrl-a :rendition so "="
    or :rendition so =00(or 01)
    will remove the while block split divider.
-   ctrl-a :caption string "%{03}"
    might remove the horizontal split (never tried)
