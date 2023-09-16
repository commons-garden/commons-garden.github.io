---
title: About this site
type: public
description: Ways to help us
category: tutorial
date: 2023-03-07
---
This site uses [hugo](https://gohugo.io/) and is hosted on [gitlab](https://gitlab.com/commons-garden/commons-garden.gitlab.io).

All content lives under `/content` folder. All posts are markdown, with specific frontmatter criteria depending on category.

Folders are the categories. URLs appear as `commons.garden/FOLDER NAME/FILE NAME`

Take some time to learn different categories frontmatter: It's half of the (documentation) battle.

## Template

Hugo uses 3 templates, all under `/templates/_default/`:

- `index` for first page
- `list` for page collections
- `single` for the post itself

## automatic classes

This site automatically adds certain classes on `<HTML>`:

- the template name (index, list, single)
- the category name (spec, wireframe, etc)
- the page slug