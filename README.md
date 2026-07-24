# Marketing Reactivation Impact — Mobile-First Site

A native, mobile-first responsive website built from the *Experience Abu Dhabi · Marketing Reactivation Impact* deck. Every slide has been **re-laid-out for the web** — content reflows into a single column on phones and expands into multi-column layouts on larger screens. No build step.

## Contents
- `index.html` — the whole site (HTML, CSS, JS inline)
- `media/` — campaign photos, videos, logos, and the desert background
- `README.md`

## What makes it mobile-first
- **Reflowed, not scaled.** Nothing is a shrunken slide. Each section is authored responsively — text, stats, tables, and timelines stack cleanly on a phone and spread out on tablet/desktop. Verified to have **zero horizontal overflow** at 390 / 768 / 1280 px.
- **Image-heavy slides become mosaics/carousels.** Digital, Offline, the China & USA case studies, and the airport section use a swipeable carousel on phones that becomes a mosaic grid on wider screens.
- **Animation on every element.** Scroll-reveal with stagger, animated bars, count-up on the big stats, parallax on the hero backgrounds, and autoplaying looping campaign videos (they pause when off-screen).
- **Proper navigation.** Sticky top bar with a **light/dark toggle** and a menu button; a full-screen menu (two-column, with its own close button) that jumps to any of the 16 sections; hairline separators between sections; and a scroll-progress bar.
- Respects `prefers-reduced-motion`.

## Notes on the assets
- The heavy campaign **GIFs were converted to compressed looping MP4** (same motion, ~15× smaller) so the whole `media/` folder is ~23 MB and loads fast.
- Country flags use system emoji (crisp at any size, no extra downloads); section icons are inline SVG. The real campaign **photos and videos** from the deck are used throughout the mosaics and case studies.

## Publish on GitHub Pages
1. Upload **`index.html` and the `media/` folder together** to a repo (keep them side by side).
2. **Settings → Pages → Deploy from a branch → main → / (root) → Save**.
3. Live in ~1 minute at `https://<username>.github.io/<repo>/`.

## Editing
Each section is a `<section id="…">` (cover, recap, timeline, digital, offline, metrics, funnel, domestic, global, sentiment, brand, spend, china, usa, next, close). Copy, numbers, and colours are plain HTML/CSS you can edit directly. Swap a photo/video by dropping a new file into `media/` under the same name.
