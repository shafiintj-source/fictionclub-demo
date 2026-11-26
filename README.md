# FICTION CLUB — isolated demo

A mobile-first Kerala digital-services and financial-products preview. This repository is separate from the production website.

## Preview
https://shafiintj-source.github.io/fictionclub-demo/

The GitHub Pages URL is a preview target, not proof that the current deployment is live. Latest deployment check (26 November 2026): build succeeded; GitHub Pages deployment failed with an HTTP 500 response. See the workflow history and the audit report before assuming the preview is available.

## Pages
- `index.html` — verified earning dashboard
- `earning-hub.html` — approved offers only; strict verification gate
- `credit-cards.html` — verified credit-card offers only
- `gromo-links.html` — finance/partner offer holding page
- `travel-tickets.html` — travel offers holding page until campaign approval
- `recharge-mvp.html` — simulated Kerala Pay flow
- `bill-payments.html` — official provider portals
- `login.html` — Firebase sign-in UI (configuration required)

## Affiliate verification status — 26 November 2026
- GroMo source catalogue: 87 records; 0 verified for public promotion.
- GroMo ticket #667691 was closed without the requested link-wise audit report.
- Cuelinks AbhiBus ticket #149111: reply acknowledged; review pending; no campaign approval.
- Admitad/Mitgo request #20722: received and under review; no publisher/campaign approval.
- vCommission ticket #160382: support asked for the publisher account's registered email ID; owner confirmation/reply pending.
- Travelpayouts saved links and earlier CJ advertiser relationships are not treated as verified earning links until current campaign terms and publisher tracking are checked.
- Generic partner newsletters and ticket acknowledgements are not account-specific campaign approval.

## Safety and payment status
- No live BBPS, bill fetch, recharge, payment collection, UPI mandate or AutoPay.
- Firebase config is intentionally blank in `firebase-config.js`; login needs a separate demo Firebase project and provider/domain setup.
- Demo pages are `noindex,nofollow`.
- Production `fictionclub.in`, production Firebase, AdSense and production integrations are separate and must remain unchanged.

See [EARNING-ONLY-STATUS.md](./EARNING-ONLY-STATUS.md) and [PARTNER-AUDIT-2026-11-26.md](./PARTNER-AUDIT-2026-11-26.md) for the audit trail.
