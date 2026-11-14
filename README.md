# proxylistchecker.org

Landing page for the ProxyVerity proxy checker widget. A static site: one HTML file,
one logo, no build step.

## Why no framework

The satellite plan calls for Astro, and that is right for webproxylist.org, which has
review and guide collections. This site is a single page with no content to collect, so
a build step would add a Node toolchain and a CI stage to produce a file that is already
written. If it ever grows past a handful of pages, moving it to Astro is the moment to
do that, not before.

## Its job, and how it differs from the other demo pages

Four pages now show this widget, and each has a different angle so they are four assets
rather than one copied four times:

| Page | Angle |
|---|---|
| proxyverity.github.io | the visual snippet builder |
| Cloudflare deployment | how the theming works |
| Netlify deployment | what the checking actually does |
| **here** | **the pitch to a webmaster: why put it up, what it costs, how to install** |

## Deploy

Cloudflare Pages, connected to this repository. No build command, output directory is
the repository root.

## Maintenance

The options table here is a short extract. The reference it must stay consistent with is
`projects/proxylib/doc/widget.md` in the monorepo — that file is the source the public
page, the showcase and this landing all derive from. When an option changes there, check
this table.
