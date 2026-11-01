# STATUS

## What was built

A beginner manual and static HTML author site for writers who want to use GitHub, created for Dylan Asdale / Asdale Dynamics, LLC (Indiana, formed October 2026). No code required; plain English, step by step.

### Files created

**Root**
- `README.md` — project overview, credits Asdale Dynamics, LLC, links to the four manual steps
- `LICENSE` — MIT License, copyright line exactly `Copyright (c) 2026 Asdale Dynamics, LLC`

**docs/** (Markdown manual)
- `00-welcome.md` — introduction: what GitHub does for writers, no-code, no secrets
- `01-getting-started.md` — create a GitHub account, create a repository, upload a manuscript file, what a commit is
- `02-version-control.md` — edit files on GitHub, upload revised files, view history, restore earlier versions, good commit messages
- `03-collaborating-with-editors.md` — invite an editor, permission levels, line comments, review changes, remove an editor, no secrets
- `04-publishing-an-author-site.md` — create a `username.github.io` repository, add `index.html`, turn on GitHub Pages, add more pages, what not to post

**site/** (static HTML author site, publishable via GitHub Pages)
- `site/index.html` — author homepage: about, books, beginner manual link, contact
- `site/manual.html` — HTML rendering of the full beginner manual

## How to run it

This is a static site. No build step, no install, no server required.

- Read the manual: open any file in `docs/` in a text editor, or view `site/manual.html` in a browser.
- Preview the author site: open `site/index.html` in a browser.
- To publish the author site for free: create a GitHub repository named `yourusername.github.io` (Public), copy `site/index.html` (and `site/manual.html`) into it, enable GitHub Pages in Settings > Pages using the `main` branch. The site goes live at `https://yourusername.github.io/`.

## Verification results

- HTML validation: `site/index.html` OK, `site/manual.html` OK (well-formed, all tags closed)
- `LICENSE`: copyright line `Copyright (c) 2026 Asdale Dynamics, LLC` present and exact
- `README.md`: credits Asdale Dynamics, LLC
- Secrets/personal-data scan: no API keys, tokens, passwords, or personal data in any file. Matches for "api key", "secret", "password" are educational warnings only (e.g., "Never put passwords, API keys..."), not actual credentials.
- No `.github/workflows` files present.
- No remote repos created, nothing pushed.

## Known gaps

- The manual is web/GitHub UI-focused; it does not cover installing Git locally or using the command line (deliberate, since the audience is "no code required").
- No automated test suite or CI configuration (no `.github/workflows` by design); verification is manual file inspection and HTML validation.
- The HTML site is a single-author template; multi-author or themed variants are not included.
- `site/manual.html` is a static snapshot of the Markdown manual; if the Markdown docs are edited, the HTML must be updated by hand.
