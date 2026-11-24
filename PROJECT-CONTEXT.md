# FICTION CLUB — project context and working plan

## Product identity
- Project: FICTION CLUB (sole proprietorship; Udyam/MSME registration has been discussed).
- Primary web property: fictionclub.in. This repository is a separate, private-development preview and must not change the production website.
- Demo product direction: Kerala-first everyday digital services hub with a compact, mobile-first interface.
- UI direction: near-black / charcoal theme, lime accent, compact copy, app-icon style service tiles, minimal navigation, responsive mobile layout.

## Demo information architecture
1. Home dashboard: short intro, quick actions, payment shortcuts, finance product shortcuts, transparent project status.
2. Pay & recharge: simulated recharge / bill flow. No live payment or BBPS claim.
3. Official bill portals: external official provider links only.
4. Credit cards: 38 directory entries with search / comparison / shortlist UI.
5. Partner register: 87 supplied GroMo source links across savings, cards, personal loans, business loans, demat/investing and other services.
6. Login: phone OTP, email/password and Google sign-in UI backed by Firebase Auth code.

## Verified source facts / safety labels
- The supplied GroMo audit data marks 87/87 links as Verified = No. Do not present these as approved, active, or commissionable until independently confirmed with the partner.
- Commission amounts, conversion events, Kerala availability and promotion permissions must be checked with the partner.
- Firebase web configuration in `firebase-config.js` is blank. Phone OTP, email/password and Google login are not live until a separate demo Firebase web app is configured and the relevant providers and GitHub Pages domain are enabled.
- Recharge MVP is simulated only. There is no live bill fetch, BBPS connection, recharge, payment collection, UPI mandate or AutoPay.
- Do not collect/store OTP, UPI PIN, CVV, bank passwords or other payment credentials in the demo.
- Do not connect production Firebase credentials or production domain to this preview.

## Current file map
- `index.html`: compact app-style home dashboard.
- `assets/theme.css`: shared near-black app theme.
- `favicon.svg`: FICTION CLUB app mark.
- `recharge-mvp.html`: simulated Kerala Pay experience.
- `bill-payments.html`: official external bill-payment portals.
- `credit-cards.html`: 38-card directory and comparison UI.
- `gromo-links.html`: 87-link partner audit register.
- `login.html`: Firebase Auth UI; configuration required.
- `firebase-config.js`: intentionally blank public web config placeholders.
- `.github/workflows/pages.yml`: GitHub Pages deployment workflow.

## Priorities
### P0 — demo usability
- Confirm GitHub Pages deployment and test every page on mobile.
- Verify navigation, buttons, search/filter, compare/shortlist, and simulated checkout.
- Keep all pages consistent with the black app-style theme.

### P1 — authentication
- Create/use a dedicated Firebase project for this demo only.
- Add its Web App config to `firebase-config.js`.
- Enable Phone, Email/Password and Google providers.
- Add the GitHub Pages hostname to Firebase Authorized domains.
- Test OTP, email create/sign-in/reset, Google sign-in, sign-out and session persistence.

### P2 — partner monetization
- Verify each partner URL and promotion permission with the relevant partner.
- Record approved status, Kerala eligibility, commission, conversion event, payout threshold and payment cycle only when sourced.
- Hide or clearly mark unverified offers; never invent earnings or approval claims.

### P3 — real payments
- Evaluate BBPS/API providers and onboarding requirements before implementation.
- Confirm business eligibility, fees, settlement, minimum payout, refund/dispute handling, security and compliance.
- Do not enable real payments until a compliant provider integration and testing are complete.

## Change-control rules
- Work only in `shafiintj-source/fictionclub-demo` unless the owner explicitly asks otherwise.
- Do not change `fictionclub.in`, production Firebase, AdSense or other production integrations as part of demo work.
- Keep payment/auth/partner claims transparent and evidence-based.
