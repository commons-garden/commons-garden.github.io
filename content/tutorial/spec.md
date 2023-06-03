---
title: spec
type: public
category: tutorial
description: How to write proper specs
date: 2023-06-03
---

1. To publish a new spec, duplicate `template.md` file on `content/spec` folder. 
2. File name decides URL, in the `commons.garden/spec/FILENAME` format. Don't change filename once published, otherwise it will break our permalink policy.
2. Site is hosted on gitlab, [ask to help](/about/help) if you don't have the permissions.

## Frontmatter criterias

| Criteria | Possible values | Req? |
| -- | -- |-- |
| `title` | The actual title of the spec | ✅ |
| `type` | `hidden` for never to be seen notes, `draft` in progress articles or `public` | ✅ |
| `category` | Use `spec` | ✅ |
| `description` | Article description | ❌ |
| `status` | pending: list possible statuses here | ❌ |
| `scope` | The technologies that use it| ❌ |
| `license` | pending: list possible licenses here, or link to where it exists| ❌ |
| `author` | Who wrote it. User needs to be on `members/` folder| ❌ |
| `reviewed` | Who reviewed this spec. User needs to be on `members/` folder| ❌ |
| `implemented` | Implemented by which organizations. Organization needs to be on `organization/` folder| ❌ |
| `date` | Use date of when spec entered latest status. Format is `YYYY-MM-DD`| ❌ |
| `link` | Link to spec| ❌ |
| `platform` | Platform where spec resides | ❌ |