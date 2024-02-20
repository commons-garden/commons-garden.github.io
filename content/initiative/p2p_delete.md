---
title: P2P Delete
display: public
status: ongoing
facilitator: [mixmix, nonlinear]
description: Serverless irretrievable delete
category: initiative
date: 2023-03-07
link: https://hackmd.io/@praxis/p2p-delete
comm_title: signal group
comm_link: https://signal.group/#CjQKIGFSis4tbGdzpujg_Xw-UudxHZnnPuxmxPfFjSbzvII7EhAXQHs1aCqWBymiid6TMV78
note_title: hackmd
note_link: https://hackmd.io/@praxis/p2p-delete
---

# Second meeting notes

> 📌 to consolidate

## Threads to explore

- shared language
- alt deletion
- making meaning out of deletion
- owner/ agency/ control
- delete/ append
- white-out/ destroy
- signed intentions/ auditability
- trinaries/ trade-offs
- data structures
- deletion in nature
- adoption of standards/ advocacy

## Advocacy




## Data structures

Are the changes small?
- yes (text)
  - trilemma (in some CRDTs, in realtime) <= seph
    - efficency
    - byzantian fault tollerance
    - ability to delete
  - use a nonce to every single edit, as this allows you to avoid rainbox tables
- no:
  - don't need nonce because who cares

Bengo [ his summary ]

Holochain
- receipts of acknowledgment of making a change

What if every blob sent out was unique to a recipient
What if we predictably mutate some piece of data every e.g. 10 days
  - so then we know the "epoch" in which it was leaked
  - companies already do this by sharing emails with unique punctuation/words


Promising approach:
- byzanine fault tollerant CRDTs (klepan approach)



exquisite corpse
- eventual possible forgetting
  - the system is not guarenteed deleting, and "forgetting" shifts us from permanence of delete
  - buried till it's hard to find it, obfuscation, garbage collection, long tail
- complete knowledge maliability
  - consent on joining that info can be modified
  - google docs
- requested context expungement
  - request to send to a service to remove a thing to remove all context around the thing
  - knowledge that's been explunged from a particular context
- comfirmed reproduceable removal
  - you have a unikernal/vm which provably executes a deletion - runs a thing and publishes a thing
  - protocol designed to prove the deletion of a particular thing
- ephemeral file expiry
  - a file that's been marked for deletion... and has reached that expiry
  - a file that hasn't been deleted, but it's relevance/ reliability has expired
  - open source code that's maintenance guarentee has expired and if you still have it and use it, that's on you



how does GDPR get audited? how does the EU know a company has removed stuff?
are there legal affordances which say "this info is no longer permissible in court"
  - e.g. revenge porn protection
    - what about we all sign that we deleted something, then it 

recovery in conversation
  - opposite/ in tension to deletion
  - deletion is "the intention to prevent harm"
    - there are other ways to do this ... e.g. repair

### Spectrum of deletion

### Words to drop


### Purpose for deletion

sometimes your deletion is my censorship

----



Sometimes we want to make a piece of data irretrievable.
Given a distributed system subject to intermittent connectivity, partitions, and variable trust,
how do we effectively syndicate deletions among peers?
What does it mean for a distributed delete to be 'good enough'?

Data in systems like Hypercore and SSB is often "signed" by an author, which makes it particularly dangerous.
When the hash of the data is also signed,
the data's metadata can be used in a "Confirmation Of A File Attack" to prove that the author once possessed the data.

---

# First meeting notes

> 📌 to consolidate

# p2p delete

