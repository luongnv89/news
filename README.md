# The AI Gazette

A sourced AI-news newspaper covering models, coding and agents, research, and industry and policy.

- Website: https://luongnv.com/news/
- Editions begin research at 06:00 and 16:00 Europe/Paris; delivery and publication follow verification.
- Full-width vintage newspaper layout, responsive from phone to desktop.
- Each edition separates publication dates, source-check times, reported facts, vendor claims, editorial analysis and caveats.
- An archive preserves prior editions, with standalone HTML, PDF, Markdown and public JSON downloads.
- Empty editions explicitly report no material verified developments rather than repeat or invent news.

## GitHub Trending

- Daily newspaper: https://luongnv.com/news/trending/
- Archive: https://luongnv.com/news/trending/archive.html
- Research starts at 08:00 Europe/Paris, followed by verified publication and delivery.
- Up to eight editorial picks from GitHub's actual all-language daily Trending listing, with repository/README verification, practical reasons to investigate, and concrete caveats.
- Covers AI/agents, developer tools, security and other standout projects. Curation order is separate from the observed GitHub rank; displayed daily stars are separate from API total stars.
- Unchanged picks are not recycled within seven days. Popularity is not an endorsement, security audit or claim that a project is newly released.
- Dated HTML, Markdown and public JSON remain in `trending/reports/`. No candidate projects or installers are executed to prepare the digest.

The Trending roundup uses GitHub's primary listing and repository sources directly; it is distinct from the AI newspaper's last30days research.

## Publication

This repository holds only the reviewed public website. Research uses Matt Van Horn's last30days skill, with primary-source verification. Generation runs on the owner's machine; GitHub Actions deploys the committed static files, without research credentials.

Publishing uses `github-pages-publish` from https://github.com/luongnv89/skills, installed through ASM. Deployment is considered complete only when the action succeeds for the exact commit and the live files match that commit.

Raw research caches, local runbooks, private logs, browser sessions, credentials and local filesystem pointers are excluded. Coverage gaps remain visible in the public newspaper. No applications or job-candidate information are part of this repository.

## Files

- `index.html`: latest edition.
- `archive.html`: date/edition archive.
- `reports/`: historical HTML, PDF, Markdown and public JSON.
- `.github/pages-publish.json`: managed publication manifest.
- `.github/workflows/pages.yml`: managed Pages deployment.

The initial edition is a dated catch-up, not a claim that every headline happened on the day it was issued. The journal is a bounded editorial digest, not an exhaustive AI-news feed.
