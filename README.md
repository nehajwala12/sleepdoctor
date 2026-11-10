# Project Nightingale — Sleep Media value extraction (CreditSwan intelligence packet, v3.2)

Prepared for Manulife | Comvest Credit Partners. Refreshed 10 November 2026. Confidential.

Version 3.2 keeps the business view of 4 November 2026 and folds the separation assessment of 10 November 2026 into
the Separation tab, so one site carries the value case and the separation work together. All main-tab values are
business values before debt, discounted at 15% (12% and 20% shown). Senior-lender considerations stay in a short
appendix tab.

The separation assessment is a **first draft: further diligence required, not for reliance**. Every part of it
carries a first-draft strip, and its diligence list sits with it on the Separation tab.

## Deploy to Vercel

This folder is a static site: one self-contained `index.html` (fonts load from Google Fonts), a `vercel.json` that
sets noindex / no-store / no-referrer / no-framing headers, and the model and data extracts under `data/`.

    cd project-nightingale
    npx vercel --prod

Or drag the folder into a Vercel project (Framework preset: Other; no build command; output directory: the folder
itself), or copy its contents over the existing Nightingale deployment and push. Nothing needs building.

The packet is confidential: turn on Vercel Deployment Protection (password or Vercel Authentication) for the
deployment, or share only the preview URL with the Comvest team.

## Contents

- Tabs: 01 Overview · 02 Media · 03 Momentum · 04 Care · 05 Separation · 06 Value · 07 Plan · 08 Cash ·
  09 Appendix · 10 Assumptions & method · 11 FAQ · 12 About CreditSwan
- The menu is the contents rail (docked at 1180px and wider, a 48px bar with a drawer below), and About CreditSwan
  is the last tab. Tabs after the Overview therefore sit one number lower than in v3.1: Separation was 06 and is now
  05, and exhibit 7.04 in v3.1 is 6.04 here. Overview exhibits from 1.09 onward move down two places to make room
  for the two Separation exhibits.
- 05 Separation has eight parts, lettered in the rail:
  A Operating side (the v3.1 Separation tab, unchanged) · B Assessment summary · C Perimeter · D Technology ·
  E Funding · F People · G Data · H Diligence required (with confidence, method and sources). Parts B to H are the
  first-draft assessment. Each part opens with an "In this part" list that links to its sections.
- 283 exhibits (graphs and tables), every one carrying a SOURCE · BASIS · ASSUMPTION line; the Separation tab holds
  124 of them and three simulators (one-time cost against the AI saving, Sleep Care's outside funding, search
  revenue at risk from a cutover error)
- One assumptions register on the Assumptions tab: A-01 to A-43 as before, and A-44 to A-60 for the separation
  assessment. The draft's own stand-alone corporate cost assumption duplicated A-05 and A-10 and now points to them.
- The FAQ adds a Separation group (16 questions); the Overview adds a Separation section with two exhibits re-drawn
  from the tab
- `data/model3.json` — business valuation outputs: media scenarios, ten value levers, Sleep Care branches and gates,
  seven paths on two sets of odds, sensitivities, discount-rate view
- `data/gsc3.json` — Search Console extracts for both properties pulled 4 November 2026 (monthly, weekly, query, page)
- `data/lrp_media.json` — the long-range plan's media build (traffic, click-through, revenue per click, categories)
- `data/research3.json` — published sources used (AI visibility studies, AI licensing deals, Google's counting change,
  comparables, precedents)
- `data/cash_1030.json` — the 13-week cash forecast series (30 Oct and 2 Oct 2026) and monthly liquidity
- `data/separation.json` — the separation estimate, gates, headcount, revenue by domain, debt and registry dates
- `data/separation_series.json` — the time series behind the separation charts (search clicks, revenue per click,
  weekly cash, liquidity)

## QA performed

Rendered in Chromium at 1440, 1366, 1280, 1024 and 390px, cream and ink themes: no console errors, no horizontal
overflow, every exhibit drawn and revealed, csMotion.audit() reports no static exhibits and no wipes, and
csLayout.report() places all 33 assumptions blocks with none moved at load. At 1280, 1366 and 1440px the rail is docked and
stays on screen to the foot of the Separation tab, and each lettered part lands at the top when chosen; at 1024 and
390px the 48px bar is the only sticky row and the drawer opens and closes. Every in-packet link and deep link resolves, every assumption reference is in
the register, exhibits number in reading order, the simulators respond and open on the draft case, and reduced
motion and print show final states.
