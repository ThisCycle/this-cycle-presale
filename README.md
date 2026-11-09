# This Cycle — pre-sale site

Standalone GitHub Pages landing page for **preorder.thiscycleco.com**.

## Status
- Responsive landing page, production countdown, and $49.99 retail price are implemented in `index.html`.
- Countdown ends at midnight Central Standard Time on November 30, 2026.
- Stripe checkout is **intentionally disabled** until identity verification, shipping terms, and payment link are ready.
- Product specification: **120 total pages, including instructional content**. Do not describe all 120 as writable pages.

## Photo setup
Upload these three image files to a folder named `assets` at the repository root:
- `assets/stacked-journals.webp` — transparent closed-journal stack (hero)
- `assets/open-journal.webp` — transparent open journal (interior)
- `assets/journals-table.webp` — real product scene on a wooden table

The page already references those paths. Until these are uploaded, the images will not display.

## Connecting Stripe later
In `index.html`, find `const checkoutUrl = '';` and insert the published **Stripe Payment Link** URL. Do not add a secret key. Verify shipping collection, shipping charges, shipping estimates, tax treatment, and refund disclosures before enabling sales.

## Hosting
GitHub Settings > Pages > Deploy from main / root. Configure custom domain `preorder.thiscycleco.com`; CNAME `preorder` pointing to `thiscycle.github.io` in DNS. Enable HTTPS after verification.
