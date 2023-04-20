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

Then the static website should be located at `public/`. You can deploy this directory to any static website server.

## How to add new content

```sh
hugo new content/<dir>/<file>.md
```

Then you can write your own content with Markdown syntax.

You may also set the default content template by adding `archetypes/default.md`. More details can be found in [archetypes](https://gohugo.io/content-management/archetypes/).

All avaliable front matter can be found in [front-matter](https://gohugo.io/content-management/front-matter/)

By default the navigation sorted by alphabetical order. If you want to make your own order, you can set in `data/menu/main.yaml` like:

```yaml
---
main:
  - name: Level 1
    ref: "/level-1"
    icon: "gdoc_notification"
    sub:
      - name: Level 1.1
        ref: "/level-1/level-1-1"
      - name: Level 1.2
        ref: "/level-1/level-1-2"
      - name: Level 1.3
        ref: "/level-1/level-1-3"
        sub:
          - name: Level 1.3.1
            ref: "/level-1/level-1-3/level-1-3-1"
  - name: Level 2
    ref: "/level-2"
    sub:
      - name: Level 2.1
        ref: "/level-2/level-2-1"
      - name: Level 2.2
        ref: "/level-2/level-2-2"
      - name: Level 2.2 Anchor
        ref: /level-2/level-2-2
        # Anchor to add to the entry. This example will result in `/level-2/level-2-2/#anchor`
        anchor: anchor
```

More details can be found in [menus](https://geekdocs.de/usage/menus/).

## Documents

- [gohugo document](https://gohugo.io/getting-started/)
- [hugo-geekdoc document](https://geekdocs.de/)
