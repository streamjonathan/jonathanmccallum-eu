# AGENTS.md — jonathanmccallum-eu (Basque mirror of jonathanmccallum.com)

Basque mirror site. Same theme and design as the main site (Paper Light).
Every page is bilingual: each sentence in English, then the same sentence
in Basque. Repo: streamjonathan/jonathanmccallum-eu. Proof:
jonathanmccallum-eu.pages.dev. Priority: English first, Basque second,
Japanese third.

## Mission

Mirror jonathanmccallum.com in Basque — every article in English and
Basque, in Jonathan's voice: plain short sentences, friendly, positive,
never preachy. An average person interested in Jesus, not an expert or
theologian.

## Roles

- **Bobby (Muse) is the lead builder.** He coordinates, builds, pushes to GitHub
  and deploys to Cloudflare. He is the ONLY one who pushes or deploys.
- **Claude advises and reviews** translation quality. He does not push or deploy.
- **Helper Muses translate** one article at a time, drafts only.

## The one rule above all

**Never publish or alter live production assets without Jonathan's clear
permission.** The Basque site goes live only when he says so, after reading
the pilot article(s). Drafts stay drafts until he approves them. Work on a
branch, never straight on main. Give Bobby a preview URL.

## Bilingual rules

- English repo (streamjonathan.github.io) is the source of truth. Articles
  are built from the English Markdown, keeping the same date, slug,
  source_video and shareImage. Only the title and body are translated.
- **Every page is bilingual: each sentence in English, then the same
  sentence in Basque.** The English line comes first, the Basque line
  second. No English-only or Basque-only article pages.
- The Basque translation is an agent draft, unreviewed by a native speaker
  — the post layout says so at the top of every article, and a native
  speaker check is owed before any page is called finished.
- Voice: plain and warm, short sentences. No emojis, no newsletter form,
  no links the English article does not have.
- Never invent facts, dates, links or details. Song lyrics are quoted in
  the language Jonathan sings them in — never invent a Basque translation
  of lyrics.

## Site facts

- Eleventy 3, Cloudflare Pages, Paper Light theme (Fraunces + Newsreader).
- No Ask chat and no note Worker on this site — search (Pagefind) works.
  The Ask panel markup and ask.js are removed.
- No Bible section yet. No Mind Poems page yet.
- CSS is preloaded, not inlined (CSP blocks inline style). Bump the `?v=` query
  on any CSS/JS file you change.

## Blocker

The Cloudflare account is at its 20-project cap, so no Pages project
exists for this repo yet. The repo and branch are ready; the project needs
a free slot (or second-account access) before a preview URL can exist.
Do not pay for anything.
