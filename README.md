# Project Nightingale — OneCare Media strategic options (CreditSwan intelligence packet)

Prepared for Manulife | Comvest Credit Partners ahead of the 4 November 2026 call on carving out Sleep Media from Sleep Care.
Refreshed 3 November 2026 (version 2, after the full-source pass). Confidential.

## Deploy to Vercel

This folder is a static site: one self-contained `index.html` (fonts load from Google Fonts), a `vercel.json`
that sets noindex / no-store / no-referrer / no-framing headers, and the model outputs under `data/` for traceability.

    cd project-nightingale
    npx vercel --prod

Or add it to the existing `creditswan-brand` project: copy the folder's contents into that project's static root
(or into a sub-path such as `/nightingale/`) and push. Nothing needs building.

The packet is confidential: turn on Vercel Deployment Protection (password or Vercel Authentication) for the
deployment, or share only the preview URL with the Comvest team.

## Contents

- Tabs: 01 Overview · 02 About CreditSwan · 03 Situation · 04 Sleep Media · 05 Sleep Care · 06 Carve-out · 07 Options ·
  08 Recommendation · 09 Assumptions & method · 10 FAQ
- 176 exhibits (81 graphs, 95 tables), every one carrying a SOURCE · BASIS · ASSUMPTION line
- `data/model.json` — the options model outputs (harvest cases, option PVs by state and odds, cash timing)
- `data/research.json` — the external research used (rates, BDC marks, comparables, precedents, legal routes)
- `data/gsc_extra.json` — the Search Console cuts (weekly, query, device, country, page) pulled 3 November 2026

## Sources covered in this version

All 29 project files and 3 project docs (board decks Q4-24 to Q3-26, SteerCo updates, SC commentaries, monthly
lender packages Jan-25 to May-26, the Q4-23 Comvest review, the tech-stack overview, the insurance decks), the
46 files in the SLEEP - ONE CARE folder (long-range plan, 19 October ask, 13-week cash, liquidity certificate,
dashboards, domain valuations and broker correspondence, Comvest internal notes), Google Search Console for both
properties through Markifact (GA4 and Google Ads connections hold no accounts for these properties), and the
published sources listed on the Assumptions tab.

## QA performed

Rendered in Chromium at 1440px and 390px, cream and ink themes: no console errors, no horizontal overflow,
csMotion.audit() reports no static exhibits, csLayout.report() places every assumptions block, and every
headline is one sentence of at most fifteen words with at most one number.
