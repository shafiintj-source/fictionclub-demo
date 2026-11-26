# FICTION CLUB — partner and demo audit

Checked: 26 November 2026  
Repository: `shafiintj-source/fictionclub-demo`  
Scope: isolated demo repository and partner email threads. Production website, production Firebase, AdSense settings and live integrations were not changed.

## Executive result

- Publicly displayable, partner-verified earning offers: **0**.
- GroMo source catalogue: **87** saved records. All 87 currently fail every required partner-verification flag. Their HTTPS format alone does not prove the links are active or commissionable.
- Demo deployment: latest GitHub Pages build job succeeded, but deployment failed with a GitHub Pages API HTTP 500 on 26 November workflow run #79. The log does not show the previously suspected Actions-storage quota error.
- Production website: no changes made.
- Demo pages carry `noindex,nofollow`; this is intentional for an isolated preview, not a public SEO launch.

## 1. Demo UI and functionality

Repository pages found:
- `index.html`: verified-earning dashboard; reads the GroMo JSON and displays only records that pass the strict gate.
- `earning-hub.html`: searchable earning directory; displays only fully verified records.
- `credit-cards.html`, `gromo-links.html`, `travel-tickets.html`: holding pages; unverified offers are hidden.
- `recharge-mvp.html`: Malayalam-first simulated recharge/bill flow.
- `bill-payments.html`: links to official provider portals; payment is completed on those provider sites, not FICTION CLUB.
- `login.html`: sign-in interface, but Firebase configuration is intentionally blank.

UI is mobile-responsive and uses a dark theme with lime accents in the shared demo styles. However, a full real-device/browser QA pass has not been evidenced. Login is not live, payment is not live, and no actual BBPS/bill fetch is connected.

## 2. Affiliate links and earning eligibility

### GroMo
- 87 records retained; none deleted.
- Current JSON check: 0/87 have `verified=true`, `indiaEligible=true`, `commissionVerified=true`, `promotionPermission=true`, `trackingUrlVerified=true`, or `conversionEventVerified=true`.
- Therefore no GroMo item may be described as approved, Kerala-eligible, commissionable, or earning.
- Ticket #667691 asking for a link-wise audit was closed without the requested audit report. Do not infer approval from ticket closure.

### Cuelinks
- AbhiBus ticket #149111: support acknowledged the reply on 25 November; review remains pending. No campaign approval has been received.
- Generic Cuelinks campaign/payout newsletters, including the 26 November update, are not FICTION CLUB-specific approval and do not establish AbhiBus eligibility.

### Admitad / Mitgo
- Request #20722 was acknowledged on 25 November; support said it is under review and promised a response within three business days.
- No publisher/cashback approval or campaign approval is confirmed.

### vCommission
- On 26 November, support replied to ticket #160382 and asked for the email address registered to the vCommission publisher account.
- This is an identity/account lookup step, not approval or rejection. The registered address has not yet been confirmed by the owner; reply in the same thread once confirmed.

### Travelpayouts and CJ
- Ten Travelpayouts tracking URLs were previously saved, but they have not been independently redirect-tested in this audit. Confirm the relevant campaign is active, India/Kerala inventory is bookable and the traffic method is allowed before display.
- Earlier CJ dashboard records showed advertiser relationships, but publisher-specific tracked links were not collected in the saved audit. An active advertiser relationship alone is not a tested earning link.

## 3. Content and AdSense readiness

- This repository is a demo, not the production article/content site. Its `noindex,nofollow` tags are appropriate for a preview.
- The demo contains no completed production article/content audit. A previous production sitemap review recorded 47 URLs, but this audit did not re-crawl or score all 47 production pages.
- Do not mark the 25-article rewrite/content review as complete without a page-by-page quality, originality, usefulness, accuracy, navigation and policy check.
- Keep ads off the demo payment/login flows. Do not add AdSense scripts or alter production ad placements during the suspension/review period.

## 4. Deployment and repository hygiene

- Repository currently has a single `main` branch as checked before this audit branch was created.
- Latest workflow run #79: build succeeded; deploy job failed while creating the Pages deployment, HTTP 500 from the GitHub Pages deployment API. This log does not indicate a storage-quota failure.
- Retry deployment after GitHub Pages service recovers; do not change production Firebase or the live domain to work around this.
- The previous README referenced `PARTNER-AUDIT-2026-11-25.md`, which was missing from the repository. This 26 November report replaces that broken reference.

## 5. Production safety boundary

- Work only in this isolated demo repository.
- Do not deploy demo changes to `fictionclub.in`.
- Do not modify production Firebase, AdSense, `ads.txt`, DNS, SEO/indexing, live affiliate integrations or live payment settings.
- No live BBPS, real bill fetch, recharge, payment collection, UPI mandate or AutoPay is enabled.
- Keep all unverified affiliate records preserved but hidden. Only update verification flags after written partner evidence confirms each required field.

## Next actions

1. Reply to vCommission with the actual registered publisher email.
2. Wait for Cuelinks AbhiBus and Admitad/Mitgo ticket outcomes; request written campaign-level terms.
3. Ask GroMo to reopen/escalate ticket #667691 and provide a row-by-row response for all 87 links.
4. Once a partner confirms an offer, test its publisher tracking URL and record commission, conversion event, India/Kerala eligibility, promotion permission and confirmation date.
5. Retry GitHub Pages deployment after the HTTP 500 issue clears, then perform mobile and desktop QA.
6. Separately audit the 47 production sitemap URLs read-only; do not edit production during the current AdSense suspension/review window.
