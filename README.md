# f2i-com/.github

Organisation-level defaults for the [F2i](https://github.com/f2i-com) GitHub organisation.

GitHub treats a repository named `.github` specially. Files placed here apply across the organisation instead of to a single project. This repository currently holds one thing: the profile page that GitHub shows at the top of [github.com/f2i-com](https://github.com/f2i-com).

## What is here

| Path | Purpose |
| :-- | :-- |
| `profile/README.md` | The organisation profile. This is the page visitors see when they open the F2i organisation. It introduces the ecosystem, links each project and embeds screenshots pulled from the project repositories. |
| `README.md` | This file. It describes the repository itself, not the projects. |

## Editing the profile page

The profile page is plain GitHub-flavoured Markdown with a little inline HTML for the layout. Some rules keep it working:

- **Links and images must be absolute.** The page is rendered on the organisation landing page, not inside a project checkout, so relative paths such as `docs/README.md` resolve to nothing. Point at `https://github.com/f2i-com/<repo>/blob/main/...` for documents and `https://raw.githubusercontent.com/f2i-com/<repo>/main/...` for images.
- **Screenshots live with their projects.** The page embeds images that are committed in `formlogic.com`, `softn.com`, `zipp.org`, `oaiy.com` and `aokie.com`. Refresh a screenshot in its own repository and the profile picks it up without a change here. Each of those repositories documents how its screenshots were captured.
- **Keep project facts in sync with the project.** Taglines, licences and status badges on the profile mirror each repository's own README. When one of those changes, update the profile row to match.
- **Only public repositories can be linked or embedded.** A private repository's raw image URLs return 404 for visitors.

Changes to `profile/README.md` appear on the organisation page as soon as they land on `main`.

## Adding organisation-wide defaults

Other files GitHub recognises in this repository, none of which exist yet:

- `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `SECURITY.md` and `SUPPORT.md` act as the default community health files for any F2i repository that does not carry its own.
- `ISSUE_TEMPLATE/` and `PULL_REQUEST_TEMPLATE.md` supply default templates.
- `workflow-templates/` publishes starter GitHub Actions workflows to the organisation.
- `FUNDING.yml` sets a default sponsor button.

A file in a project repository always takes precedence over the same file here. FormLogic, SoftN, ZIPP, XDB, OAIY and Aokie each keep their own `SECURITY.md`, so security reports go to the project concerned.

## The projects

The profile page is the place to read about the ecosystem. The short version:

| Project | Repository |
| :-- | :-- |
| ZIPP, the execution engine | [f2i-com/zipp.org](https://github.com/f2i-com/zipp.org) |
| SoftN, the editable app language and runtime | [f2i-com/softn.com](https://github.com/f2i-com/softn.com) |
| FormLogic, the business platform | [f2i-com/formlogic.com](https://github.com/f2i-com/formlogic.com) |
| OAIY, the local AI workspace | [f2i-com/oaiy.com](https://github.com/f2i-com/oaiy.com) |
| Aokie, the local AI receptionist | [f2i-com/aokie.com](https://github.com/f2i-com/aokie.com) |
| XDB, the local-first database | [f2i-com/xdb.org](https://github.com/f2i-com/xdb.org) |

Website: [f2i.com](https://f2i.com/)