- p2p delete [signal group](https://signal.group/#CjQKIGFSis4tbGdzpujg_Xw-UudxHZnnPuxmxPfFjSbzvII7EhAXQHs1aCqWBymiid6TMV78)
- status: tentative as of Jan 13, 2023
- hashtag to use in other media: `#p2p-delete`

## Terminology

- disavow: demand in an auditable way that peers cease replicating data, and record instances of noncompliance.
- irretrievable: the inability to obtain data.
- tombstone: metadata left behind after deleting data, excluding the data itself.
- PII: personal identifiable information

## Problem Description

Sometimes we want to make a piece of data irretrievable.
Given a distributed system subject to intermittent connectivity, partitions, and variable trust,
how do we effectively syndicate deletions among peers?
What does it mean for a distributed delete to be 'good enough'?

Data in systems like Hypercore and SSB is often "signed" by an author, which makes it particularly dangerous.
When the hash of the data is also signed,
the data's metadata can be used in a "Confirmation Of A File Attack"
to prove that the author once possessed the data.

### Disaster scenario

- A) PII: personal identifiable information
    - biased scientific review
    - doxxing
      - yourself
      - another person
- B) Medical data
    - legality around holding / custodianship of data 
        - e.g. I move from Doctor A to Doctor B, then it becomes illegal for A to hold my data
- C) accidentally posted illegal info (illegal number attack)
- D) Company changes policies and need to reduce confusion
- E) Bad selfie
- F) My recipe is wrong/dangerous/useless
- G) unrepentant doxxer: ability of other peers to disavow message "i dont want to replicate this" (message block)

## Solution Shape

Our solution should:

1. Propagate deletes throughout a network for peers to enact.
2. Deleted content should not be replicated
    - we don't want to accidentally re-propogate previously deleted data
    - implies I may need to *remember* what's been deleted
3. Must not destroy verification of data structures
    - e.g. if a particular deleted message was part of a hash-chain, the hash of the content may be preserved while the content no longer exists
4. Be auditable
    - we want to find naughty / ignorant peers
    - test whether peers are following (1-3) ? or have published a "delete receipt"?
5. Must be able to delete data authored by other peers
    - this needs a lot more work/ clarification
    - do we need a hierarchy for deletes
    - disavowal (you should not hold it/ I'm blocking this message and if you hold it I'll hold you accountable)

## Questions

1. how do we know the data is "deleted"?
    - If a peer who is known to have received a deletion responds with the deleted data when asked, it is in violation.
2. can you delete someone elses content? (needed for doxx)
    - Delete for who? Can a peer autonomously forget data, or refuse to replicate it?
4. what happens to *links* to deleted records?
    - Ex: Signal's "this message was deleted" meta-message.
6. do we need *reasons* for deletion?
    - Does this annotation belong at the protocol or application layer?
8. how does edit relate to delete?
9. how do I know the "health" deletion?
10. can I *disavow* data? (demand data become irretrievable and hold noncompliant peers accountable)

## Neighbor technologies, solutions

## Threats to mitigate

1. tombstone spamming
    - an adversary can take up all your disk space by forcing you to propogate and remember tombstones


## state-of conference

A guest on Metagov Seminars (Wednesdays 12-1pm EST), midjuly https://metagov.org/seminar/

- [ ] consolidate unconference findings (here)
- [ ] video platform (jitsi)
- [ ] shared notes (post-its, visual)
- [ ] facilitator
- [ ] guests
- [ ] state-of deck (3-5 slides, summarizing what we collectively know so far (hackmd))
- [x] promotion (define audience to join, pitch, etc)
    - announcement
    - drop your questions (where? use kickoff questions to start)
    - event
    - initative update
- [x] date event
- [ ] rules for shared notes
- [x] code of conduct
- [ ] kickoff questions
    - how to deal with bad actors (governance)
    - how to deal when data is impermanent. is it troubling? is it liberating?
    - threat models for user personas
    - how do you deal with information assymetry on p2p. decisions in distributed context

## TODO

- [x] consolidate notes
- [ ] 📌 pin [message group](https://signal.group/#CjQKIGFSis4tbGdzpujg_Xw-UudxHZnnPuxmxPfFjSbzvII7EhAXQHs1aCqWBymiid6TMV78) messages that are worthy of documentation
- [ ] copy these messages here
- [ ] ✅ flag that pinend messages have been moved
- [ ] draft glossary
- [ ] discuss MetaGov session
- [ ] agree on glossary
- [ ] organise show + tell with MetaGov (virtual)


