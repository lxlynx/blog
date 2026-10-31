<div align="center">

# blog

**Source for lxlynx.com — notes on developer tooling, growth engineering, and practical security for small teams.**

[![site](https://img.shields.io/badge/site-lxlynx.com-black?style=flat-square)](https://lxlynx.com)
[![jekyll](https://img.shields.io/badge/jekyll-github%20pages-cc0000?style=flat-square&logo=jekyll&logoColor=white)](#quick-start)

</div>

## About

A stock Jekyll site on GitHub Pages: no JavaScript build, no asset bundler,
no analytics. Writing a post is creating one Markdown file, and the site is
rebuilt by Pages on push. The constraint is the point — the only maintenance
that ever happens here is writing.

## Quick start

```bash
git clone https://github.com/lxlynx/blog
bundle exec jekyll serve   # or just push; Pages builds it
```

## Configuration

| Key | Description |
| --- | --- |
| `_posts/` | one Markdown file per post, dated filename |
| `_config.yml` | site metadata, permalink scheme, plugin list |
| `no build pipeline` | stock Jekyll on GitHub Pages — no bundler, no JS build step |
## Roadmap

- [ ] Index page by tag
- [ ] RSS/Atom link on every page
- [ ] Open Graph image per post

## Contributing

Issues and pull requests are welcome. Please keep changes small and focused,
and add a test for any behaviour change — every repository here ships with a
runnable test suite and no third-party dependencies, so CI is just
`python3 -m unittest` / `bash test_*.sh`.

## License

[MIT](LICENSE)
