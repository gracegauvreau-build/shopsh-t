# Shop Sh*t 🛍️

A private, personal buy-planner. Save links to things you're eyeing while you browse, organize them by category and *when you need them by*, and decide later — instead of cluttering your public storefront.

Built as a companion to ShopMy: most saves stay private, but the ones you actually love and buy can be **promoted to your public storefront** in two taps.

## Why

ShopMy is for outward-facing curation. This is the private inbox that feeds it — a fast capture spot for everything you're shopping for in the moment, with two things a storefront doesn't track: a **need-by date** and a **buy intent** (just want it / planning / need soon).

## Screens

- **Home** — your saved items, filterable by category, with bought / pass / promote actions
- **Plan** — a timeline and month-calendar view that lays your buys out by when you need them
- **Insights** — your real conversion rate: of everything you saved, how much you actually bought, what you saved by passing, and follow-through by category
- **Profile** — ShopMy connection, monthly budget cap, default collections

## Run it

It's a single file with no build step. Either:

- Open `index.html` directly in a browser, or
- Serve it: `python3 -m http.server` then visit `http://localhost:8000`

To publish on GitHub Pages: push to a repo, then enable Pages on the `main` branch (root). Your app will be live at `https://<username>.github.io/<repo>/`.

## Notes

- All data is in-memory demo data (in the `items` array near the top of the script). It resets on refresh — wiring up real storage is the natural next step.
- No dependencies bundled; icons load from the Tabler CDN and the font from Google Fonts.

## Next steps

- Persist data (localStorage for a quick win, or a backend for multi-device sync)
- A browser extension / iOS share-sheet target for one-tap capture while browsing
- Real ShopMy API integration behind the promote flow
- Budget enforcement that warns when due-soon items exceed your monthly cap
