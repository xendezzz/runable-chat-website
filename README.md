# Runable Chat Website

A responsive static landing-page prototype for Runable multimodal chat, built with HTML, CSS and JavaScript. All runtime assets are included locally; no package installation or build step is required.

## Run locally

From this repository:

```sh
python3 -m http.server 4173 --bind 127.0.0.1 --directory dist
```

Open http://127.0.0.1:4173. For static hosting, use `dist/` as the publish directory.

## Features

- Animated hero cycling through coffee-shop creation, trip planning, research and playlist conversations; starts after the CTA entrance.
- Moving clouds with a subtle 2px dither treatment, italic hero heading and rotating AI provider icons.
- Independent hero input and scroll-driven three-step product demonstration: typing, voice, attachments, research, website publishing and report exports.
- Five feature cards with pastel ancient Greece backgrounds and minimal 2D UI. Cards rest on their final frames and replay individually on hover, keyboard focus or touch.
- Weighted desktop scrolling matching the Runable website-builder prototype; native scrolling on touch, narrow viewports and reduced-motion settings.
- Staggered blur entrances, responsive layout, pricing before FAQs, closing CTA and footer.
- Pricing toggle and disclosures based on a snapshot of the existing Runable multimodal-chat page.

## Demo scope

Chat, voice, research and publishing interactions are scripted previews. They do not call AI services, record audio or publish websites. Report downloads provide sample Markdown, HTML and plain-text files; PDF opens a printable report. Pricing is a static snapshot, not a live API. External CTA links lead to Runable.

## Main files

- `dist/index.html`: page structure and content.
- `dist/exact-hero.js` / `.css`: hero layout and conversations.
- `dist/app.js` and `story-minimal.css`: scroll-driven product demo.
- `dist/feature-demos.js` / `.css`: independently replayable feature demos.
- `dist/features-pricing.js` / `.css`: cards and pricing.
- `dist/page-reveals.js` / `.css`: section entrances.
- `dist/weighted-scroll.js`: desktop scroll smoothing.
- `dist/assets/`: fonts, icons and imagery.

Image-generation prompts and asset references are documented in the accompanying `*-prompts.md` files. The ancient Greece set is documented in `greece-background-prompts.md`.

## References

- Existing product page: https://runable.com/multimodal-chat
- Related website prototype: https://github.com/xendezzz/runable-websites-hero-prototype

Design and brand assets belong to their respective owners. No additional license is granted by this repository.
