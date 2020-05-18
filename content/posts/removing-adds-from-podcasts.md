+++
title = "Removing adds from podcasts"
author = ["T", "Ivan"]
lastmod = 2020-05-18T14:12:51+09:00
weight = 2066
draft = false
+++

I am sick of the psyops of advertising. I want to detox. but I still
want to listen to podcasts. I need strip out the adds from them


## How can I programatically remove adds from podcasts {#how-can-i-programatically-remove-adds-from-podcasts}

-   most podcasts have an add role at the beginning, end or middle
-   the Beginning and end are easy enough to skip, it's built into
    my podcast player, to skip X seconds. I use this to avoid
    annoying jingles and "brought to you by" messages.
-   middle bits might have silence or a tune to signal their coming.
-   would want a way to identify the timestamps of the beginning and
    end of this, and then, skip it real time (hard without modifying
    a player app)
    -   or clip it out and re-save the podcast.
        -   if I save it it raises the question. Where to, and for how
            long
-   I am thinking I could make this a lambda function, feed by the
    rss of my podcasts, that resaves to an object storage provider,
    and makes a new rss feed, that I can subscrice to with my app.
-   First I have to research about how to detect middle bits.
    -   it could be that they are always at the same time in the more
        reliable podcats.
-   sometime there is info in the middle bit I want to hear too, so
    maybe .. ASR it to text, and add the text to the feed
    description. It is not so invasive to see the text.. then I can
    also regex out square space and blue apron and things.


## Notes {#notes}

-   [Adblock Radio](https://www.adblockradio.com/blog/2018/11/15/designing-audio-ad-block-radio-podcast/)
-   <https://blog.rekawek.eu/2016/02/24/radio-adblock/>
-   <https://stackoverflow.com/questions/45526996/split-audio-files-using-silence-detection/46001755>
-   [Landmark project to identify audio](https://github.com/adblockradio/stream-audio-fingerprint)
-   [Landmark in python](https://github.com/worldveil/dejavu)


## dpwe/audfprint {#dpwe-audfprint}

[Dpwe's audfprint](https://github.com/dpwe/audfprint) Is a python command line tool for working with
audio landmarks. It seems to be a reimplementation of a matlab
project.


### Install {#install}

-   pip(3?) install -r requirements.txt
    -   make sure you have ffmpeg.. the OSX ffmpeg might give
        slightly different output (i.e time formatting) to the linux
        one. It doesn't seem to be a problem.


### Use. {#use-dot}

-   Get some podcasts. (in this use case the podcast play a little
    tune(motif) at the beginning and end of the ads. beginning tune and
    end tune differ)
-   Clip out the audio motifs that bookend the middle bit with
    adds. This can be done with audacity's export selection. Wav
    files seem to be fine (anything ffmpeg can open?).
    {{<figure src="/images/audacity_middle_bit_export.png">}}
    -   save these clips to named for the start and ends.
-   Make a landscape database for the start motif and the end
    motif.
    -   python audfprint.py new --dbase
        podcast\_middlebit\_in.pklz
        podcast\_clip\_in\_\*.wav
    -   python audfprint.py new --dbase
        podcast\_middlebit\_out.pklz
        podcast\_clip\_out\_\*.wav
    -   Use this DB to scan podcast to identify the position of the
        start and end of the middle bit.
        -   OSX will output in -1500.9s negative seconds format


#### <span class="todo TODO_">TODO </span> Use start and stop timestamps to clip out and re-compile podcast with no-middle bit. {#use-start-and-stop-timestamps-to-clip-out-and-re-compile-podcast-with-no-middle-bit-dot}


#### <span class="todo TODO_">TODO </span> Make this .. an automated system {#make-this-dot-dot-an-automated-system}

-   Make a DB of IN/OUT motifs for podcasts that you listen to
