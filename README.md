# FICTION CLUB — isolated demo

A mobile-first Kerala digital-services and financial-products preview. The UI uses a near-black app-style theme with compact navigation and icon tiles.

## Preview
https://shafiintj-source.github.io/fictionclub-demo/

If the preview is not live yet, enable **Settings → Pages → Build and deployment → GitHub Actions**. The workflow in `.github/workflows/pages.yml` deploys this repository only.

## Pages
- `index.html` — compact dashboard
- `recharge-mvp.html` — simulated Kerala Pay flow
- `bill-payments.html` — official provider portals
- `credit-cards.html` — 38-card directory
- `gromo-links.html` — 87-link audit register
- `login.html` — Firebase sign-in UI (configuration required)

## Important status
- No live BBPS, bill fetch, recharge, payment collection, UPI mandate or AutoPay.
- All 87 GroMo rows in the supplied source are marked Verified = No; approval and commission are not confirmed.
- Firebase config is intentionally blank in `firebase-config.js`; login needs a separate demo Firebase project and provider/domain setup.
- Production `fictionclub.in`, production Firebase and AdSense are separate and must remain unchanged.

See [PROJECT-CONTEXT.md](./PROJECT-CONTEXT.md) for the organized product scope, source facts, file map and backlog.
