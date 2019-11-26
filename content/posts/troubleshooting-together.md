+++
title = "Troubleshooting together"
author = ["T", "Ivan"]
lastmod = 2019-11-26T17:24:03+09:00
weight = 2007
draft = false
+++

## Making Changes {#making-changes}

Aside from the general best practice of making changes in a
shared change controled environment (like not doing so without
prio planning and communication) When troublesshooting in an
environment that no-one is using for anything important currently,
it's important that you can put everything back how you found
it at the end. This helps prevent configuration drift, and breaking things
for the next guy.
When troubleshooting, you should keep a detailed and time ordered
list of the changes to configuration. So you always know what you
changed, and how to reverse it back when your done.
