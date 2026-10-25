# dilgrover.github.io

Dhiren Grover's link-in-bio site. Live at https://dilgrover.github.io (GitHub Pages, `main` branch, repo root). This URL is the link in his Instagram bio, so it must never change or break.

## Rules
- Plain static HTML/CSS. No build step, no frameworks, no Jekyll (`.nojekyll` is present).
- No Claude or claude.ai branding or links anywhere. Content made as a Claude artifact gets copied in as plain HTML, never embedded or linked.
- Keep the visual identity: background `#0a0710`, panel `#120c1b`, Avan pink `#ff3d9a` / `#ff8cc6`, fonts Inter Tight (display/body) and JetBrains Mono (labels), loaded from Google Fonts.
- Phone first: about 400px wide must work with no horizontal scroll.
- Affiliate links: if any are added, change the desk page footer ("No affiliate links") to a clear disclosure.

## Layout
- `index.html`: home page. Sections, top to bottom: header, **RESOURCES · FREE** (resource cards, newest first), FOLLOW · MAIN, TRAVEL, GAMING, MY PODCAST · SOCIAL UNTOLD, COMING SOON.
- `desk/index.html`: desk setup gear list (12 products).
- `downloads/`: files people can download (PDFs, images, route lists).
- `assets/`: images (`desk-banner.jpg`, `avan-orb.jpg` also used as favicon, `og.jpg` link preview).

## Adding a new resource (page or download)
1. Create a folder named after it, e.g. `swiss-route/index.html`. Copy `desk/index.html` as the template (keep the `← All links` back link, the head meta and the styles).
2. Put any downloadable file in `downloads/` with a descriptive lowercase name, e.g. `dilgrover-swiss-road-trip.pdf`.
3. In `index.html`, add an `<article class="res">` card at the **top** of the RESOURCES section, copying the existing desk card. Move the `NEW` chip to the new card and remove it from the older one. Use `Open …` for the page and `Download PDF ↓` (with the `download` attribute) for files. A card without a banner image is fine: just drop the `.rimg` link.
4. Check at phone width, then commit and push to `main`. The site updates in about 1–2 minutes.

## Adding or changing a social link
Copy an existing `<a class="btn">` in the relevant section of `index.html`, keeping the "Name / @handle · short description" pattern.

## Pending
- Confirm whether @travelseri is Instagram (currently linked as Instagram).
- When the `avan` repo goes public, replace the COMING SOON card with a real "Avan on GitHub" link.
