+++
title = "Writing Hugo blog in org"
author = ["T", "Ivan"]
date = 2017-09-10
lastmod = 2020-02-18T13:37:35+09:00
tags = ["hugo", "org"]
categories = ["emacs"]
weight = 2001
draft = true
foo = "bar"
baz = "zoo"
alpha = 1
beta = "two words"
gamma = 10
[menu.main]
  weight = 2001
  identifier = "writing-hugo-blog-in-org"
+++

## First heading within the post {#first-heading-within-the-post}

-   This post will be exported as  a s
    `content/posts/writing-hugo-blog-in-org-subtree-export.md`.
-   Its title will be "Writing Hugo blog in Org".
-   It will have _hugo_ and _org_ tags and _emacs_ as category.
-   The menu item _weight_ and post _weight_ are auto-calculated.
-   The menu item _identifier_ is auto-set.
-   The _lastmod_ property in the front-matter is set automatically to
    the time of export.


### A sub-heading under that heading {#a-sub-heading-under-that-heading}

-   It's draft state will be marked as `true` as the subtree has a the
    todo state set to _TODO_.

With the point <span class="underline">anywhere</span> in this _Writing Hugo blog in Org_ post
subtree, do `C-c C-e H H` to export just this post.

The exported Markdown has a little comment footer as set in the _Local
Variables_ section below.


### using hugo shortcodes {#using-hugo-shortcodes}

<https://github.com/kaushalmodi/ox-hugo/issues/242>
<https://gohugo.io/content-management/shortcodes/>

```nil
#+html: {{< gist iveskins 4b0c620f3e51968ff67453ac78f2fb59 >}}
```


### Using images {#using-images}

1.  put them in the ./static/images/ folder
2.  link them as /static/images/name surrounded by [[ s
