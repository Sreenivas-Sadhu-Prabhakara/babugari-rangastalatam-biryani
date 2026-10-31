# Babugaari Rangastalam Biryani

A premium, independent, mobile-first restaurant website hosted on GitHub Pages. **No Swiggy dependency, no website framework, no build step, and no external runtime photo URLs.**

## Live site
https://sreenivas-sadhu-prabhakara.github.io/babugari-rangastalatam-biryani/

## Architecture
- `index.html`: complete self-contained page with semantic HTML, responsive CSS, minimal vanilla JavaScript, meta tags, and Restaurant JSON-LD.
- `assets/*.jpg`: food photography stored in the repo, served directly by GitHub Pages. Gallery and menu cards use these local paths.
- `assets/brand-fallback.svg`: branded fallback if any photograph fails to load.
- `favicon.svg`: custom monogram favicon.
- `.github/workflows/cache-food-images.yml`: one-time asset mirroring workflow; photo files are already checked in. It runs on workflow edits or manual dispatch. Avoid regenerating photo files unnecessarily.
- `robots.txt`, `sitemap.xml`: search-engine discovery.

## Features
- Cinematic split-screen hero, bespoke brand direction, announcement banner.
- Restaurant menu showcase with filterable categories: All, Dum, Fry & Ghee Roast, Coastal.
- Responsive food photo grid and keyboard-accessible photo lightbox.
- Accessible navigation and FAQ accordion; reduced-motion CSS; mobile sticky menu and directions CTA.
- Google Maps navigation; local-business structured data, canonical and OpenGraph tags.
- No ecommerce/order-processing backend and no tracking scripts. The site remains entirely static.

## Owner verification needed before final business launch
- Confirm the restaurant's exact spelling and logo.
- Confirm current postal address. Listings for the restaurant are inconsistent; this version uses 31, 12th Main Road, 3rd Block, Rajajinagar, and the owner-supplied landmark “opposite Asha Sweets”.
- Confirm phone, opening hours, and approved direct ordering contact; deliberately omitted instead of inventing.
- Confirm the six menu items and today's prices. Menu names came from public listing data and can change.
- Replace editorial illustrative food images with authentic restaurant food and premises photography. Photos are **not** represented as pictures of actual dishes or the restaurant.
- Owner approval of content, business registration / schema details, and local search setup.

## Image licensing and provenance
Current photos were independently downloaded from Unsplash under the Unsplash License and cached in `assets/`:
- `biryani-hero.jpg` and `biryani-chicken.jpg`: Mario Raj / Unsplash — https://unsplash.com/photos/a-white-bowl-filled-with-rice-and-meat-ysmeQt1dzcw
- `biryani-table.jpg`: Mario Raj / Unsplash — https://unsplash.com/photos/a-table-topped-with-bowls-of-food-and-sauces-vsnAIYA9bms
- `biryani-dark.jpg`: Steve Tsang / Unsplash — https://unsplash.com/photos/food-photography-of-bowl-of-chicken-biryani-OterGMpkdsM
- `biryani-celebration.jpg`: Prchi Palwe / Unsplash — https://unsplash.com/photos/cooked-food-on-white-ceramic-plate-3OMLWzkkt0Y

These are **illustrative** images and should not be labeled as actual BRB dishes. Do not use competitor restaurant-owned photos.

## Updating the site
Edit `index.html` on `main` to change text/menu sections or CSS. To replace an image, upload a file with the same filename under `assets/` (or update the `src` paths). Github Pages automatically redeploys main/root on commits.

## Launch QA
- All five `assets/biryani-*.jpg` images resolve and render.
- Responsive layout at ~360px, 768px, and 1440px.
- Mobile nav toggle, menu filters, gallery lightbox, and FAQs work by keyboard and pointer.
- No external ordering platform URLs; directions open Google Maps.
- Run an SEO, accessibility, and Core Web Vitals check after owner content is finalized.
