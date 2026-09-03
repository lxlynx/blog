# blog

Source for [lxlynx.com](https://lxlynx.com): notes on developer tooling, growth
engineering, and practical security for small teams.

It is a stock Jekyll site on GitHub Pages. No JavaScript build, no bundler pipeline for
assets, no analytics. Writing a post means adding one Markdown file and pushing, which
is the entire reason it still gets updated.

## Layout

```
_config.yml                     site metadata, theme, plugins
index.md                        home page, lists posts via the minima home layout
_posts/YYYY-MM-DD-title.md      one file per post
Gemfile                         pins the same gems GitHub Pages builds with
```

## Running it locally

```bash
bundle install
bundle exec jekyll serve --livereload
# http://127.0.0.1:4000
```

Drafts go in a `_drafts/` directory without the date prefix, and show up with
`jekyll serve --drafts`.

## Adding a post

Create `_posts/2026-07-22-some-title.md` with front matter:

```yaml
---
layout: post
title: "Some Title"
date: 2026-07-22 09:10:00 +0800
categories: tools
---
```

Filename date and front matter date should agree. Jekyll uses the filename for the URL
and the front matter for sorting, and disagreement between them produces posts that
appear to travel in time.

## Deploying

Push to `main`. GitHub Pages builds it. If a build fails, the reason is nearly always a
plugin that is not on the Pages allowlist, or a stray tab in `_config.yml`.

## Licence

Site code is MIT (see [LICENSE](LICENSE)). Post text is not: please link rather than
repost in full.
