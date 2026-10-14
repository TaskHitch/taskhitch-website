# taskhitch.com

The public marketing site for [TaskHitch](https://www.taskhitch.com), served by GitHub Pages from
the `main` branch of this repository.

## Why this is its own repository

It used to be published out of the private application repository, from a workflow that uploaded a
whole folder. That folder held 127 files — internal UI specs, a v1.3 roadmap, brand guidelines, and
retired assets — and all of them were publicly readable until 14 Oct 2026. The immediate fix was an
allowlist of the nine files the page actually needs; the structural fix is this repository.

The point is that nothing private is *here to leak*. A mistake in a path, a workflow or a Pages
setting can only ever expose the marketing site, because the marketing site is all there is.

## What is here

```
index.html                    the page
TaskHitch-logo-{accent,dark}.svg
TaskHitch-wordmark-{accent,dark}.svg
screenshots/                  four product screenshots the page embeds
```

Nine files, and that is the entire public surface. The page also loads two Google Fonts families
from `fonts.googleapis.com`; everything else is local.

## Editing it

This repository is the source of truth for the published site. Push to `main` and Pages redeploys.

The *design sources* — brand guidelines, the master SVGs, archived marks, UI specs — stay in the
private repository under `brand/`. So the logo files here are published copies: if a mark is
redesigned there, copy the new file here deliberately. That duplication is the price of the
separation, and it is the right way round — a stale logo is a cosmetic problem, where a leaked
roadmap is not.
