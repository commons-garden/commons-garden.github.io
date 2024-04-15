---
title: P2P Delete
display: public
status: ongoing
description: Serverless irretrievable delete
date: 2023-03-07
link: https://hackmd.io/@praxis/p2p-delete
comm_title: signal group
comm_link: https://signal.group/#CjQKIGFSis4tbGdzpujg_Xw-UudxHZnnPuxmxPfFjSbzvII7EhAXQHs1aCqWBymiid6TMV78
note_title: hackmd
note_link: https://hackmd.io/@praxis/p2p-delete
---

Sometimes we want to make a piece of data irretrievable.
Given a distributed system subject to intermittent connectivity, partitions, and variable trust,
how do we effectively syndicate deletions among peers?
What does it mean for a distributed delete to be 'good enough'?

Data in systems like Hypercore and SSB is often "signed" by an author, which makes it particularly dangerous.
When the hash of the data is also signed,
the data's metadata can be used in a "Confirmation Of A File Attack" to prove that the author once possessed the data.
