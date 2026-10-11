# oden-store — Oden Goods storefront (GitHub Pages)

Public landing pages for digital products. Hosted free on GitHub Pages.

## Products
- `index.html` — Calibration Trading Journal v0.1 ($12)

## Digital delivery
Buyers are redirected after Stripe payment to an unguessable download path
under `dl/`. The path token is NOT linked from any public page and is excluded
from sitemaps. (v1 control; upgrade to Stripe-backed expiring links later.)

## Deploy checklist when Stripe Payment Link arrives
1. `index.html`: replace `href="#"` on `#buy-btn` with the payment link
2. In Stripe Payment Link settings: after-payment redirect →
   `https://ofasgardoden.github.io/oden-store/dl/<TOKEN>/`
3. Commit + push — Pages deploys in ~1 min

## Rules
- Marketing claims must stay honest (show misses, refund promise) — trust doctrine.
- Internal ledgers/sales data stay in the agent workspace, never in this repo.
