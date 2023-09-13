---
title: person
type: public
category: manual
description: How to write proper specs
date: 2023-06-30
---

> ⚠️ Site is hosted on gitlab, [ask to help](/about/help) if you don't have the permissions.

## Adding a person

1. Duplicate `content/person/template.md` file
2. Rename with name of person (slug: no spaces, no special characters)
3. Edit frontmatter
	- Title is same as filename
	- any description
	- change type to public (it will appear on [person](/person) list)
4. Write anything (in markdown) after `---` and it appears below the list


## Crediting a person

1. Open the post you want to credit user, and add person title on respective frontmatter (facilitator, author, helper)
2. Same for organizations, as contact or member
3. If person has a file, and it's public, it will appear both on person page and post it references on

## Adding image

1. Save image with same name of person title on `/static/images/person`
2. Open person post and add a new frontmatter criteria: `imageType: VALUE`
3. `VALUE` is the image type: png, jpg, gif...


