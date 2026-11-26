# FICTION CLUB — earning-only demo status

Last checked: 26 November 2026

## Current result
- Source catalogue: 87 GroMo entries.
- Verified for promotion: 0.
- Verified commission and Kerala/India eligibility: 0.
- No product is currently published in the earning hub.
- Source records and product image references are preserved; nothing is deleted.
- All 87 current records fail the required verification flags. HTTPS URL format alone is not proof of a working tracking link.

## Strict display gate
An offer appears only when all of these fields are confirmed in `assets/gromo-products.json`:
- `verified = true`
- `indiaEligible = true`
- `commissionVerified = true`
- `promotionPermission = true`
- `trackingUrlVerified = true`
- `conversionEventVerified = true`
- `url` is a valid HTTPS tracking URL
- `commissionDetails` is a non-empty, partner-confirmed description

Never set these fields true based on an automated acknowledgement, a generic newsletter, a public product page, or an unverified promotional claim.

## Partner follow-up status — 26 November 2026
- GroMo ticket #667691: request to audit all 87 links was closed without the requested link-wise report. Keep all entries hidden.
- Cuelinks AbhiBus ticket #149111: reply acknowledged on 25 November; review pending. No campaign approval.
- Admitad/Mitgo request #20722: received on 25 November; response promised within three business days. No publisher/campaign approval.
- vCommission ticket #160382: on 26 November support requested the registered publisher email ID. Account lookup pending; this is not approval or rejection.
- Travelpayouts: 10 saved tracking URLs exist, but were not independently redirect-tested in this audit.
- CJ: earlier advertiser relationships do not prove that publisher-specific tracking links are ready or that a campaign is approved for FICTION CLUB promotion.

See `PARTNER-AUDIT-2026-11-26.md` for the full evidence-based status.

## Demo UI and safety
- Home page reads the catalogue and shows only records that pass the strict verification gate.
- Credit-card and finance pages hide unverified offers.
- The earning hub has no verified offers to display at present.
- Recharge/bill-pay is simulated or links to official provider portals; no real payment processing is enabled.
- Firebase config is intentionally blank; demo sign-in is not live.
- Production `fictionclub.in`, production Firebase and AdSense are not changed.
