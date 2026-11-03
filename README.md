# Project Nightingale — OneCare Media strategic options (CreditSwan intelligence packet)

Prepared for Manulife | Comvest Credit Partners ahead of the 4 November 2026 call on carving out Sleep Media from Sleep Care.
Refreshed 3 November 2026. Confidential.

## Deploy to Vercel

This folder is a static site: one self-contained `index.html` (fonts load from Google Fonts), a `vercel.json`
that sets `noindex`/`no-store` headers, and the model outputs under `data/` for traceability.

    cd project-nightingale
    npx vercel --prod

Or add it to the existing `creditswan-brand` project: copy the folder's contents into that project's static root
(or into a sub-path such as `/nightingale/`) and push. Nothing needs building.

Because the packet is confidential, turn on Vercel Deployment Protection (password or Vercel Authentication) for the
deployment, or share only the preview URL with the Comvest team.

## Contents

- Tabs: 01 Overview · 02 About CreditSwan · 03 Situation · 04 Sleep Media · 05 Sleep Care · 06 Carve-out · 07 Options ·
  08 Recommendation · 09 Assumptions & method · 10 FAQ
- 155 exhibits (73 graphs, 82 tables), every one carrying a SOURCE · BASIS · ASSUMPTION line
- `data/model.json` — the options model outputs (harvest cases, option PVs, odds sensitivity, cash timing)
- `data/research.json` — the external research used (rates, BDC marks, comparables, precedents, legal routes)

## QA performed

Rendered in Chromium at 1440px and 390px, cream and ink themes: no console errors, no horizontal overflow,
csMotion.audit() reports no static exhibits, csLayout.report() places every assumptions block, and every
headline is one sentence of at most fifteen words with at most one number.
