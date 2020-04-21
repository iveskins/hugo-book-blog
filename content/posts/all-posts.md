+++
author = ["T", "Ivan"]
lastmod = 2020-04-21T13:56:10+09:00
draft = false
+++

## Ideas {#ideas}


### <span class="todo DONE_">DONE </span> About this site {#about-this-site}


#### Whats is this? {#whats-is-this}

This a blog. It is edited in emacs org. It is exported to MD by
[ox-hugo](https://ox-hugo.scripter.co/), and generated into a static site with Hudo, using the
book theme. I wanted a way to make my many and various notes in my
org journal more centralised, and more useful in the future.
I like the book theme because it has a TOC. I am a fan
of the Cornell note taking system. {{<figure src="/images/cornell.webp.png">}}
Cornell notes have a focus on revision and skim-ability. I wanted
a blog site where I had a TOC I could use like the left hand
"keyword" column of this note system. That is to say. cover the
content, and use the keywords or key questions to revise what was
written. I often find myself writing my org journal headlines in
question format. But the answer are forgotten soon after i have
solved that problem and moved on to the next. I think If I had a
output for these notes, it would encourage me to keep them
neater. If they are neat they can form a support for my
professional accumulation of knowledge, and the ability to do the
thing. As it stands, even though I have done many amazing things once, I'm
not sure I could do them again any easier or quicker.

All the content is kept in one file content-org/all-posts.org. It
is exported with `C-c C-e H A`. Which triggers ox-Hugo to make a
md file for each Headding in the file.
[how to link images](https://ox-hugo.scripter.co/doc/image-links/)

[This guy helped](https://mstempl.netlify.com/post/static-website-with-emacs-and-hugo/) me when I googled how to do this.

-   What now?

    -   [ ] Learn more about how to format things in org files so I can
        output a pretty well formated blog
    -   [ ] Get a better idead of how to controll the menues and things of
        the book theme
    -   Make this integrated with netlify so i can just push
        changes to github and have it update the site. [This helped](https://gohugo.io/hosting-and-deployment/hosting-on-netlify/#use-hugo-themes-with-netlify). It
        is now online at amazing-beaver-3ff5b0.netlify.com and soon
        become.radioac.dev
    -   [ ] Wait for tsl certificate to be issued.
    -   [ ] make the "edit this page" link at bottom of template go to the org file.
    -   [ ] add some more blog like features to the book blog pages
        -   [ ] tags and things
        -   [ ] next and previous etc
    -   [ ] get the export on save thing working

-   Features I want.

    -   [ ] Discovery
        -   [ ] Other things from this tag
        -   [ ] next and previous
        -   [ ] category
        -   [ ] Footnotes, or tool tips
        -   [ ] move TOC to the left
        -   [ ] Make a quiz mode.. like hide the content of the
            subheadings until clicked.
        -   [ ] have a summary footer for each post..
            -   [ ] be able to skim browse all the post by these sumaries

-   Alternatives

    -   Hosting

        -   <https://zeit.co/>


### <span class="todo DONE_">DONE </span> Epwing dictionaries {#epwing-dictionaries}


#### What is EPWING? {#what-is-epwing}

It seems to be a legacy format for dictionary data, that was
/ is mostly used by Japanese electronic dictionaries. I remember
someone complaining about its great inconsistency as a format, so
as to make importing data from it difficult. It seems that there
needs to be custom parsers written for each different publishers
version of the format. I came across it as a Japanese learner.
The browser dictionary extension [yomichan](https://foosoft.net/projects/yomichan/) can import some of these
to provide J:J&nbsp;[^fn:1] look
ups. The  J:J dictionaries I find most useful are the ones
targeted at people of my reading level (kids). These are not
available as EPWING.


#### Why do I care? {#why-do-i-care}

Because yomichan sometimes doesn't give you the defintion of
longer phrases, and I wanted to find a dictionary that might have
contained longer connected keywords, so I could make flashcards
directly of those, instead of their component parts.


#### Why this post? {#why-this-post}

to remember that there is a big collection of them [here](https://onedrive.live.com/?id=AC31052BF2B8CA11%211937&cid=AC31052BF2B8CA11).


### <span class="todo DONE_">DONE </span> Links {#links}


#### 2019 November {#2019-november}

-   21

    -   How do I get the DS\_store file out of my git repo?

        [Untrack-files-already-added-to-git-repository-based-on-gitignore](https://web.archive.org/web/20190521183336/http://www.codeblocq.com/2016/01/Untrack-files-already-added-to-git-repository-based-on-gitignore/)

    -   Where can I get example gitignore strings for osx?

        <https://github.com/github/gitignore>

    -   What is the a Finish gum I want to try.

        I was wondering if there was any endocrine disrupters in chewing
        gum. And that lead me to read some research papers about gum. The
        one i was reading was linking chewing flavorful gum to a reduction
        in saliva stress hormone indicators [fn::salivary cortisol level -

        -   <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5381771/> ] and in
            that it also mentioned that chewing speed has been shown to be a
            indicator of stress, so they had the participants chew at 70
            chews per minute to a metronone.. I wonder if you can look at
            people and make any assessment of their stress level by their
            chewing speed.. Anyway this article mentioned an unpalatable
            gum, Fazer Salmiakki. Which I of course wanted to know why
            anyone would make unpalatable gum. But it's just that salty
            licorice flavor.

        <https://candyhero.com/fazer-salmiakki-chewing-gum>

    -   How do I Add footnotes to org?[^fn:2]

-   28

    -   What is deschooling?

        [book and mp3 here](http://www.unwelcomeguests.net/Deschooling_Society) This is about an distributed,
        non-institutional approach to education. It's criticisms of
        schools are about how they condition people to chase the symbol
        of the thing not the real thing .. was my skim reading

    -   Some interesting discussion of the costs and responses to climate change from HN community

        <https://news.ycombinator.com/item?id=21648582>

    -   IOT edge tool

        <https://docs.edgexfoundry.org/Ch-Intro.html>
        A project to handle the movement of data from and between IOT
        devices and the cloud services they server

    -   Facebook has alternative text on images describing their features made by AI.

        I noticed today, that an image in my feed had text, one person
        and airplane. It's an accessibility thing. If only they let my
        just copy text from the mobile site.. sesh.. dont need AI to not
        do anti-patterns for free use
        [link](https://www.theverge.com/2016/4/5/11364914/facebook-automatic-alt-tags-blind-visually-impared)

    -   Blog / writing platform

        <https://read.write.as/> Write.as seems nice and simple.. not sure
        if I would pay for it..

    -   A source of information about CMS platforms and other tech reviews

        Not sure how much of this site is payola .. but its a good place
        to find a lot of CMS related service [CMSCRITIC.com](https://www.cmscritic.com)
        and <https://headlesscms.org/>

    -   WP > Publii

        <https://www.callmefred.com/i-switched-from-wordpress-to-a-static-website-using-publii/>
        <https://tidycustoms.net/introducing-publii-static-website-cms/>

    -   What can be done about bitrot

        <https://www.redhat.com/en/blog/what-bit-rot-and-how-can-i-detect-it-rhel>
        <https://scotch.io/bar-talk/how-i-migrated-from-wordpress-to-a-static-site>
        This was an easy to follow and practical discussion with
        commands and all, about using a layer between a block device and
        a FS to keep track of bitrot. I since found someone who
        automated this with raid1 set up..

    -   An interesting Japanese thinker maybe

        <https://en.wikipedia.org/wiki/Kojin_Karatani>
        because you need to get more involved with intelectual
        communities outside of english world

    -   Media theory in japan overview book

        <https://www.dukeupress.edu/media-theory-in-japan>

    -   Bio of a Canadian born Tokyo university prof talking about democracy etc

        <https://www.u-tokyo.ac.jp/en/whyutokyo/people020.html>

    -   Word press to static site generators

        <https://wp2static.com/>
        one possible plugin


### <span class="todo DONE_">DONE </span> I want to try a Kubernetes cluster on Pi {#i-want-to-try-a-kubernetes-cluster-on-pi}


#### Link {#link}

<https://itnext.io/building-a-kubernetes-cluster-on-raspberry-pi-and-low-end-equipment-part-1-a768359fbba3>
<https://github.com/lucasteligioridis/raspbernetes>
<https://itnext.io/headless-kubernetes-on-15-raspberry-pis-boot-in-under-8-minutes-808402ea2348>


### <span class="todo DONE_">DONE </span> How do I migrate a postgess database running in a docker container to one running on RDS? {#how-do-i-migrate-a-postgess-database-running-in-a-docker-container-to-one-running-on-rds}


#### How do I set up a PG DB on RDS. {#how-do-i-set-up-a-pg-db-on-rds-dot}

first what do I need? well in this case this is a POC[^fn:3] project, not a real build. So I don't need to think too
much about provisioning anything with sensible amounts of
resource. I will make the assumption that there is some resource
configuration that will match our apps needs, but I don't want to
figure that out for now. I want to just make some thing quick and
cheap. why not a t3.micro with none of the features enabled..
So I guess I need a PG instance of the same version as our docker
db.

-   Links

    -   <https://dev.to/jamby1100/deploy-rails-in-amazon-ecs-part-3-create-the-rds-database-task-definition-and-load-balancer-1ffe>


#### How do i migrate data from docker to RDS {#how-do-i-migrate-data-from-docker-to-rds}

Transition to AWS RDS:

-   Login to your machine.
    -   Stop the application docker- docker stop <application\_docker\_name>
    -   Check the website - should be down
-   Login to postgres container- docker exec -it <postgres\_docker\_name> bash
    -   Take a dump of your database:

        ```nil
        	pg_dump -Fc -v -h localhost -U <username> -d <db_name> -p
        	  5432 > dump_file.dump
        :q	 #+END_SRC
              - Copy the database to AWS RDS:While you’re in your postgres
        	container:
        	#+BEGIN_SRC
        	pg_restore -c -h <aws_rds_link> -U <username> -d <db_name> -v
        	dump_file.dump
        ```
-   Login to AWS RDS, validate the last entries in some tables.
-   Deploy the new code (with the new AWS RDS url)
-   Check your website - should be up and running
-   Validate some db updates
-   Stop the postgres container and remove it.
-   Most important step, first try it in your dev environment or staging before moving to productionAH

-   Links

    -   <https://medium.com/@aditya_misra5/move-your-local-postgres-db-container-to-rds-in-12-simple-steps-84f9fd450c9e>


#### What I did to get it working. {#what-i-did-to-get-it-working-dot}

-   Login to postgres container

    ```nil
    docker exec -it bw_db_1 bash
    ```
-   Take a dump of your database:

    ```nil
    root@b8fe08f89e89:/# pg_dump -Fc -v -h localhost -U postgres -p
    5432 > dump_file.dump
    ```
-   Copy the database to AWS RDS

    ```nil
    pg_restore -c -h <rds.endpoint> -U <master_user> -v dump_file.dump
    pg_restore -c -h bdw-multitenant-db-test.xxxxxxxxxxxxxxxxx.ap-northeast-1.rds.amazonaws.com
    -U postgres -v dump_file.dump
    ```
-   Put the DB details in the .env file, and in your docker-compose
    env vars if needed
-   A also rebuilt my images, but that was for an unrelated issue.
-   I got some "incompatible marshal file format (can't be read)"
    errors after doing this and recreating the docker container. Maybe
    the clients cookies are no longer valid or something. I could log
    in from another browser. so maybe some extra step is needed to
    clear out rails cache (rake cache:clear)?


#### What might the change path look like for production? {#what-might-the-change-path-look-like-for-production}

1.  Clone  production all up to speed with the current build on the
    docker container. and make sure it's okay.
2.  make an outage period where we take a dump of the docker-db and load
    it to RDS-db
3.  update production to use RDS endpoints for db. start it up and
    test it out.
    -   point it back at the docker instance if its not working.
4.  Bonus points ..
    -   clone prod to a staging environment .. and do it
        once there first
    -   How can you make sure users dont lose data if they input it
        into the new system and something goes wrong?


### <span class="todo DONE_">DONE </span> How do I troubleshoot RDS connectivity? {#how-do-i-troubleshoot-rds-connectivity}


#### How do I check access to RDS from my EC2 instance. {#how-do-i-check-access-to-rds-from-my-ec2-instance-dot}

The endpoint address and port of an RDS database can be found from
the RDS console on the "Connectivity & security" page.
To test Connectivity from a host to the DB here are some steps to
follow:

1.  confirm the endpoint dns resolves to the IP of the DB
    -   \`nslookup <endpoint>\`
2.  confirm network connectivity from host to the DB
    -   nc <endpoint> <port>
3.  Try to connect with a database client.
    -   psql -h <endpoint>


#### Well that didn't work. What should I check? {#well-that-didn-t-work-dot-what-should-i-check}

1.  Is there something else I should be doing?
2.  Is everything turned on?
    -   For example is the RDS instance in a running state or stopped?
3.  Are there typos anywhere?
4.  Am I using the right tool for the job?
5.  Is everything configured like you thought?
    -   IS the RDS instance in the subnet group you expected?
    -   Do you know how things are configured?
6.  is the configuration correct generally speaking?
    -   Do the subnet ACLS and SG allow for traffic between the the Let's check. I'm sure its an ACL or SG problem.
    -   Are RDS Subnet groups correct?

also [here is the aws support docs](https://aws.amazon.com/premiumsupport/knowledge-center/rds-cannot-connect/). It adds

-   Check DNS resolution with nslook up. \`nslookup rds.endpoint\`
    (usually I would ping the resolved IP to check network
    connectivity. .but I have a feeling RDS hosts have ping responders
    turned off.)
-   Then check with telnet or nc
-   As for troubleshooting the network the docs say
    -   check your VPC SGs allow access from client.
    -   (probably also need to check the clients SG and ACLs allow access
        out as well)
    -

-   Extra Commands

    -   install postgress on AmznLinux: \`sudo amazon-linux-extras install postgresql10\`

-   Links

    -   [Digital ocean blog](https://www.digitalocean.com/community/tutorials/how-to-use-netcat-to-establish-and-test-tcp-and-udp-connections-on-a-vps)


#### Whats is an RDS subnet group? {#whats-is-an-rds-subnet-group}

I made an RDS database, and then had problems connecting to it. It
turns out it had provisioned with an IP from another old projects
subnet, and that subnet's ACL didn't allow access. Why did my DB use
an interface in this seemingly random subnet? Maybe it was because of
the [RDS Subnet group](https://docs.rightscale.com/cm/dashboard/clouds/aws/rds_subnet_groups.html) configuration for this VPC. I had never heared of
this before so lets take a look.

> An RDS Subnet Group is a collection of subnets that you can use to designate for your RDS database instance in a VPC. The database within your VPC will use the Subnet Group and the preferred Availability Zone to select a subnet and an IP address within that subnet. An Elastic Network Interface will be associated to the database instance with that IP address. Note that each DB Subnet Group should have at least one subnet for every Availability Zone in a given Region.

[^fn:4]


#### Conclusion {#conclusion}

When I provisioned our general systems VPC and subnets, I did not
account for the need of a second subnet in another AZ, for the use
of RDS. I need to go back to the team and talk about make a new
subnet.


### <span class="todo DONE_">DONE </span> Troubleshooting together {#troubleshooting-together}


#### Making Changes {#making-changes}

Aside from the general best practice of making changes in a
shared change controled environment (like not doing so without
prior planning and communication) When trouble shooting in an
environment that no-one is using for anything important currently,
it's still important to put everything back how you found it when
you're finished. This helps prevent configuration drift, and
breaking things for the next person.
When troubleshooting, you should keep a detailed and time ordered
list of the things you have done. Especially changes to
configuration, so you know how to reverse these chaneges after.


### <span class="todo DONE_">DONE </span> Usefull Tools {#usefull-tools}


#### Thursday, 11/28/19 {#thursday-11-28-19}

-   [A swiss army knife tool for data transformation and analysis for
    Web apps](https://gchq.github.io/CyberChef/)
    Could be useful when developing web apps, or troubleshooting
    issues with apps. I found it in relation to someone describing
    traffic to their host that was BASE64 encoded twice. You can
    chain transformation together. It also seems to have quite a few
    image forensic tools.


### <span class="todo DONE_">DONE </span> How to build a Publii blog with Netlify {#how-to-build-a-publii-blog-with-netlify}

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


### <span class="todo DONE_">DONE </span> links 2019 11 29 {#links-2019-11-29}


#### How do you make file-specific setting changes in Vim? {#how-do-you-make-file-specific-setting-changes-in-vim}

using [Modeline](https://www.howtoforge.com/tutorial/vim-modeline-settings/). like to [force a file type](https://stackoverflow.com/questions/3853028/how-to-force-vim-to-syntax-highlight-a-file-as-html) and if it don't work
look [here](https://superuser.com/questions/323712/modeline-not-work-in-vim) and [here](https://emacs.stackexchange.com/questions/36525/is-there-an-emacs-equivalent-of-vims-modeline-magic).


#### What are parasocial relationships? {#what-are-parasocial-relationships}

This a term often used in examination of marketing and star
power. Like [how digital celeberties influence people to buy
things](https://www.sciencedirect.com/science/article/pii/S0747563218302553). And whats is [wron with youtube culture](https://digg.com/2018/parasocial-relationships-shannon-strucci-interview).


### <span class="todo DONE_">DONE </span> What was that chinese open source project to make RSS feeds from websites? {#what-was-that-chinese-open-source-project-to-make-rss-feeds-from-websites}

it was [RSShub](https://docs.rsshub.app/en/)


### <span class="todo DONE_">DONE </span> Terminal Tools {#terminal-tools}

As the workstation I station my work at slowly evolves, I grow
forgetful of all the little things I have done to make it comfortable
and efficient.


#### Command Line tools {#command-line-tools}

-   [Lnav](http://lnav.org/)

    Is a log file viewer with some great features for search, syntax
    highlighting, and in / out filtering, that makes it realy quick
    to understand the information in a log file. What is good about
    it, is that it is powerful like having a log agergation platform,
    but it is just a lightweight command line application.
    {{<figure src="/images/screenshot.lnav.png">}}

-   Htop

    is better than top
    {{<figure src="/images/screenshot.htop.png">}}

-   [Ranger](https://ranger.github.io/)

    Is a "A VIM-inspired filemanager for the console". It can be used
    for very quick navigation of files. it also integrates with
    iterm, and other terminal apps to allow for preview of images.
    {{<figure src="/images/screenshot.ranger.png">}}

-   NVIM

    -   plugins

        -   Nerdtree

    -   Keybindings

    -   Config

-   Emacs

    -   Aquamacs

-   Termshark

    [Termshark](https://github.com/gcla/termshark) is a A terminal UI for tshark, inspired by Wireshark
    [About it](https://www.linuxuprising.com/2019/04/analyze-network-traffic-with-termshark.html). It seems the doccuments are a bit sparse. If there is
    anythign that is unclear, it is probably something that can be
    looked up in the wireshark docs.. like what scale a suration
    number is in etc. these are just concepts taken directly from wireshark.
    {{<figure src="/images/screenshot.termshark.png">}}


#### Docker apps {#docker-apps}

-   Prouctivity

    -   Icescrum

-   DNS

    -   pihole

    -   Cloudflare

-   Webdav

    -   for zotero sync


#### Publishing {#publishing}

-   Blog

    -   Hugo

        -   -> emacs

    -   Publi


#### Colour schemes {#colour-schemes}


#### Chat {#chat}

-   nheko
-   riot


#### Fonts {#fonts}

-   [Nerd Fonts](https://NerdFonts.com) is a project that makes lots of differnt font icon

projects avaliable in one font. It also has a font patcher so you
can put icons into any font. Patched fonts can be installed by
homebew.
One font I found nice to use was [Fantasque](https://github.com/ryanoasis/nerd-fonts/tree/master/patched-fonts/FantasqueSansMono#installation). it Is in the spirit of
comic sans. [discussion of comic fonts](https://news.ycombinator.com/item?id=20533923)

-   I use monaco for my orgmode font in aquamacs
-   I use firacode for my iterm at the moment
-   my atom font is Menlo, Consolas, DejaVu Sans Mono, monospace
-   I also use Cascadia Code, and Caskaydia Cove Nerdfont on
    iterm. for the ligatures


#### Editors {#editors}

-   see nvim and emacs

-   Atom

-   Sublime text

-   textmate


#### Utility software {#utility-software}

-   Spectical

    -   making osx more like a tiling windows manager .. use hotkeys to
        shove windows around the screen into layouts

-   Clippy

    -   clipboard history

-   BalenaEtcher

    -   write images to sd cards (for RPI etc)

-   Keka

    -   (un)compress files


#### Browser {#browser}

-   Chrome

    -   Plugins

-   Firefox

    -   Plugins


#### Language {#language}

-   Custom dictionaries

    -   Types

        -   Emoji

    -   MacOS

    -   Google japanese Input

        All my current dictionaries can be found it [this git repo](https://github.com/iveskins/google.input.dic)
        I can't remember how I made them. but I am sure I just formatted
        other peoples files in a way that can be inported to google
        input.
        e.g:

        -   JAP-ENG

            There is a dictionary for displaying the English meaning of
            words typed in Japanse. useful
            {{<figure src="/images/ja-eng-words.png">}}
            and a dictionary for translating words typed in Japanse to
            English. not too useful for me.
            {{<figure src="/images/ja-ja-eng.png">}}

        -   Emoji dictionary

            [here](https://gist.github.com/iveskins/4b0c620f3e51968ff67453ac78f2fb59) is a gist of the dictionary file.
            Like this: {{<figure src="/images/emoji.input.png">}}
            {{<figure src="/images/emoji.@.emoji.png">}}
            {{<figure src="/images/emoji.icons.input.png">}}

    -   Where to get what

        -   EPWING

        -   JSON

-   Japanese word lookup

    -   Browser

        -   Mouse Dictionary

        -   Yomichan

    -   Whole OS

        -   Mac Linguist

-   Studya

    -   Flashcards

        -   Anki

            -   Deck types

            -   Input

    -   Media

        -   Subtitle Video Viewer

        -   Reading app

-   Keyboards

    -   Macbook

        -   Remapping keys

        -   Typing things like づ


#### Research {#research}

-   Zoreto


### <span class="todo DONE_">DONE </span> What is a language for creating interactive stories? {#what-is-a-language-for-creating-interactive-stories}

Its [ink](https://github.com/inkle/ink/blob/master/Documentation/WritingWithInk.md).

I can imagine using this to make an interacive story to run on a ebook
reader navigating through black and white images.
or [pubcoder](https://www.pubcoder.com/Features/Interactivity) or [apple ibook?](https://www.apple.com/ibooks-author/) or [kotobee](https://www.kotobee.com/blog/how-create-interactive-ebook-guide/)
or [Twine](https://twinery.org/) which is from the [Interactive Fiction Technology Foundation.](https://iftechfoundation.org/)
.. and used to make this cool interactive browser experience
[burnt matches](https://pippinbarr.com/games/burntmatches/). [morehere](https://www.pippinbarr.com/2016/11/29/burnt-matches/)

or to use with children in a coding skills and language development
situation. because it's so language bassed.. and then makes
interacctive content which encourages revision.. and the writing part
is like accuracy focused output .. and making a game is like
.. naturally you adapt from something else .. so there is pleanty of
chance to look at example text and adopt practical genre bassed
language patterns from it .. and re-write in your own way.. and there
is also the integration with art.. making assets for this game .. and
the coding language is very shallow learning curve but goes into
introducing some of the concepts of logical code thinking in a very
understandable ways..


### <span class="todo DONE_">DONE </span> News and research sources 2019/12/05 {#news-and-research-sources-2019-12-05}


#### Journals and information organisations {#journals-and-information-organisations}

-   [Asia-pacific journal](https://apjjf.org/2019/19/Temocin.html) with a japan focus. [here](https://apjjf.org/admin) has a list of
    articles and books.
-   [peach philosophy centre](http://peacephilosophy.blogspot.com/p/about-peace-philosophy-centre.html). Links to journals atleast..
-   [Advocacy for antiracism](https://antiracism-info.com/) group


#### Studies about automatic detection of hate speech. {#studies-about-automatic-detection-of-hate-speech-dot}

-   [Hate speech detection: Challenges and solutions](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0221152)
-

-


#### SPEECH Computing {#speech-computing}

-   [Creating an open speech recognition dataset for (almost) any
    language](https://medium.com/@klintcho/creating-an-open-speech-recognition-dataset-for-almost-any-language-c532fb2bc0cf). This is a very detailed instructions on using audio
    books to make speech traning data
-


#### Headless CMS {#headless-cms}

-   [Sheetsu](https://sheetsu.com/) with a japanese spelling form some reason.. uses google
    sheets as the source of data to make pages and tables and things
    .. could be useful for a toastmasters type situation where there
    is a static page to be made every month for the agenda
    etc.. that just needs data changed .. and has a lot of not tech
    fluent users - I found it here in this blog post about [headless cms](https://bejamas.io/blog/headless-cms/)


#### Non-centralised social web {#non-centralised-social-web}

I found out about the [Indiweb wiki](https://indieweb.org/) which says it is "The IndieWeb
is a people-focused alternative to the "corporate web".". There I
read about [pingbacks](https://indieweb.org/pingback) and [webmentions](https://indieweb.org/webmention.io). Which seems to be a way of
linking together websites or blogs that make mentions of each
other in their writings. so I dont need twitter or facebook as a
gobetween. I found out about it from
[This blog](https://paul.kinlan.me/using-web-mentions-in-a-static-sitehugo-/) by Paul Kinlan talking about how to implement it in a
hugo site.. which seems to involve some code for including the
things on the page,.. and then some extra code in your static site
build stage to go and find or send out mentions. I think Paul
Kinlan is a chrome developer, and I found him reading about
progressive web apps as an way for web developers to appeal to
users who are being entraped by app walled gardens of in app
browsers and no external links etc.


#### IT stuff {#it-stuff}

[The ombulabs](https://www.ombulabs.com/blog) blog has many intersting looking articles about how
to work well in it, and test code, upgrade rails, etc. very
sharing way of working .. if you can do something .. why not do it
well, document and share it and sell it as a consultancy service
.. that the kind of transparent working style that seems very
sustainable for everyone involved

-   [Koji](https://withkoji.com/docs/tutorials/creating-your-first-custom-vcc) is s code remixing platform trying to be the youtube of
    code.. they are paying for simple games to seed their library.


#### Interactive text {#interactive-text}

-   [Twine is an open-source tool for telling interactive, nonlinear
    stories.](https://twinery.org/) which looks pretty flexible .. it was used to make the
    game [Burnt matches](http://www.pippinbarr.com/2016/11/29/burnt-matches/) by the media researcher Pippin Barr.
    Which was a mix of text and interface and browser animation
    [speculative play](http://www.speculativeplay.com/about/) also looks interesting.
    Which I read about when reading about how to make an interactive
    epub [here](https://www.kotobee.com/blog/how-create-interactive-ebook-guide/) . I was thinking of how I could use my ereader in a
    more interesting way to navigate around some black and white
    photos.. or maybe use them to make an ereader point and click
    adventure game.. so I was readign about publishing tools for
    interactive epubs .. because Im not sure how advance the browser
    is on a kobo.. for handling normal html.. that page has a list
    of publishing tools that can out put as interactive epub. mostly
    as self promotion of itself Kotobee Author.
    if kobo can handle html5.. it might be worth looking into html
    game [engines](http://html5gameengine.com/)

-   Ink [ink](https://github.com/inkle/ink/blob/master/Documentation/WritingWithInk.md) also seems to be a very full featured game writing
    language like twine .. for pathed stories

-   [a list here](https://vagrantcursor.wordpress.com/2018/01/02/tools-to-make-narrative-games/) of tools to make interactive text


#### List of games researches {#list-of-games-researches}

[here](http://www.kmjn.org/game-rankings/) . including my old lecturer .. found this by cross searching
his name and the developer of burnt matches.


### <span class="todo DONE_">DONE </span> whats the story with Yahoo groups? {#whats-the-story-with-yahoo-groups}

yahoo sent short notice that they were deleting all their groups
data, and didn't make good tools for downloading it beforehand.
it will all be deleted on december 14th.


#### What are the tools to help the archivers get it? {#what-are-the-tools-to-help-the-archivers-get-it}

there is a tool to answer captures to join public groups, and then
give that account to the archvie team.
[download](https://github.com/davidferguson/yahoogroups-joiner/archive/master.zip) it here.


#### how can I archive myself? {#how-can-i-archive-myself}

[This python script](https://github.com/IgnoredAmbience/yahoo-group-archiver) can archive groups. I guess you need to join
them for it to work well.. I spun up an ec2 instance to try and
save a few groups from communities I would have been interested in
back in the 2000s.


#### Where can I read more? {#where-can-i-read-more}

[hacker news](https://news.ycombinator.com/item?id=21737696), [the group leading the archive effort](https://modsandmembersblog.wordpress.com/2019/12/08/verizon-yahoo-bad-form/)


### <span class="todo DONE_">DONE </span> critical Interface projects {#critical-interface-projects}


#### Whats that idea you had about a poem from source code? {#whats-that-idea-you-had-about-a-poem-from-source-code}

   you read on [hackernews](https://news.ycombinator.com/item?id=19672436) that the source-code for ZORK1 had been
   uploaded to [gitlab](https://github.com/historicalsource?tab=repositories), and there was discussion of an unpublished
   hitchhikers guide sequel. Someone linked to the [Zaphod source](https://github.com/historicalsource/restaurant/blob/master/people.zil#L265-L268).
   this had a bit like
   #BEGIN\_SRC
   <CONSTANT LDESC-STRINGS
<PLTABLE	"dancing"
	       "sipping sherry"
       ;3	"watching you" ;"talking quietly"
	       "looking at you with suspicion"
	       0 ;"gazing out the window"
       ;6	"walking along"
	       "sobbing quietly"
	       "poised to attack"
       ;9	"waiting patiently"
	       "eating with relish"
	       "preparing dinner"
       ;12	"listening to you"
	       "lounging and chatting"
	       "asleep"
       ;15	0 ;"reading a note"
	       "listening"
	       "preparing to leave"
       ;18	"deep in thought"
	       "out cold"
	       "ignoring you"
       ;21	"searching"
	       "playing the piano"
	       "following you"
       ;24	"brushing her hair"
	       "looking sleepy">>
   #END\_SRC

which was kind of poetic. atleast in layout.. and It made you think
this was a vein that could be mined for artistic expression.


### <span class="todo DONE_">DONE </span> reduce gitlab memory for docker {#reduce-gitlab-memory-for-docker}

-   omnibus
    unicorn['worker\_processes'] = 3
    postgresql['shared\_buffers'] = "256MB"
    gitlab\_rails['db\_prepared\_statements'] = false
    sidekiq['concurrency'] = 15 #25 is the default
    prometheus\_monitoring['enable'] = false

    2.2 -> 1.7 G


### <span class="todo DONE_">DONE </span> Ai writing {#ai-writing}


#### What was that site to plat with the GPT-2 text generation? {#what-was-that-site-to-plat-with-the-gpt-2-text-generation}

[here](https://www.theverge.com/tldr/2019/5/13/18617449/ai-text-generator-openai-gpt-2-small-model-talktotransformer) is the blog that talks about it [here](https://talktotransformer.com/) is the site. There is
alot of capchas


### <span class="todo DONE_">DONE </span> find the files thats being written {#find-the-files-thats-being-written}


#### How do you find which file recursively is the most recent modified in a folder? {#how-do-you-find-which-file-recursively-is-the-most-recent-modified-in-a-folder}

\#BEGIN\_SRC bash
find $DIR -type f -printf "%T@ %p\n" | sort -n | cut -d' ' -f 2- | tail -n 1
\#END\_SRC
from [here](https://stackoverflow.com/questions/1015678/get-most-recent-file-in-a-directory-on-linux)


### <span class="todo DONE_">DONE </span> What was that old guy taling about emacs? {#what-was-that-old-guy-taling-about-emacs}

[Bob newell](http://www.bobnewell.net/publish/35years/index.html) has some good writing about the simple joys of emacs.


### <span class="todo DONE_">DONE </span> CLI flashcards {#cli-flashcards}

 Someone asked on reddit linuxquestions about a commandline tool for
 doing flashcard revision like quizlet. I had a look into it thinking
 Immediatly of ANKI and emacs org mode. There is a tool to
 [edit anki cards in emacs](https://github.com/louietan/anki-editor). There is a [Drill](https://orgmode.org/worg/org-contrib/org-drill.html) minor mode for org that
 lets you do flashcards and srs.
 #BEGIN\_QUOTE
Org-Drill is an extension for Org mode. Org-Drill uses a spaced
 repetition algorithm to conduct interactive "drill sessions", using
 org files as sources of facts to be memorised. Each topic is treated
 as a "flash card". The material to be remembered is presented to the
 student in random order. The student rates his or her recall of each
 item, and this information is used to schedule the item for later
 revision.
\#END\_QUOTE
There is also [Pamparam](https://github.com/abo-abo/pamparam) "a new spaced repetition (SR) memory cards
 implementation for Emacs." which is under development recently.


### <span class="todo DONE_">DONE </span> What was that young musician you heard? {#what-was-that-young-musician-you-heard}


#### On wfmu? {#on-wfmu}

[Juniper](http://michaelshelley.net/juniper/) sining cheesy xmas songs and that "BOYS! BOYS! BOYS!
BOYS! BOYS!" song which could come in handy if anyone ever askes
my to teach english singing to young persons again.


### <span class="todo DONE_">DONE </span> Reading {#reading}


#### Read about political speech and heckling {#read-about-political-speech-and-heckling}

From [Jeremy Waldron](https://its.law.nyu.edu/facultyprofiles/index.cfm?fuseaction=profile.publications&personid=26993) which i read about here in the context of what
makes [a good campus speech](https://www.guernicamag.com/anatomy-of-a-successful-campus-talk/)


#### Product market fit {#product-market-fit}

<https://a16z.com/2017/02/18/12-things-about-product-market-fit/> via
<https://a16z.com/2019/12/09/product-zeitgeist-fit/>


### <span class="todo DONE_">DONE </span> How can I trust any code? {#how-can-i-trust-any-code}

[This](https://security.stackexchange.com/questions/222457/how-am-i-ever-going-to-be-able-to-vet-120-000-lines-of-composer-php-code-not) discussion on security.stackexchange talks about the use of
other people libraries in your code and what to do about the fact
that you didnt write it yorself.. and there is too mush code to
review it line by line.. how can you be sure of secuiriy

-   you can't, but you have to think about how sensitive your data /
    system is.
-   if you can't audit the code, you can audit the people releasing
    it, and their release methods, and their past action about
    security issues.. in short you can assess how trust worthy they
    might be
-   writing everythign yourself and reviewing it yourself isn't a way
    to manufacture security anyway.. because you can make
    mistakes.. isn't it better to use a popular library that lots of
    people use, and experts in the minutia of that field have
    written?
-   There is a [book](https://dl.acm.org/citation.cfm?id=358210) _Reflections on trusting trust_ - Ken Thompson
    (1984) that is some of the though on this issue from the early
    days of software


### <span class="todo DONE_">DONE </span> Can I stop an RDS instance for more than 7 days? {#can-i-stop-an-rds-instance-for-more-than-7-days}


#### Google {#google}

-   <https://cloudiknow.com/rds-stopped-for-more-than-7-days/>
-   <https://github.com/awslabs/aws-instance-scheduler/issues/42>


#### Looks like. {#looks-like-dot}

-   can use Cloudwatch scheduled tasks
-   Can use maintenance windows of rds to start and stop and reset
    7day timer?


#### Maybe it's better to delete it if its not being used.. {#maybe-it-s-better-to-delete-it-if-its-not-being-used-dot-dot}

and take a snapshot.
that seems to be the design on the system
if we cant do that then we need to increase our capabilities and
knowlege.

-   how to restore
    -   <https://www.youtube.com/watch?v=fxNmMQvOjbA>
-   What is the cost of keeping a snapshot around?
-   What will this mean in a COC defined environemnt
    -   the deletion should problaly be made by a code chagne..
        becuase even if you put back a new db with all the same
        setting
        the ids of the db will have changed, and terraform wouldnt
        recognise the database as the one it made


#### Make it {#make-it}

-

      default     = "cron(0 9 ? \* MON-FRI \*)"
    } # stop every weekday at 18:00JST+9

    variable "start\_schedule\_expression" {
      description = "Schedule for lambda execution"
      default     = "cron(50 23 ? \* SUN-THU \*)"
    } # start every weekday at 08:50JST+9


### <span class="todo DONE_">DONE </span> Done Are good-faith communities possible on the internet anymore? {#done-are-good-faith-communities-possible-on-the-internet-anymore}


#### Factors {#factors}

-   Organised bad-faith actors
    -   State backed troll farms
    -   ideological group backed organised actors
-   Increased diversity of internet users
    -   backgrounds
    -   social norms
    -   language
    -   knowledge
-   Generational changes in social interaction norms
    -   technological mediation, and there7s an multi-national
        corporated developed app for that, leaning
        to less developed social skills, and alientation,
        disconnection from own location, reigon. cant imagine actually
        calling a local business on the phone, and talking to a
        person..
-   Network effects??
    -   like chain recations.. The bad faith actors creating
        situations were other groups create anti-community action even
        though the do not share the same goals a the bad-faith group.
-   Infulence of hegemonic battles in wider society
    -   increased polerisation, antagonism, politicalisation of
        everyday life
    -   identiry politics
-   Unequal
    -   access to privacy and anonmyity
    -   knowledge and skills in the used of tech
    -   knowleged and skill in the use of new media
    -   levels of organisation and focus
        -   one side thinks this is a culture war
        -   the other side isnt aware there is a war going on
    -   levels of radicalized resoorting to violence


### <span class="todo DONE_">DONE </span> Voices {#voices}


#### What was that radio presenter with the archtypical radio voice? {#what-was-that-radio-presenter-with-the-archtypical-radio-voice}

-   RIP harry HARRY HARRISON.
-   On CBS fm.
-   <https://www.youtube.com/watch?v=jQ7r2P2cHDU>


### <span class="todo DONE_">DONE </span> Rpg systems where the player plays as a merchant or shopkeeper {#rpg-systems-where-the-player-plays-as-a-merchant-or-shopkeeper}

   :PROPE
RTIES:
   :EXPORT\_FILE\_NAME: rpg-systems-where-the-player-plays-as-a-merchant-or-shopkeeper


#### Google {#google}

-   <https://forum.rpg.net/index.php?threads/merchant-rpg.441068/>
-   <https://boardgamegeek.com/thread/1000184/fantasy-innkeeper>
-   less


### <span class="todo DONE_">DONE </span> How do I stop chrome going back when i two finger swipe on trackpad? {#how-do-i-stop-chrome-going-back-when-i-two-finger-swipe-on-trackpad}


#### Problem {#problem}

I keep losing data in forms and the like, by accidentially
trigging the browser to go back with a two finger swipe. this iis
because three finger swipe is the way to change desktops, so its
easy to misregister a finger and get a back.


#### solutions {#solutions}

-   Turn it off with a flag: Some places said to set a flag at
    "chrome://flags/#overscroll-history-navigation". but this doesn't
     seem to exist anymore.

-   Turn if off with osx defaults
    -   <https://support.google.com/chrome/thread/5616407?hl=en&msgid=24668853>
        For mac os x:defaults write com.google.Chrome AppleEnableSwipeNavigateWithScrolls -bool FALSE


### <span class="todo DONE_">DONE </span> Where is the cloudwatch logs query syntax actually doccumented? {#where-is-the-cloudwatch-logs-query-syntax-actually-doccumented}

its [here](https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/CWL_QuerySyntax.html). It is just hard to find. also 'like' should be followed by
regex in /'s


### <span class="todo DONE_">DONE </span> Links 2020 02 07 {#links-2020-02-07}


#### word regex {#word-regex}

<https://stackoverflow.com/questions/27349556/is-it-possible-to-check-if-a-word-is-really-an-english-word-via-regex>
if re.match(r'^([^aeiouy]{1,3}[aeiouy]{1,3}[^aeiouy]{1,3}|[aeiouy]{1,3}[^aeiouy]{1,3})+
    print "gobbledy gook!!!"


#### Cool speaker {#cool-speaker}

    Flat speaker from that movie theater. makes soft sound good for
ambience and detail
<http://taguchi-onken.com/product.html>


#### cloud training (expensive.. better than linkedin now maybe) {#cloud-training--expensive-dot-dot-better-than-linkedin-now-maybe}

<https://acloud.guru/gcp-cloud-training>


### <span class="todo DONE_">DONE </span> How can run forked processes in bash {#how-can-run-forked-processes-in-bash}


#### With gnue parallel {#with-gnue-parallel}

$ parallel -j 4 wget -q {} < list.txt

<https://www.cyberciti.biz/faq/how-to-run-command-or-code-in-parallel-in-bash-shell-under-linux-or-unix/>

like make all the voices of all languages speak at once bable style
parallel -j 40 say -v {} (diceware -n 4 -d ' ') < voices.txt


### <span class="todo DONE_">DONE </span> What was that document by the DOD on Agile {#what-was-that-document-by-the-dod-on-agile}


#### It was this {#it-was-this}

<https://web.archive.org/web/20200204200102/https://media.defense.gov/2018/Oct/09/2002049591/-1/-1/0/DIB_DETECTING_AGILE_BS_2018.10.05.PDF>


#### Summary {#summary}

-   there is many things that claim to be agile, but are not realy
    agile
-   this document explains some key points to look at when trying to
    detect is something is just saying it's agile.
-   it provides some questions you could ask to a development team,
    users, and other parties
    to see if they are really using agile
-   It would be useful to someone trying to understand the real

    nature of a project as oposed to the way it is described.
-   I can't beleive he keeps hitting the Enter button on that macbook like its
    somekind of carnaval game. I don't keed to know how emphatically
    you feel about your own trying.


#### I found this Linked in An article about how website focused dev practices dont create stability {#i-found-this-linked-in-an-article-about-how-website-focused-dev-practices-dont-create-stability}

from this HN thread <https://news.ycombinator.com/item?id=22309291>
[Here](https://www.bitlog.com/2020/02/12/why-are-we-so-bad-at-software-engineering/) and arccive [Here](https://web.archive.org/web/20200215122420/https://www.bitlog.com/2020/02/12/why-are-we-so-bad-at-software-engineering/)
to quote:
“I don’t quite know how to put this, but our entire field is bad at what we do, and if you rely on us, everyone will die.” Our industry’s mindset grew in an environment where failure is cheap and we are incentivized to move quickly.


### <span class="todo DONE_">DONE </span> What are some Taskboard tools for project management? {#what-are-some-taskboard-tools-for-project-management}

-   <https://clubhouse.io/>
    A fast web bassed tool. free tier. All the agile bells and
    whistles.
-   Ice scrum
    Java app. Can self host it with docker. Is reasonably functional
    for personal use.. Most advanced features not avalible in free
    version. Nice UI
-   Weka
    I havn't used this in a while. there are many install options,
    even a snap. putting it here So I don't forget the name
-   Gitlab. also has these things.. but also alot more.. so its not
    the lightweight solution here..
-   Trello?
-   And lots more.


### <span class="todo DONE_">DONE </span> What was that alternative to Terraform that used general coding languages? {#what-was-that-alternative-to-terraform-that-used-general-coding-languages}

It was [Plumi](https://www.pulumi.com/docs/index.html)

-   Why Pulumi?

By using real languages for infrastructure as code, you get many
benefits: IDEs, abstractions including functions, classes, and
packages, existing debugging and testing tools, and more. The
result is greater productivity with far less copy and paste, and it
works the same way no matter which cloud you're targeting

Maybe I should give it a try. Terrafrom's domaon specific langaige
is a bit special.


### <span class="todo DONE_">DONE </span> Neural Net generated Music? {#neural-net-generated-music}


#### Metal {#metal}

-   <https://dadabots.bandcamp.com/album/coditany-of-timeness>
    (and other from the same people <http://dadabots.com/music.php>)


#### Melody {#melody}

-   open AI has [Musenet](https://www.openai.com/blog/musenet/) which can make melodies in the style of
    diferenet artits


#### Notes. {#notes-dot}

-   I was reading about it
    [on Hacker News](https://news.ycombinator.com/item?id=22322408) Where they were talking about a generated rap
    song.
-   Sometimes AI generated = the agl. spits out a huge amount of
    stuff and some humans choose a few not bad examples from anoung
    it all.
-   [Art](https://news.ycombinator.com/item?id=22344254)


### <span class="todo DONE_">DONE </span> China-news {#china-news}

[China Brief](https://jamestown.org/programs/cb/about-china-brief/) is a very indepth policy analisys level review of news
and politics out of China.


### <span class="todo DONE_">DONE </span> Less wrong {#less-wrong}


#### What is less wrong? {#what-is-less-wrong}

<https://news.ycombinator.com/item?id=22323090>
<https://www.lesswrong.com/s/SGB7Y5WERh4skwtnb>
less wrong is a collection of writings by, Eliezer Yudkowsky,
Robin Hanson, and others, on words and cognition, organised into
collections called Sequences.


#### Not to be confused with {#not-to-be-confused-with}

MontyPython which was "do not adjust your set" meets "the 1948 show"


### <span class="todo DONE_">DONE </span> links-2020-02-17 {#links-2020-02-17}

-   About PIA vpn sale and trust etc

<https://news.ycombinator.com/item?id=21679682>

-   Art generated
    <https://art42.net/>
-   Langauge learning hacking
    <https://news.ycombinator.com/item?id=22341983>
    note:
    BTBurke 11 minutes ago [-]

I don't believe there is a shortcut for "hacking" languages. I'm a diplomat, and currently learning my fourth language to the C1+ level.
When we learn languages, it's a full time job. It was 9 months to learn Mandarin to a B1, 6 months to a C1+ in Spanish, and I'm currently at a B1 in Estonian after 5 months.

There are several things I think are crucial after years of full time study (note: this assumes you're going for professional fluency, not just touring around the country where interactions are largely scripted and predictable):

There is no substitute for production - you must speak the language with a native speaker (not an app) and talk about topics that are relevant to the kind of scenarios you anticipate. We spend the first several months discussing current events in target language - at first scripted, then later free form. This builds vocabulary and helps fluency. This is quickly expanded to discussing current events in depth and participating in mock debates.

Give mini presentations - target 3-5 minutes of talking about a relevant topic with little prep time. The difference between intermediate and advanced is the ability to move from discussing only facts to making a coherent argument. Native speakers will often not be able to follow your train of thought without learning to connect cause and effect using structures appropriate for your language.

Interview native speakers - prepare 2-3 questions about a particular topic and check your comprehension by translating their answers to English. This obviously helps build your comprehension, but also helps to learn to "automate" comprehension while you are thinking about something else. If you can take notes in English while a native speaker is talking at normal speed (and achieving 90%+ accuracy), it will make it easier for you to participate in normal speed conversations.

Read target language news - this is critical for expanding vocabulary and learning colocations - knowing what verbs are used in particular contexts (e.g., do they say "I talked with X" or "I talked to X". Do they say country X shot, launched, or threw a rocket?)

Bottom line - language learning is not just about the number of hours you put in. The quality and type of practice you do matters a lot. You aren't going to be fluent via Duolingo alone. You need to put in the time using structured practice with native speakers to really learn anything.


### <span class="todo DONE_">DONE </span> 2020-02-18-links {#2020-02-18-links}


#### SSM Session manager for aws {#ssm-session-manager-for-aws}

This is a way to access aws things like EC2 instances without the
need for having a network ingress to port 22 and ssh.
It is manage by IAM and policies. So it is easier to audit than
SSH keys
It is not as good as ssh for tunneling and scp so
[Here is a way to use it to connect to ssh](https://github.com/elpy1/ssh-over-ssm)


#### Discussion of VPNs and aws {#discussion-of-vpns-and-aws}

With all the news of global epidemics, it reminded me that the
office I am in at the moment
[Reddit](https://www.reddit.com/r/aws/comments/f2t9ds/aws_client_vpn_seems_like_a_rip_off_no/)
TIL:

-   AWS managed services are expensive. There is angry abusive
    reddit debate over if it is cheaper to pay engineers to make one
    on your own ec2 instances, or to pay for a managed VPN.
    [AWS vpn pricing](https://aws.amazon.com/vpn/pricing/)
-   If VPN is a critical thing, then there is an advantage to using
    the ASW service, in terms of avaliability and scaling etc
-   there are diferences in the pricing. OpenVPN charges per seat,
    otehrs might charge for uptime and throughput.
-   In a mass-surveilance world, why would I trust AWS VPN not to
    have a backdoor?
-   [pritunl](https://pritunl.com/#promo) is a commercial OpenVPN wrapper
    -   Pritunl has a free version that's excellent for simple use
        cases,
-   "would it be cheaper to just make a cloud formation template to
    spin up my own version of this service on demand?"
-   <https://github.com/joshmcgrath08/openvpn_on_ec2>
    -   explains how to make an ec2 instance with openVPN, and the
        template automatees to the extent that you also get a
        download link for the credentials needed to sign into it.
-   <https://github.com/hwdsl2/docker-ipsec-vpn-server>
    -   or a docker image for ipsec server


#### The port-knocking on AWS {#the-port-knocking-on-aws}

the goal would be to keep your logs from being filled with junk
noise of auto scans. but still have a service online when you
needed it
[Reddit thread](https://www.reddit.com/r/aws/comments/6yks6t/the_portknock_protocol_and_aws_security_groups/) here.
I was interested in this because of the idea of having an endpoint
that you could call to add your current IP adress to a security
group through a lambda function or something .. then let yourself
into your ssh port, or what have you. but tunneling through
session manager might be another option.

-   [hole punch](https://github.com/erik/holepunch) seems to do this


### <span class="todo DONE_">DONE </span> Fonts {#fonts}


#### Learn about webfonts from HN discussion. {#learn-about-webfonts-from-hn-discussion-dot}

-   <https://news.ycombinator.com/item?id=22368247>


#### Why are web fonts used? {#why-are-web-fonts-used}

webfonts are used because fonts are considered intelectual
proprty, and have restrictive licensing. If a web designer wants
to use a font on a webpage it can be a big prblem to get the
licence to use it. by using a font api, you are using fonts that
are already licenced by google.
web fonts are also a way to make traffic more efficient, because
many sites would be sharing the same font data, so they can be
cached easier
it also means that only google gets to track you data, and not
lots of diferent font providers
without them we would be limited to looking at web pages in fonts
that are installed on the OS, and OSes all have diferent sets of
fonts, so pages would look diferent on diferent systems


#### What fonts are on all systems? {#what-fonts-are-on-all-systems}

there are a few microsoft fonts that were released in the 90s that
can be found on linux to, but they have to be installed from a CAB
file.


#### Spirals as base for font design {#spirals-as-base-for-font-design}

basically bu variying the value of a curve equation you can get
many types of curves, these curves can be put together in
descretly to make a shape. This work is about using a sipral
equation to make up fonts that look nice.

A man who worked on the google font project at launch, Raph
Levien, wrote a [PHD thesis](https://levien.com/phd/phd.html) called "From Spiral to Spline: Optimal
Techniques in Interactive Curve Design".
"The Euler spiral is an excellent choice for this generator
curve."
"the properties of the various interpolating splines
explored in this thesis, to facilitate choosing the best one for
any given application. In using these splines for drawing a
number of fonts, I also found they brought an aesthetic quality to
the work."


### <span class="todo DONE_">DONE </span> Discontinuities {#discontinuities}


#### What was that site that had logs of graphs showing discontinious data and its implications {#what-was-that-site-that-had-logs-of-graphs-showing-discontinious-data-and-its-implications}

<https://danluu.com/discontinuities/>
for instance, the rigged voting in russia can be seen by the round
numbers of voter regidtered at polling stations.
[via HN](https://news.ycombinator.com/item?id=22378555)


### <span class="todo DONE_">DONE </span> Parsing-Text {#parsing-text}


#### What was that Google project for Parsing text into parts of speech? {#what-was-that-google-project-for-parsing-text-into-parts-of-speech}

SyntaxNet


#### what is SyntaxNet {#what-is-syntaxnet}

A NN framework for NLP with tensorflow.
It includes training data and "arsey McParseface, an English
parser that we have trained for you, and that you can use to
analyze" text.

-   It seems to have dissapared from the tensorflow github page.


### <span class="todo DONE_">DONE </span> Epidemiology {#epidemiology}


#### What's R0 {#what-s-r0}

R Naught is the rate of infection spread. The number is the number
of other people an infected person will ingect.
R1 = 1 more person
R2 = 2 more people
<https://sph.umich.edu/pursuit/2020posts/how-scientists-quantify-outbreaks.html>
CORVID-19 R0 is maybe from 1.5 - 4.08 .. but it depends on the
population and the desease controll measures.
[Here](https://github.com/midas-network/COVID-19/tree/master/parameter_estimates/2019_novel_coronavirus#effective-reproduction-number) has some sources for R


#### Info Sources {#info-sources}

[maps and tools and data](https://github.com/midas-network/COVID-19/wiki/Software-Tools#visualization)
[pandemic](https://virologydownunder.com/past-time-to-tell-the-public-it-will-probably-go-pandemic-and-we-should-all-prepare-now/)


#### How to deal with Pneumonia {#how-to-deal-with-pneumonia}

[1](https://www.verywellhealth.com/pneumonia-treatments-770681) [2](https://www.medicalnewstoday.com/articles/320881)

-   fever
    -   tepid bath
        -   or towels
    -   fenegreek tea
        -   makes you sweet?
    -   anti-flam
        -   ibuprofin
        -   asprin
        -   tumerick
-   breathing (mucus)
    -   caffiene
        -   coffee
        -   green/black tea
    -   tea
        -   pepermint
        -   eucalyptus
        -   fenegreek powder
    -   nebulizer
    -   humidifyer
    -   deep in / cough out 10x
-   chills
    -   warm drink
-   inflamation
    -   tumeric
    -   ginger
-   infection
    -   depends on type of infection
    -   maybe cant with a virus


#### How should I use a respirator? {#how-should-i-use-a-respirator}

-   [N95 useage](https://www.bu.edu/ehs/files/2014/08/N95-Respirators-Training.pdf) training.
    -   straps
    -   checks
    -   nose seal
-   [CDC on reusing](https://www.cdc.gov/niosh/topics/hcwcontrols/recommendedguidanceextuse.html) resperators
    -   it depends on the things you are guarding against. Is it
        likely to spread through contact? Are you going to get
        spalshed or sprayed in the face?
    -   Try to take it on and off as little as possible
    -   make sure it can maintain its fit and function
        -   are the straps getting stretched so it doesnt seal?
    -   If its not dusty, the use lenght is determed by how long you
        can keep it hygenic.
    -   Try to limit surface contamination of resperator
        -   dont touch it as much as possible
        -   cover it with a surgical mask or face guard
        -   dont touch the inside
        -   put it on with gloves and discard them
    -   Discard it if it becomes contaminated
        -   areisol / liquid spray
    -   Hand hygene before and after touching
        -   soap wash or sanitizer
    -   Check manufacturers advice on resue
    -   Dont share between people.
    -   lable the resperator
        -   use times
        -   user


#### Corovid-19 {#corovid-19}

-   Clean surfaces with diluted Bleech.


### <span class="todo TODO_">TODO </span> Commands that make lots of text scroll on the screen {#commands-that-make-lots-of-text-scroll-on-the-screen}


#### Why? {#why}

because it looks cool and computery


#### commands {#commands}

-   tcpdump -A
-   cat /dev/urandom
-   htop
-   tail -f /var/logs/syslog | lnav


### <span class="todo DONE_">DONE </span> What was that better Thesaurus site? {#what-was-that-better-thesaurus-site}

[Onelook](https://onelook.com/) because it links to many many other databases. some of them
very cool like [MnemonicDictionary](https://mnemonicdictionary.com/) and it has a port mantaux
generator.


### <span class="todo DONE_">DONE </span> merger between our Milky Way galaxy and the neighbouring Andromeda galaxy {#merger-between-our-milky-way-galaxy-and-the-neighbouring-andromeda-galaxy}

{{<figure src="/images/galaxycrash.jpg">}}
{{<figure src="/images/starforming.jpg">}}
:PROPERTIES:


### <span class="todo DONE_">DONE </span> Pig sicknesses {#pig-sicknesses}

:EXPORT\_FILE\_NAME: pig-sicknesses


#### What is wrong with pigs at the moment? {#what-is-wrong-with-pigs-at-the-moment}

-   [Classical Swine Fever (CSF) and African Swine Fever(ASF)](https://www.env.go.jp/nature/choju/infection/notice/guidance.pdf)


#### How is it spreading in Japan? {#how-is-it-spreading-in-japan}

[it is spreading out from around the middle](https://www.maff.go.jp/j/syouan/douei/csf/domestic.html) and maybe passing
between wild pigs and farm pigs via smaller animals coming in and
out of pig farms.


#### What did you learn from this? {#what-did-you-learn-from-this}

about how the environmental persistence of this virus and its many
and varied routes of transmission make it spread by local
epidemics and then become endemic in populations.
it is 80%+ fatal to pigs


### <span class="todo TODO_">TODO </span> Interesting HN Discussions. {#interesting-hn-discussions-dot}


#### This analysis seems superficial and xenophobic {#this-analysis-seems-superficial-and-xenophobic}

<https://news.ycombinator.com/item?id=22522247>

-   a good rebuff of the common way we talk about people in the
    middle east.


#### Websites have evolved back to static HTML/CSS/JS files {#websites-have-evolved-back-to-static-html-css-js-files}

-   <https://news.ycombinator.com/item?id=22519090>
-   Talking about the rise of serverless webpages and static site
    generators.


#### How to schedule meeting and be nice about it {#how-to-schedule-meeting-and-be-nice-about-it}

<https://news.ycombinator.com/item?id=22483847>


### <span class="todo TODO_">TODO </span> Development {#development}


#### Frameworks {#frameworks}

-   APP

    -   Remake

        <https://remaketheweb.com/>
        This is an app framework that aims to make app development as
        easy as writing HTML. This could e good for learners, or things
        to make quickly and simply. Use with kids?


### <span class="todo TODO_">TODO </span> Stuff I want to read {#stuff-i-want-to-read}


#### [how-to-build-a-learning-machine](https://superorganizers.substack.com/p/how-to-build-a-learning-machine) {#how-to-build-a-learning-machine}


#### [if-money-doesnt-make-you-happy.nov-12-20101](https://scholar.harvard.edu/files/danielgilbert/files/if-money-doesnt-make-you-happy.nov-12-20101.pdf) {#if-money-doesnt-make-you-happy-dot-nov-12-20101}


#### The feeds discussed in this post {#the-feeds-discussed-in-this-post}

<https://news.ycombinator.com/item?id=22744171>


### <span class="todo TODO_">TODO </span> phrases {#phrases}

Phrases to re-read


#### [Economic anxiety, a policy pushed by financial planners, is what motivates. Not money.](https://news.ycombinator.com/item?id=20682564) {#economic-anxiety-a-policy-pushed-by-financial-planners-is-what-motivates-dot-not-money-dot}

-   You could decide money and the rat race are pointless and
    decide to just stop pursuing it. And you'll survive... for a
    time. Then you won't be able to function in society. Won't be
    able to eat, or have a place to live, effectively the
    equivalent of having your skull bashed in like in that
    previous world.
-   there's a certain amount of hubris in assuming that you know
    better than the norms. Often, norms became norms because they
    work for a lot of people.
-   Don't buy into the myths of scarcity and learned helplessness
    society uses to get people to play along. Everyone's capable
    of learning how to reconnect with and be an active contributor
    to nature. We


#### Hyper-sane {#hyper-sane}

It is not just that the ‘sane’ are irrational but that they lack
scope and range, as though they’ve grown into the prisoners of
their arbitrary lives, locked up in their own dark and narrow
subjectivity. Unable to take leave of their selves, they hardly
look around them, barely see beauty and possibility, rarely
contemplate the bigger picture

-   NOTE: I'm not sure this is a thing


#### "He that would make his own liberty secure, must guard even his enemy from oppression; for if he violates this duty, he establishes a precedent that will reach to himself." {#he-that-would-make-his-own-liberty-secure-must-guard-even-his-enemy-from-oppression-for-if-he-violates-this-duty-he-establishes-a-precedent-that-will-reach-to-himself-dot}

-   <https://news.ycombinator.com/item?id=22540337>


#### long-range amorphous order {#long-range-amorphous-order}

“long-range amorphous order,” where each molecule feels and
affects the position of every other, so that in order to move,
they must move as one. The hidden long-range order of this
putative state could rival the more obvious orderliness of a
crystal. “That observation right there was at the heart of why
people thought there should be an ideal glass,"

-   perfect glass


#### How an open-loop scrubber works {#how-an-open-loop-scrubber-works}

-   <https://www.theguardian.com/environment/2018/oct/29/thousands-of-ships-could-dump-pollutants-at-sea-to-avoid-dirty-fuel-ban>
-   Exhaust gas is sprayed with seawater to wash out sulphur oxide
-   Washwater is treated and monitored
-   Treated washwater is discharged into the sea


#### ontogeny {#ontogeny}

I’ve come to love this term ontogeny because it brings together,
in one helpful word, the flux of becoming that scientists as well
as existentialists seek to understand. By rallying readers with
their slogan ‘existence precedes essence’, Beauvoir and Sartre
were drawing attention to the utterly singular way in which we
each become the selves that we are, with our own memories, stories
and storytelling habits.

-   What point dod we become human?

    if evolution is a continious process.. then there is no one event
    that changes from one species to the next.. we cant draw a linet:W
    when humanity begun..
    maybe it hasn't even started yet.. we havn't become human
    yet.. we are skill walking apes.


#### Forced filter {#forced-filter}

<https://news.ycombinator.com/item?id=22744311>

-   Agreed. It's not the feed that broke the internet – it's the forced filter.

The notion that forced filtration, reprioritization, and chronological
rearrangement of content is implicit the idea of information feeds
(search, social media, etc) shows how deep the brokenness is
    baked in.

-   I've always imagined animals on a farm feeding happily at a trough, unaware of their impending doom.


#### It's hard to make good choices when you're only surrounded by bad one. {#it-s-hard-to-make-good-choices-when-you-re-only-surrounded-by-bad-one-dot}

<https://news.ycombinator.com/item?id=22744409>
You're spot on. But really... all people are basically the
same. And like Google, they're incentivized by the system to be
horrible to each other and/or horrible to the environment. I think
people all have a choice. But I think the good choices are really
hard to make when you're only surrounded by bad choices.

-   This sentiment reflects some of what I have been confronted with
    moving out of one society and culture into another. How our
    environment is a big limit on our choices and even perceptions
    of whats choosable.


### <span class="todo DONE_">DONE </span> What was that math visuals software? {#what-was-that-math-visuals-software}

-   <https://www.geogebra.org/?lang=en>


### <span class="todo DONE_">DONE </span> Links 2020-03-18 {#links-2020-03-18}

<https://developers.google.com/assistant/tools/sound-library> | Sound Library  |  Conversational Actions  |  Google Developers
<https://developer.amazon.com/en-US/docs/alexa/custom-skills/speechcon-reference-interjections-english-australia.html> | Speechcon Reference (Interjections): English (AU) | Alexa Skills Kit
<https://aeon.co/ideas/hypocognition-is-a-censorship-tool-that-mutes-what-we-can-feel?utm_medium=feed&utm_source=atom-feed> | Hypocognition is a censorship tool that mutes what we can feel | Aeon Ideas
<https://news.ycombinator.com/item?id=20676959> | The hypersane are among us, if only we are prepared to look | Hacker News
<https://aeon.co/ideas/the-hypersane-are-among-us-if-only-we-are-prepared-to-look> | The hypersane are among us, if only we are prepared to look | Aeon Ideas
<https://www.nickkolenda.com/psychological-pricing-strategies/#pricing-t1> | Psychological Pricing: An Enormous List of Tactics
<https://feedly.com/i/entry/IZR+JDs9ZnUqD6xpCfaGbmkqTZtq3kpqwIx1GMAFNLo=_170eb1798ad:25bc8c8:79e8e7ea> | All Personal Feeds
<http://docs.bigbluebutton.org/> | BigBlueButton : BigBlueButton
<https://www.cambridge.org/core/what-we-publish/textbooks> | Textbooks | What We Publish | Cambridge Core
<https://www.cambridge.org/core/books/key-questions-in-language-teaching/how-do-we-carry-out-second-language-research/D5DC57AD2B3C1319AB9B460E9D29C894/online-view> |
How Do We Carry Out Second Language Research? (Chapter 6) - Key
Questions in Language Teaching


### <span class="todo DONE_">DONE </span> How do I grep in a minified file? {#how-do-i-grep-in-a-minified-file}

when a file has all its text on one big long line, grep is not very
useful. how can i just get the part of a line I want?


#### Use regex to match character before and after, and -o to only show match. {#use-regex-to-match-character-before-and-after-and-o-to-only-show-match-dot}

grep -o "\\{0,15\\}search\_string\\{0,20\\}" file


### <span class="todo DONE_">DONE </span> Android weather apps {#android-weather-apps}

I was reading about apple buying a weather server and turning off
it's api and stopping it's android apps. in that discussion there
was a few suggested alternatives.

-   [Flowx: Weather Map Forecast](https://play.google.com/store/apps/details?id=com.enzuredigital.weatherbomb&hl=en_US)
-   [Klara weather](https://play.google.com/store/apps/details?id=org.androworks.klara)
-   [YR](https://play.google.com/store/apps/details?id=no.nrk.yr&hl=en)
-   [Hello Weather](https://play.google.com/store/apps/details?id=com.helloweatherapp&ah=RtPyJfHEtl2bzH0QB-kPw2m2RIs)


### <span class="todo DONE_">DONE </span> How do I make gnu screen look better? {#how-do-i-make-gnu-screen-look-better}


#### How do I remove the white dividers between splits? {#how-do-i-remove-the-white-dividers-between-splits}

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


### <span class="todo DONE_">DONE </span> Frameworks and things {#frameworks-and-things}


#### design {#design}

-   [Tailwind](https://tailwindcss.com/) A utility-first CSS framework for rapidly building
    custom designs.


### <span class="todo DONE_">DONE </span> Networking and remote {#networking-and-remote}


#### ZeroTrust networking {#zerotrust-networking}

-   [tail scale](https://tailscale.com) . it's like a lan over the internet


### <span class="todo DONE_">DONE </span> Making vim look better {#making-vim-look-better}


#### How Do I make vim buffer centered in the middle of the page, and have nerdtree list toggle over the margin empty space? {#how-do-i-make-vim-buffer-centered-in-the-middle-of-the-page-and-have-nerdtree-list-toggle-over-the-margin-empty-space}

-   Goyo
    <https://jennifermack.net/2017/02/01/recreating-ulysses-with-vim/>


#### How Do I show indentation with VIM? {#how-do-i-show-indentation-with-vim}

-   Plugin 'nathanaelkane/vim-indent-guides'


### <span class="todo DONE_">DONE </span> What is a tool for using Brackets editor for academic writing? {#what-is-a-tool-for-using-brackets-editor-for-academic-writing}


#### [Brackets Zotero](https://baig.github.io/brackets-zotero/) {#brackets-zotero}


### <span class="todo DONE_">DONE </span> How do i make Gnu/Screen multi-user {#how-do-i-make-gnu-screen-multi-user}


#### [Follow instructions here](https://www.mfitzp.com/article/collaborate-in-the-shell-with-screen-multiuser/) {#follow-instructions-here}

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


### <span class="todo DONE_">DONE </span> What was that site that Trimed articles to load better? {#what-was-that-site-that-trimed-articles-to-load-better}


#### <https://beta.trimread.com/> {#https-beta-dot-trimread-dot-com}

-   I wonder if there is one that works for japanese news sites that
    spread things over multiple pages.


### <span class="todo TODO_">TODO </span> How can I alarm if my gitlab backups arn't running? {#how-can-i-alarm-if-my-gitlab-backups-arn-t-running}

I just had an incident where the crontab on my gitlab host had been
removed for about a month. Because of this the backups to s3 had
not been running, and the existing backups were all deleted by the
s3 bucket policy to delete after 14 days. This reveals two problems
with my system. I have a dashboard set up to monitor the bakups,
but no-one looks at it.

-   it is possible to be left with no backups
-   there was no alarming that the backups were not running.


#### How can I alarm if the backup didn't run. {#how-can-i-alarm-if-the-backup-didn-t-run-dot}

Seeming as the AWS tools eem to be the most fail safe(unlikely to
have configuration drift), one way
could be to alarm on the items in the s3
bucket. assuming that nothing else but backups should be in this
bucket. I would would idealy want to check each day if a new
backup file has appared, and if not send an alert message.

-   [This](https://stackoverflow.com/questions/59063713/how-to-setup-cloud-watch-alarm-for-s3-bucket-if-no-data-is-received-in-bucket-fo) stackoverflow answer talks about "Create an Amazon
    CloudWatch Events rule to trigger an AWS Lambda function" That
    seems to be a bit complicatione
-   Maybe I can just make the bucket publish to an SNS topic on any
    create event. Then any time a backup runs a notification will
    be published to that topic. We don't care to know if the back up runs
    successfully, that would be information overload. So we can use
    Cloudwatch metrics to set up an alarm to monitor the numbers of
    messages published to that topic per day. If there isn't a
    message published, then we can assume the bakcup hasn't run and
    we need to investigate.

-   How can i make this with terraform?

    What are the components?

    -   SNS topic to recieve s3 file events
    -   [S3 Events configuration](https://www.terraform.io/docs/providers/aws/r/s3_bucket_notification.html)

    -   Cloudwatch metic
        -   maybe this is can be created together with the alarm.(maybe
            it doesnt need to be created because we are not using a
            custome metric, and it already exists, and we can just query
            it in the alarm config)
    -   [Cloud watch alarm](https://www.terraform.io/docs/providers/aws/r/cloudwatch_metric_alarm.html)
        following
        [This](https://webcache.googleusercontent.com/search?q=cache:pweBgqTEfqQJ:https://underthehood.meltwater.com/blog/2019/01/31/monitoring-your-system-heartbeat-using-cloudwatch/+&cd=1&hl=ja&ct=clnk&gl=jp&client=firefox-b-d) example.
        -   We will set the "period" to "one day(in seconds 86400)" (the frequency of backups)
        -   set "treat\_missing\_data" to "breeching"
            -   so if no data (message) is recieved in a day it will invoke the configured "alarm\_action"
        -
    -   SNS topic to recieve alarms(use existing)

    -   That was annoying.

        There are some big gotcha with policy permissions to get this
        working via terraform.. In the end I have just set it up by hand
        for the time being because I have other things to get done.

        The alarm:

        Threshold
        NumberOfMessagesPublished < 1 for 1 datapoints within 1 day
        Last change
        2020-04-20 07:17:25
        ARN
        arn:aws:cloudwatch:::alarm:gitlab\_backups\_missing

        amespace
        AWS/SNS
        Metric name
        NumberOfMessagesPublished
        TopicName
        ops-gitlab-backup-metrics-monitor
        Statistic
        Maximum
        Period
        1 day

        Datapoints to alarm
        1 out of 1
        Missing data treatment
        Treat missing data as bad (breaching threshold)
        Percentiles with low samples
        evaluate

        The bucket notification config:
        ✓　All object create events
        　　send to SNS topic:
        ops-gitlab-backup-metrics-monitor

        And lots of policies to allow that to happen.


## Emacs {#emacs}

All posts in here will have the category set to _emacs_.


### <span class="todo TODO_">TODO </span> Writing Hugo blog in org {#writing-hugo-blog-in-org}


#### First heading within the post {#first-heading-within-the-post}

-   This post will be exported as  a s
    `content/posts/writing-hugo-blog-in-org-subtree-export.md`.
-   Its title will be "Writing Hugo blog in Org".
-   It will have _hugo_ and _org_ tags and _emacs_ as category.
-   The menu item _weight_ and post _weight_ are auto-calculated.
-   The menu item _identifier_ is auto-set.
-   The _lastmod_ property in the front-matter is set automatically to
    the time of export.

-   A sub-heading under that heading

    -   It's draft state will be marked as `true` as the subtree has a the
        todo state set to _TODO_.

    With the point <span class="underline">anywhere</span> in this _Writing Hugo blog in Org_ post
    subtree, do `C-c C-e H H` to export just this post.

    The exported Markdown has a little comment footer as set in the _Local
    Variables_ section below.

-   using hugo shortcodes

    <https://github.com/kaushalmodi/ox-hugo/issues/242>
    <https://gohugo.io/content-management/shortcodes/>

    ```nil
    #+html: {{< gist iveskins 4b0c620f3e51968ff67453ac78f2fb59 >}}
    ```

-   Using images

    1.  put them in the ./static/images/ folder
    2.  link them as /static/images/name surrounded by [[ s

[^fn:1]: Japanese word with Japanese definition
[^fn:2]: <https://web.archive.org/web/20190924112658/https://orgmode.org/manual/Footnotes.html>
[^fn:3]: proof of concept
[^fn:4]: RightScale Docs - <https://docs.rightscale.com/cm/dashboard/clouds/aws/rds_subnet_groups.html>
