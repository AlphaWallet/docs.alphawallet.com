# Alphawallet Docs

This project was built by [gohugo](https://gohugo.io/) with [hugo-geekdoc](https://themes.gohugo.io/themes/hugo-geekdoc/) theme.

## How to use

First you should install [gohugo](https://gohugo.io/installation/) locally.

Run locally:

```sh
hugo serve
```

Then you can open http://localhost:1313/ to watch locally.

Production build:

```sh
hugo --minify
```

Then the static website should located at `public/`. You can deploy this directory to any static website server.

## How to add new content

```sh
hugo new content/<dir>/<file>.md
```

Then you can write your own content with Markdown syntax.

## Documents

- [gohugo document](https://gohugo.io/getting-started/)
- [hugo-geekdoc document](https://geekdocs.de/)
