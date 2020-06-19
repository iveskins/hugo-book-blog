+++
title = "Generating text for utterances"
author = ["T", "Ivan"]
lastmod = 2020-06-18T13:59:30+09:00
weight = 2067
draft = true
+++

## 1 Make source text. {#1-make-source-text-dot}

Here is [a list of submitted sentences](https://kinto.mozvoice.org/v1/buckets/App/collections/Sentences_Meta_en/records) to the common voice
project sentnece collection tool. It includes sentences yet to be
validated.. but It is as good a start as any.

This json can be parsed down to lines of text by using json query
to select the sentence element, and sed to remove the quote
marks. We want to remove those so the model doesn't get confused
by them. It might be worth randomising the order of the lines too.

<a id="orgd04f54e"></a>
```bash
'''jq '.data[].sentence' <
mozilla.sentence.collector.20200527.records.json | sed -e 's/^"//'
-e 's/"$//' | head >
mozilla.sentence.collector.20200527.records.utts.txt
```

or maybe

<a id="orgfc48d80"></a>
```bash
gsed -e 's/\\\u2060//g' < mozilla.sentence.collector.20200527.records.json  | jq  '.data[] | select(.approved!=false).sentence' | gsed "s/[$SINGQ]/'/g; s/[$DUBQ]/\"/g" | iconv -f utf-8 -t ascii//translit |  sed -e 's/^"//' -e 's/"$//' | sed -e 's/\\\"/"/' > mozilla.sentence.collector.20200527.records.utts.clean.txt
```
