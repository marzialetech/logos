# Logos

Logo and pixel-reveal assets for Marziale Technologies.

- **pixel-reveal.html** – Animated pixel reveal (logo, angel, man on boat). Build with `node build-pixel-reveal.js`.
- **index.html** – Redirects to pixel-reveal (for serving at e.g. marziale.tech/logos/).

## Build

```bash
node build-pixel-reveal.js
```

Inlines the pixelated SVGs into `pixel-reveal.html` so the page works when opened directly or served statically.

## Assets

- **martechtext** – Marziale Technologies text (pixelated).
- **logo** – Logo mark (pixelated).
- **angel-silhouette**, **two-figures** (man on boat) – Figure SVGs.
- **cursor** – Potrace-traced hand cursor (white, for use on blue).

Pipeline: PNG → (ImageMagick → PBM) → potrace → SVG; pixelation via `pixels-to-svg.js` and ImageMagick `txt:-`.
