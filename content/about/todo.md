---
title: TODO
type: public
status: ongoing
description: Our next steps
category: about
author: [nonlinear]
date: 2023-09-10
---

## Show-and-tell

- [ ] event category
- [ ] past/upcoming
- [ ] podcast?
- [ ] .ics (how to automate)
- [ ] show time in local area
- [ ] social media
	- [ ] mastodon
	- [ ] youtube?

## Content

- [ ] document p2p-delete 📌
- [ ] update initiatives Michael wants to facilitate, define needs and next steps
- [ ] "needs" tags (resources, skillset, etc)
- [ ] "type" tags (language, wireframe)
- [ ] 2 emoji per initiative/spec
- [ ] list volunteer types
- [ ] redirect policy, template: `p2p-delete` becomes `p2p_delete`

## Hugo

- [ ] mapping category diagram into hugo [category/criteria diagram](https://hackmd.io/@mixmix/rywE-3P1T/edit)
- [ ] merge wireframe into spec + type
- [ ] subpages
	- [ ] page template checkjs if slug has a folder and:
		- lists all public pages in alphabetical order, into a table of content
		- folder pages point to original page
	- [ ] subgroups should not be listed on list.html (or should? we need at least a new template)

## Training gardeners

- [ ] tutorials
- [ ] statuses
- [ ] definition of proper training
- [ ] who can educate others? how to prevent bottleneck?

## Admin

- [ ] legal fiction, NGO
- [ ] review [open collective](https://opencollective.com/commons-garden)



## Internal documentation

How we write and update documentation for our facilitators?

- [ ] list inventory of initial tutorials we need
- [ ] maybe as we pass on knowledge, we write our manuals
- [ ] checklists. CHECKLISTS!
- [ ] adding categories tutorial: css, nav, json, etc
- [ ] template inside tutorial (loop from yml file)

## Design

- [ ] redesign on figma
- [ ] categories have colors:
	- organization: blue
	- person: yellow
	- spec: pink
	- initiative: green
	- about: grey
- [ ] design open graph image
- [ ] slide design:
	- title
	- history
	- description
	- pages (how to separate?)
	- frontmatter badges
	- needs (with actionables)
	- credits (people)
- [ ] design favicons
- [ ] phase out dropdown menu for accordion + list
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

- [ ] review [hugo aliases](https://gohugo.io/content-management/urls/#aliases)
- [ ] review `/template` layout, scale it
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
