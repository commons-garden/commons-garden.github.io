---
title: spec
display: public
description: How to write proper specs
date: 2023-06-03
---

1. To publish a new spec, duplicate `template.md` file on `content/spec` folder.
2. File name decides URL, in the `commons.garden/spec/FILENAME` format. Don't change filename once published, otherwise it will break our permalink policy.
3. Site is hosted on gitlab, [ask to help](/about/help) if you don't have the permissions.

## Frontmatter criterias

| Criteria      | Possible values                                                                        | Req?     |
| ------------- | -------------------------------------------------------------------------------------- | -------- |
| `title`       | The actual title of the spec                                                           | Required |
| `type`        | `hidden` for never to be seen notes, `draft` in progress articles or `public`          | Required |
| `category`    | Use `spec`                                                                             | Required |
| `description` | Article description                                                                    | Optional |
| `status`      | `draft`, `testing`, `stable`, `deprecated`, `archived`                                 | Required |
| `scope`       | The technologies that use it                                                           | Required |
| `license`     | pending: list possible licenses here, or link to where it exists                       | Optional |
| `author`      | Who wrote it. User needs to be on `member/` folder                                     | Optional |
| `reviewed`    | Who reviewed this spec. User needs to be on `member/` folder                           | Optional |
| `implemented` | Implemented by which organizations. Organization needs to be on `organization/` folder | Optional |
| `date`        | Use date of when spec entered latest status. Format is `YYYY-MM-DD`                    | Optional |
| `link`        | Link to spec                                                                           | Optional |
| `platform`    | Platform where spec resides                                                            | Optional |
