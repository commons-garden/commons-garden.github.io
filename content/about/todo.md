---
title: TODO
type: public
status: ongoing
description: Our next steps
category: about
author: [nonlinear]
date: 2023-09-10
---

## First

- [ ] document p2p-delete 📌
- [x] document knowledge ecology 📌
- [ ] keep working on [category/criteria diagram](https://hackmd.io/@mixmix/rywE-3P1T/edit)
- [ ] one emoji per category
- [x] remove salon, move to initiative

## Admin

- [ ] review [open collective](https://opencollective.com/commons-garden)
- [ ] define gardeners statuses (when a grdener was facilitated by other and then facilitate someone, etc)
- [ ] what do we call our ongoing discussion groups? other than salon?

## subpages

- [ ] page template checkjs if slug has a folder and:
	- lists all public pages in alphabetical order, into a table of content
	- folder pages point to original page
- [ ] subgroups should not be listed on list.html (or should? we need at least a new template)

## Workflows

Discuss how we do things

- [ ] redirect template: `p2p-delete` becomes `p2p_delete`
- [ ] redirect policy

## Internal documentation

How we write and update documentation for our facilitators?

- [ ] list inventory of initial tutorials we need
- [ ] maybe as we pass on knowledge, we write our manuals
- [ ] checklists. CHECKLISTS!
- [ ] adding categories tutorial: css, nav, json, etc
- [ ] template inside tutorial (loop from yml file)

## Design

- [ ] design open graph image
- [ ] design favicons
- [ ] design stickers
- [ ] reorganize `layout.scss`
- [ ] bg animation (vector, subtle)
- [x] blockquote, no count, no hover if alone
- [x] fix select error on non-firefox browsers
- [ ] fix text wrap on gardener template (break-word)

## Gardener template

- [x] loop thru facilitator, author, helper
- [x] loop only thru public
- [x] empty state
- [x] fix person dropdown
- [x] from person to team
- [x] from team to gardener
- [x] fix dropdown
- [x] from manual to tutorial
- [x] style person image
- [x] loop content on single
- [x] manual/tutorial on how to write and edit person
- [x] fix the markdown container (currently very narrow)
- [x] change team to gardener

## Organization template

- [ ] organization wiring
- [ ] organization template

## About 

- [ ] from about to root
- [ ] how many root pages we want?

## Glossary

- [ ] discuss what we want for glossary
- [ ] glossary vs context
- [ ] term + synonyms + deprecated (use this one instead and why)
- [ ] how to ensure glossary is being read, consulted?
- [ ] repackaging content?

## version control

Website is a snapshot of the latest update, but we do have the git commits in the open.

A way to integrate Hugo content with its older versions, maybe a timeline of updates (gitlab updates a json file on build) where user is pointed to the markdown file.

Or if we wanna get fancy, a comparison tool in pare showing what's added, removed by sho and when (we need to connect gardener with gitlab user for that).

This way volunteers can compare what changed since last time they checked, to stay in the loop. 

## publish for non techies

A content-only permission that allows authors to:
- add page (from template)
- edit page
- edit frontmatter criteria (required always on, optional on a menu)
- edit frontmatter values (limiting choices with autosuggest)

System presents user with URL of changed objects, on commit. 

## Tech Debt

- [ ] categories should point to .json, not category-description or nav-post
- [ ] why title? It should point to filename
- [ ] why category? It should point to folder
- [ ] reset select
- [x] emoji
- [ ] [mermaid diagrams](https://gohugo.io/content-management/diagrams/)
