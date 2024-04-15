---
title: About this site
display: public
description: How this site is made
date: 2023-03-07
---

This site uses [hugo](https://gohugo.io/) and is hosted on [gitlab](https://gitlab.com/commons-garden/commons-garden.gitlab.io).

All content lives under `/content` folder. All posts are markdown, with specific frontmatter criteria depending on category.

Folders are the categories. URLs appear as `commons.garden/CATEGORY NAME/FILE NAME`

Take some time to learn different categories frontmatter: It's half of the (documentation) battle.

## Template

Hugo uses 3 templates, all under `/templates/_default/`:

- [index](https://gitlab.com/commons-garden/v2/-/blob/main/layouts/_default/index.html?ref_type=heads) for first page
- [list](https://gitlab.com/commons-garden/v2/-/blob/main/layouts/_default/list.html?ref_type=heads) for page collections
- [single](https://gitlab.com/commons-garden/v2/-/blob/main/layouts/_default/singler.html?ref_type=heads) for the post itself

## Automatic classes

This site automatically adds certain classes on `<HTML>`:

- the template name (index, list, single)
- the category name (spec, wireframe, etc)
- the page slug
