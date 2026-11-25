# FICTION CLUB — isolated demo

A mobile-first Kerala digital-services and financial-products preview. This repository is separate from the production website.

## Preview
https://shafiintj-source.github.io/fictionclub-demo/

If the preview is not live yet, enable **Settings → Pages → Build and deployment → GitHub Actions**. The workflow in `.github/workflows/pages.yml` deploys this repository only. A repository URL is not proof that the Pages deployment is currently live.

## Pages
- `index.html` — verified earning dashboard
- `earning-hub.html` — approved offers only; strict verification gate
- `credit-cards.html` — verified credit-card offers only (source catalogue contains 39 entries)
- `gromo-links.html` — finance/partner offer holding page
- `travel-tickets.html` — travel offers holding page until campaign approval
- `recharge-mvp.html` — simulated Kerala Pay flow
- `bill-payments.html` — official provider portals
- `login.html` — Firebase sign-in UI (configuration required)

## Affiliate verification status — 25 November 2026
- GroMo source catalogue: 87 records; 0 verified for public promotion.
- All records remain held until active status, Kerala/India eligibility, commission, conversion event, tracking URL and FICTION CLUB promotion permission are confirmed.
- GroMo ticket #667691 was closed again without the requested link-wise audit report.
- Cuelinks AbhiBus ticket #149111: reply received/under review; no campaign approval yet.
- Admitad/Mitgo request #20722: received and under review; no publisher/campaign approval yet.
- vCommission: follow-up sent; no response recorded yet.
- Do not treat generic campaign newsletters, ticket acknowledgements or estimated commission examples as account-specific campaign approval.

## Safety and payment status
- No live BBPS, bill fetch, recharge, payment collection, UPI mandate or AutoPay.
- Firebase config is intentionally blank in `firebase-config.js`; login needs a separate demo Firebase project and provider/domain setup.
- Production `fictionclub.in`, production Firebase, AdSense and production integrations are separate and must remain unchanged.

See [EARNING-ONLY-STATUS.md](./EARNING-ONLY-STATUS.md) and [PARTNER-AUDIT-2026-11-25.md](./PARTNER-AUDIT-2026-11-25.md) for the audit trail.
