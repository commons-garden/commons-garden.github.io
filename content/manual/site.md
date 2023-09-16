---
title: How to help
type: public
description: Ways to help us
category: manual
date: 2023-03-07
---
This site uses hugo and is hosted on gitlab.

All content lives under `/content` folder. All posts are markdown, with specific frontmatter criteria depending on category.

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