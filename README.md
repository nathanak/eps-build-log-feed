# EPS Build Log — podcast feed

The public RSS feed for **EPS Build Log**, the build-in-public podcast from
[Every Possible Service](https://github.com/nathanak).

**Feed URL:** https://nathanak.github.io/eps-build-log-feed/feed.xml

## Why this repo exists

Episodes are produced and published through Muse, whose podcast feed omits
two channel fields Apple Podcasts requires (`itunes:author` and
`itunes:category`) and offers no way to set them. This repository hosts a
mirror of that feed — same episodes, same audio — with the complete field
set, served by GitHub Pages, so the show can be listed on Apple Podcasts
(and anywhere else) under our own control.

## Contents

- `feed.xml` — the feed itself. Channel: *EPS Build Log*, author
  *Every Possible Service*, category *Technology*.
- `cover.jpg` — show artwork, 1600×1600.
- `index.html` — a small landing page for the feed.

## Updating

When a new episode publishes to the Muse feed, add an `<item>` for it at the
top of `feed.xml` (newest first) with its title, description, publish date,
audio URL, byte length, and duration, and update `lastBuildDate`. Audio files
stay hosted on Muse's media URLs; this repo hosts only the feed and artwork.
