# Publishing — how a post goes live

The whole flow is three steps, and the third one is one command.

## 1. Write the draft

A post is one Markdown file in `content/posts/`, named
`YYYY-MM-DD-slug.md`, starting with:

```yaml
---
title: "The title"
date: 2026-11-26
slug: the-title
draft: true
---
```

Every Basque page is bilingual: each sentence in English, then the same
sentence in Basque. The Basque is a draft translation until a native
speaker checks it — the post layout says so at the top.

Write it yourself, or ask Claude (on the PC, in the local repo clone) to
draft it from the English text. Drafts never appear on the site until
step 3 — that is the rule, so nothing goes live unreviewed.

## 2. Read it back

Open the file and read it. Check it sounds like you, the facts are right,
and there is nothing personal in it (no addresses, no private details
about where you live, no one else's private information).

## 3. Publish it

Tell Bobby "publish <the post>" — or run it yourself:

```sh
scripts/publish-post.sh content/posts/2026-11-26-my-article.md
```

That flips `draft: true` to `draft: false`, builds the site, commits, and
pushes. Cloudflare Pages rebuilds from the repo and the post is live at
`jonathanmccallum-eu.pages.dev/2026/11/26/<slug>/` in about a minute. If
the build fails, the script puts the draft flag back and stops — nothing
half-live.

## Rules that stay

- Drafts stay drafts until Jonathan says publish, one post at a time.
- The Carl Medearis post and the AI-topic post are deleted — never
  re-publish them.
- No AI as a post topic.
- Keep the site to one page: no header, no nav tabs, no newsletter form
  until the mailing list is decided.
