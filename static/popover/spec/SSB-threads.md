---
title: SSB threads
category: spec
type: public
description: How to post and reply to messages
status: stable
scope: SSB
license: CC0-1.0
author: [mix]
initiative: 
reviewed: [staltz, cel]
implemented: [patchwork, manyverse, planetary, patchfox]
date: 2023-03-07
link: https://github.com/ssbc/sips/blob/964e9a5cf407f1adf6e26f3b656c0e769f21caf4/010.md
platform: github
---
The post message type is the foundational unit for talking with peers on the original scuttlebutt network.

Post messages can be used standalone, but are most commonly collected as sets of related messages and formed into a "thread".

During rendering, threads of posts are also further decorated with vote messages (for likes), and about messages (for displaying author details).

