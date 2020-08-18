+++
title = "Removing adds from podcasts"
author = ["T", "Ivan"]
lastmod = 2020-08-07T12:01:28+09:00
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

{{< highlight bash "linenos=table, linenostart=1">}}
bash-3.2$ python3 audfprint.py match --dbase taz_fpdbase.pklz ../audio/taz14_tc.mp3 --find-time-range -T -x 10
 -H 2
Mon May 18 16:42:36 2020 Reading hash table taz_fpdbase.pklz
Read fprints for 4 files ( 1262 hashes) from taz_fpdbase.pklz (0.00% dropped)
Mon May 18 16:43:49 2020 Analyzed  ../audio/taz14_tc.mp3 of 4756.956 s to 298377 h
ashes
Matched    1.3 s starting at 1932.3 s in ../audio/taz14_tc.mp3 to time   18.5 s in /Users/bwp002/Documents/taz
_13_mid_in_audfprint.wav with    10 of   216 common hashes at rank  2
Matched    2.7 s starting at 1931.8 s in ../audio/taz14_tc.mp3 to time    7.9 s in /Users/bwp002/Documents/taz
_mid_in_audfprint.wav with    25 of   314 common hashes at rank  0
Matched    1.5 s starting at 1932.8 s in ../audio/taz14_tc.mp3 to time    7.2 s in /Users/bwp002/Documents/taz
_13_mid_in_audfprint.wav with    16 of   216 common hashes at rank  2
Matched    1.7 s starting at 1932.3 s in ../audio/taz14_tc.mp3 to time    3.8 s in /Users/bwp002/Documents/taz
_mid_in_audfprint.wav with     8 of   314 common hashes at rank  0
Matched    0.8 s starting at 1934.3 s in ../audio/taz14_tc.mp3 to time    5.4 s in /Users/bwp002/Documents/taz
_mid_out_audfprint.wav with    13 of   197 common hashes at rank  1
Matched    4.0 s starting at 1932.3 s in ../audio/taz14_tc.mp3 to time    2.5 s in /Users/bwp002/Documents/taz
_mid_in_audfprint.wav with   109 of   314 common hashes at rank  0
Matched    2.5 s starting at 1932.8 s in ../audio/taz14_tc.mp3 to time    2.5 s in /Users/bwp002/Documents/taz
_mid_out_audfprint.wav with    61 of   197 common hashes at rank  1
Matched    1.5 s starting at 2075.1 s in ../audio/taz14_tc.mp3 to time   17.6 s in /Users/bwp002/Documents/taz
_13_mid_in_audfprint.wav with     7 of   216 common hashes at rank  2
Matched    2.9 s starting at 2075.1 s in ../audio/taz14_tc.mp3 to time    7.5 s in /Users/bwp002/Documents/taz
_mid_in_audfprint.wav with    24 of   314 common hashes at rank  0
Matched    1.2 s starting at 2076.5 s in ../audio/taz14_tc.mp3 to time    7.2 s in /Users/bwp002/Documents/t
az_13_mid_in_audfprint.wav with    10 of   216 common hashes at rank  2

{{< /highlight >}}


#### <span class="todo TODO_">TODO </span> Use start and stop timestamps to clip out and re-compile podcast with no-middle bit. {#use-start-and-stop-timestamps-to-clip-out-and-re-compile-podcast-with-no-middle-bit-dot}

[Ref](https://superuser.com/questions/681885/how-can-i-remove-multiple-segments-from-a-video-using-ffmpeg)

{{< highlight bash "linenos=table, linenostart=1">}}
bash-3.2$ ffmpeg -i audio/taz14_tc.mp3 -filter_complex "atrim=start=0:end=1932[s];[0:a]atrim=start=2075[e];[s]
[e]concat=v=0:a=1[af]" -map [af]  out.mp3
{{< /highlight >}}

which outputs this:

[Output mp3](/mp3/out_trimmed.mp3)

 But this is slow as it has to re-encode the file. If I try the
"-acodec copy" flag, it says it doesnt work with complex filters.


#### <span class="todo TODO_">TODO </span> Make this .. an automated system {#make-this-dot-dot-an-automated-system}

-   Make a DB of IN/OUT motifs for podcasts that you listen to
