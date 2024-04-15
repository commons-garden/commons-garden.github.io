---
title: spec
display: public
description: How to create or edit specs
date: 2023-06-03
---

<!-- # Writing a new spec

1. To publish a new spec, duplicate textarea as a file on `content/spec` folder.
2. File name decides URL, in the `commons.garden/spec/FILENAME` format. Don't change filename once published, otherwise it will break our permalink policy.
2. Site is hosted on gitlab, [ask to help](/about/help) if you don't have the permissions. -->

<!-- ## Required frontmatter

- `title:` The actual title of the spec
- `type:` `hidden` for never to be seen notes, `draft` in progress articles or `public`
- `category:` Use `spec`
- `status:` `draft`, `testing`, `stable`, `deprecated`, `archived`
- `scope:` The technologies that use it

## Optional frontmatter

- `description:` Article description
- `license:` pending: list possible licenses here, or link to where it exists
- `author:` Who wrote it. User needs to be on `member/` folder
- `reviewed:` Who reviewed this spec. User needs to be on `member/` folder
- `implemented:` Implemented by which organizations. Organization needs to be on `organization/` folder
- `date:` Use date of when spec entered latest status. Format is `YYYY-MM-DD`
- `link:` Link to spec
- `platform:` Platform where spec resides -->

## title 📌

appears in the path, must match the folder name

## status 📌

where this spec is in it's journey

## scope

the specs / technologies that are related

[choosing scope](/internal/scope) (or write your own)

## description

a description of the category type

## display 📌

boolean - should this be displayed on lists? will be rendered, but not linked to. true / false

[choosing display](/internal/display)

## license

[choosing license](/internal/license)

## author 📌

who wrote this spec

[choosing gardener](/gardener), [writing new gardener](/internal/gardener)

## reviewed

who reviewed this spec

[choosing gardener](/gardener), [writing new gardener](/internal/gardener) (or write your own)

## implemented

organizations that implemented this spec

[choosing organization](/organization), [writing new organization](/internal/organization) (or write your own)

## date 📌

When this document was first written. Format is `YYYY-MM-DD`

## link

link for the actual spec

## needs

the kind of help this spec needs to thrive
