---
on:
  workflow_dispatch:

permissions:
  contents: read
  issues: read
  pull-requests: read

tools:
  web-fetch:

safe-outputs:
  create-pull-request:
    title-prefix: "[Mona] "
    draft: false
    allowed-files:
      - site/**
---

# Keep Mona's GitHub Info website up to date

## Purpose

Review Mona's notes and recent official GitHub information, then propose relevant updates to Mona's GitHub Info website.

The goal is to keep the website accurate and current while making only changes that are supported by reliable sources.

## Sources to consult

1. Read the relevant files in the `notes/` directory to understand Mona's requirements and existing information.
2. Review recent posts and announcements from the official GitHub Blog:
   `https://github.blog/`
3. Review recent updates from the official GitHub Changelog:
   `https://github.blog/changelog/`

Use official GitHub sources as the authoritative sources for GitHub product and platform updates.

## Files you may modify

You may modify files only inside:

`site/`

Do not modify files in:

- `notes/`
- `.github/`
- `.devcontainer/`
- `.vscode/`
- the repository root
- any other directory outside `site/`

## Instructions

1. Read Mona's notes before making any changes.
2. Review recent information from the GitHub Blog.
3. Review recent information from the GitHub Changelog.
4. Identify GitHub updates that are relevant to the content of Mona's website.
5. Compare the relevant updates with the existing website content.
6. Make appropriate updates only when they are supported by the sources.
7. Preserve the existing website's structure, style, and organization.
8. Do not invent facts, announcements, features, dates, or other information.
9. Do not make unrelated changes.
10. If there are no meaningful updates, do not make unnecessary changes.

## Expected changes

Update the appropriate files under `site/` to reflect relevant, well-supported GitHub updates.

For every proposed update, make sure the pull request description clearly explains:

- What was changed.
- Which Mona note or website content motivated the change.
- Which GitHub Blog or Changelog source supports the change.
- Why the update is relevant to Mona's website.

## Pull request

Create a pull request containing the proposed website changes.

The pull request should include:

- A clear title describing the website update.
- A concise summary of the changes.
- The official GitHub Blog and/or Changelog sources used.
- A clear explanation of why the changes are relevant.

Leave the pull request open for human review. Do not merge it.