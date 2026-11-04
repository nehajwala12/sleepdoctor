# Project Nightingale — Sleep Media value extraction (CreditSwan intelligence packet, v3)

Prepared for Manulife | Comvest Credit Partners ahead of the 4 November 2026 call on carving out Sleep Media from
Sleep Care and capturing its cash. Refreshed 4 November 2026. Confidential.

Version 3 is the business view: what Sleep Media and Sleep Care are worth, how the value is extracted, and what the
board decides in the next ninety days. All main-tab values are business values before debt, discounted at 15%
(12% and 20% shown). Senior-lender considerations (the debt stack, management's request and a counter, lender
recoveries, governance and enforcement routes) are kept to a short appendix tab.

## Deploy to Vercel

This folder is a static site: one self-contained `index.html` (fonts load from Google Fonts), a `vercel.json` that
sets noindex / no-store / no-referrer / no-framing headers, and the model and data extracts under `data/`.

    cd project-nightingale
    npx vercel --prod

Or copy the folder's contents into the existing `creditswan-brand` project's static root (or a sub-path such as
`/nightingale/`) and push. Nothing needs building.

The packet is confidential: turn on Vercel Deployment Protection (password or Vercel Authentication) for the
deployment, or share only the preview URL with the Comvest team.

## Contents

- Tabs: 01 Overview · 02 About CreditSwan · 03 Media · 04 Momentum · 05 Care · 06 Separation · 07 Value · 08 Plan ·
  09 Appendix (lender and capital matters) · 10 Assumptions & method · 11 FAQ
- 164 exhibits (77 graphs, 87 tables), each with a SOURCE · BASIS · ASSUMPTION line; 41 assumptions in the register
- Tab 04 Momentum is new: a balanced read of this year's Google rank, AI visibility and monetisation gains against
  the continuing traffic decline, with the October read for the holiday quarter
- The appendix is deliberately short (3 graphs, 5 tables), below the nine-and-nine standard of the analytical tabs
- `data/model3.json` — business valuation outputs: media scenarios, ten value levers, Sleep Care branches and gates,
  seven paths on two sets of odds, sensitivities, discount-rate view
- `data/gsc3.json` — Search Console extracts for both properties pulled 4 November 2026 (monthly, weekly, query, page)
- `data/lrp_media.json` — the long-range plan's media build (traffic, click-through, revenue per click, categories)
- `data/research3.json` — published sources used (AI visibility studies, AI licensing deals, Google's counting change,
  comparables, precedents)

## QA performed

Rendered in Chromium at 1440px and 390px, cream and ink themes: no console errors, no horizontal overflow,
csMotion.audit() reports no static exhibits, csLayout.report() places every assumptions block, exhibits number in
reading order, and every headline is one sentence of at most fifteen words with at most one number.
