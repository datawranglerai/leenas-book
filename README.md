# Leena Keshishian — Portfolio

A single-page portfolio for conceptual copywriter Leena Keshishian. The site
wraps a published Google Slides presentation in a responsive, full-window
viewer and is hosted with GitHub Pages.

**Live site:** <https://leenasbook.fyi/>

## Project structure

- `index.html` — page metadata, presentation embed, and layout
- `favicon.png` — browser icon
- `social-preview.png` — image used by social link previews
- `LICENSE` — proprietary, all-rights-reserved notice

There is no build step and there are no package dependencies.

## Preview locally

From the repository root, run:

```sh
python3 -m http.server 4173
```

Then open <http://localhost:4173/>.

## Update the presentation

Changes made to the existing published Google Slides deck should appear in the
embed automatically. If the deck is republished under a new URL, replace the
iframe `src` in `index.html`. Keep embedded videos set to manual playback so
that they do not intercept slide-navigation clicks while loading.

## Deployment

GitHub Pages publishes the site directly from this repository's `main` branch.
Push changes to `main` and allow GitHub Pages a few minutes to deploy them.

## Search visibility

The page includes `noindex, nofollow` in its robots metadata so compliant search
engines, including Google, are instructed not to index it. Do not block the page
in `robots.txt`: crawlers must be able to load the page to read the `noindex`
instruction. This is not access control; anyone with the URL can still view and
share the site.

## Copyright

Copyright © 2026 Leena Keshishian. All rights reserved. See [LICENSE](LICENSE).
