# CLAUDE.md

Guidance for working in this repository.

## What this repo is

This is the **`Tautellini/Tautellini`** special repository. Its name matches the owner's GitHub username, which makes its [README.md](README.md) render as a **Profile README** at the top of https://github.com/Tautellini — visible to anyone who visits the profile.

This is a public-facing personal landing page, not a software project.

## Implications for edits

- **Audience is humans browsing GitHub.** Every change to [README.md](README.md) is user-visible on the profile. Treat it with the care you'd give a personal homepage, not an internal doc.
- **GitHub Flavored Markdown only.** The page is rendered by GitHub's Markdown pipeline. Raw HTML is allowed but limited (GitHub sanitizes `<script>`, most inline styles, etc.). No JS, no external CSS.
- **Relative links resolve against this repo**, not the profile. For links into other repos or the profile itself, use absolute `https://github.com/...` URLs.
- **Images load over HTTPS** and should be hosted somewhere stable (this repo, another public repo, `user-images.githubusercontent.com`, shields.io, etc.). Avoid hotlinking from personal servers.
- **No build step.** The file is served as-is. Don't add tooling, package manifests, or CI unless the user explicitly asks.

## What typically goes in a Profile README

- Short intro / role
- What the user is currently working on or learning
- Tech stack badges (commonly via [shields.io](https://shields.io))
- Contact links (email, LinkedIn, personal site)
- GitHub stats cards (commonly via `github-readme-stats`)
- Pinned highlights or featured projects

The current [README.md](README.md) is the GitHub starter template with placeholder bullets commented out — it has not been personalized yet.

## Editing rules of thumb

- Preview rendered Markdown mentally before saving; GitHub does not warn on broken images or dead links.
- Don't add emojis unless the user asks (this overrides the friendly tone typical of profile READMEs).
- Keep the file short. Profile READMEs are skimmed, not read.
- Don't invent personal details (name, pronouns, employer, location, projects). Ask the user for any content you don't already have.
- Don't commit changes unless explicitly requested — see the root agent guidelines.

## Repo layout

```
.
├── README.md     ← the profile page; this is the only file that renders publicly
└── CLAUDE.md     ← this file (guidance for Claude; not rendered on the profile)
```

There is no source code, no tests, no dependencies.
