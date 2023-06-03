---
title: spec
type: public
category: tutorial
date: 2023-06-03
---

To publish a new spec, duplicate `template.md` file on `content/spec` folder. 

File name decides URL, in the `commons.garden/spec/FILENAME` format. Don't change filename once published, otherwise it will break permalink policy.

Site is hosted on gitlab, [ask to help](/about/help) if you don't have the permissions.

## title

The actual title of the spec

## type

- `hidden`for never to be seen notes
- `draft` in progress articles
- `public` visible, published 

## abstract

Article description

## status

> pending: list possible statuses here

## scope

The technologies that use it

## license

> pending: list possible licenses here, or link to where it exists

## author

Who wrote it. 

> pending: user needs to be on `members/` folder

## reviewed

Who reviewed this spec

> pending: user needs to be on `members/` folder

## implemented

Implemented by which organizations

> pending: organization needs to be on `organization/` folder

## category

Use `spec`

## date

Use date of when spec entered latest status. Format is `YYYY-MM-DD`
## link

Link to spec

## platform

Platform where spec resides

> pending: generalize criterias used by other categories as partials