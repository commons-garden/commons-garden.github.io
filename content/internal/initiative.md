---
title: initiative
display: public
description: How to write proper specs
date: 2023-06-30
---

## Writing a new initiative

1. To publish a new initiative, duplicate `template.md` file on `content/initative` folder.
2. File name decides URL, in the `commons.garden/initiative/FILENAME` format. Don't change filename once published, otherwise it will break our permalink policy (more on redirect later).
3. Site is hosted on gitlab, [ask to help](/about/help) if you don't have the permissions.

## Required frontmatter

- `title:` The actual title of the spec
- `date:` Use date of when spec entered latest status. Format is `YYYY-MM-DD`
- `type:` `hidden` for never to be seen notes, `draft` in progress articles or `public`
- `category:` Use `initiative`
- `status:` `draft`, `testing`, `stable`, `deprecated`, `archived`
- `scope:` The technologies that use it

## Optional frontmatter

- `description:` Article description
- `author:` Who wrote it. User needs to be on `member/` folder
