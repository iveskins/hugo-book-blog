+++
title = "How to build a Publii blog with Netlify"
author = ["T", "Ivan"]
lastmod = 2020-04-24T17:45:07+09:00
weight = 2009
draft = false
+++

[Pretty much this](https://getpublii.com/docs/build-a-static-website-with-netlify.html#js-header). If the css doesn't load, double check you used
https when putting in the netlify url into the publii server setting
page.

My impressions is that the number of themes are a bit limited. There
also seems to be a bit of learning curve as to how all the fields and
levers in the settings page relate to changes on the site. Like it
took me a few tries to get the landing page background image
changed. apparently that is called a "hero section".
I was also interested in the little work around of starting a new
netlify page by uploading a zip file with an empty index.html. Seems
like a bit of a design oversight or .. anti-patern.. to not just have
a create new site buton that is not linked to a git repo. It also
seems a bit of a security nono to have to make an access token that
has rites to my entire netlify account when I only want to manage one
page. And then is that token stored safely on my desktop? anyway there
is nothing stopping someone(on my desktop) clicking the show password
and getting an access token that can be used to change anything on my
netlify account...

I was also interested to see the import wordpress WXR file tool. I
wonder how that would work out.. Just take all the posts and pages
etc.. You would still have to do a lot of theme or css work I think.

Also I worry If I make this on my work computer I will get trapped
there. [This](https://getpublii.com/blog/managing-static-website-on-multiple-computers.html) talks about how to edit from multiple computers.
