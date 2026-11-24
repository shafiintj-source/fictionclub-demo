# FICTION CLUB — isolated demo

This repository contains a development-only FICTION CLUB Kerala Pay and financial-products demo.

## Preview

The intended GitHub Pages URL is:

https://shafiintj-source.github.io/fictionclub-demo/

Enable **Settings → Pages → Build and deployment → GitHub Actions** if Pages is not already enabled. The workflow in `.github/workflows/pages.yml` deploys this repository only.

## Important limitations

- This is a demonstration, not a live payment or BBPS service.
- No real recharge, bill fetch, payment collection, mandate or AutoPay is active.
- All 87 GroMo links remain unverified in the supplied audit source; do not describe them as approved or commissionable.
- Firebase Authentication is not configured yet. `firebase-config.js` contains empty placeholders, so phone OTP, email/password and Google sign-in will not work until the isolated demo Firebase web-app configuration and provider/domain settings are supplied.
- This repository is separate from the production `fictionclub.in` website. Do not connect a production domain or production Firebase project to this demo.

## Pages

- `index.html` — demo home
- `recharge-mvp.html` — simulated Kerala Pay flow
- `login.html` — Firebase sign-in UI (configuration required)
- `credit-cards.html` — credit-card directory
- `gromo-links.html` — 87-link audit register
