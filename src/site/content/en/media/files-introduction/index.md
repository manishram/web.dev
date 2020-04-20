---
layout: post
title: Introduction
description: |
  TBD
date: 2017-06-30
updated: 2020-04-30
tags:
  - FFmpeg
  - files
  - Shaka
---

You might think that you can take a video camera and upload it to the web as is.
Indeed, video streaming sites such as YouTube or Vimeo let you do this. These
sites simplify video processing and uploading for the sake of customer
service. Preparing a video for serving from your own site is a bit more
complicated.

Video files come in a variety of formats. The format that comes off your camera,
typically an `mov` file, is good for recording and for editing and other early
post-production processes. But it is not good for streaming over the web. You
need to convert this file to a format such as an `mpeg` or a `web`.

Converting files requires running specialtiy tools with esoteric commands.
Internet searches for the correct arguments and flags is often frustrating. This
section provides background and instructions for converting media files from
your camera for serving on the web.

It begins with [Application basics](application-basics), which provides basic
instructions on the applicatins used to convert files. I explain converting
files in two parts. The first part, titled [For embedding](for-embedding), shows
how to prepare files for use with the `&lt;video>` element.

If you intend to use a video framework such as [Google's Shaka
Player](https://github.com/google/shaka-player), [JW
Player](https://developer.jwplayer.com/), or [Video.js](http://videojs.com/),
you will start by following the same instructions. Additionally, you will need
to separate the audio and video portions of your media into separate files. I
cover this in [For media frameworks](for-frameworks).