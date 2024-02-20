---
title: gardener
display: public
category: manual
description: How to write proper specs
date: 2023-06-30
---

> ⚠️ Site is hosted on gitlab, [ask to help](/about/help) if you don't have the permissions.

## Adding a gardener

1. Duplicate `content/gardener/template.md` file
2. Rename with name of gardener (slug: no spaces, no special characters)
3. Edit frontmatter
	- Title is same as filename
	- any description
	- change type to public (it will appear on [gardener](/gardener) list)
4. Write anything (in markdown) after `---` and it appears below the list


## Crediting a gardener

1. Open the post you want to credit user, and add gardener title on respective frontmatter (facilitator, author, helper)
2. Same for organizations, as contact or member
3. If gardener has a file, and it's public, it will appear both on gardener page and post it references on

## Adding image

1. Save image with same name of gardener title on `/static/images/gardener`
2. Open gardener post and add a new frontmatter criteria: `imageType: VALUE`
3. `VALUE` is the image type: png, jpg, gif...


