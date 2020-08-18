+++
title = "What is WebRTC"
author = ["T", "Ivan"]
lastmod = 2020-08-07T12:01:33+09:00
weight = 2077
draft = false
+++

communicate in 200ms for live video.

pieced to gether unrelated parts

Generic Description: real time communication between browsers and mobile.

now used to conferencing apps.
talk from one persone to another.

-   can do many interesting things:
    -   TOR's snowflake. censorship circumvention
        (p2p traffic not dependent on server)
    -   server-side proccessing (realtime processing of
        video/audio. subtitles etc)
    -   P2P data transfer. <http://pyget.com/about.html>
    -   augmented reality([hololense](https://www.youtube.com/watch?v=rgtGswLDsT4))


## WebRTC API {#webrtc-api}

-   SDP
    session description protocol
    declare properties about self.
    -   I support these codecs
    -   this is my ip
    -   these are the streams (tracks) I am going to send you


### How do I talk to you. {#how-do-i-talk-to-you-dot}

you have an IP that I cant directly access.
I have no idea where you are.
STUN server.

-   send a UDP packet to StunServer on :5000<>:5000
    punches a permanent hole through NAT
    sned a packet to NATB forwarded through to browser.
-   now can reply


### ORTC API {#ortc-api}


#### RTCPeenConnection {#rtcpeenconnection}

-   SRTP

    Sending video buffers of UDP losing 3% randomly stopping

    -   Jitter buffer
    -   ability to account for loss
        -   adjust amount of delay dynamically.
            -   waits for packets to arrive
            -   raise and lower latency
            -   ask for resending of lost packets.
                -   inside the latency time frame


#### DATAChannel {#datachannel}

-   SCTP

    -   Data transfer
    -   send binary back and forward, account for loss.
    -   negotiate a channel
        -   decide the parameters of the channel (lossy?)


#### DTLS {#dtls}

How do we communicate with people listening in the middle

-   TLS that accounts for loss
-   DH encryption
-   share states
    even if someone is eves-dropping they can't steal


### ICE {#ice}

-   how do I talk to you?


#### STUN {#stun}

punched hole through NAT

-   UDP

    -   Lossy connection
    -   enables it to be fast?


#### TURN {#turn}

B establish session with turn server
A sends packets through turn server.

-   TCP

-   RTP Framing


## Ever changing. {#ever-changing-dot}


## Pion-webrtc {#pion-webrtc}


## Current WebRTC designed with incumbent application in mind {#current-webrtc-designed-with-incumbent-application-in-mind}

-   no access to send arbitrary video
-   no access to bring own decoder.


## All in Go. {#all-in-go-dot}
