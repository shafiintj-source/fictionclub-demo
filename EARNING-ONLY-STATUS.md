# FICTION CLUB — earning-only demo status

Last checked: 25 November 2026

## Current result
- Source catalogue: 87 GroMo entries.
- Verified for promotion: 0.
- Verified commission and Kerala/India eligibility: 0.
- No product is currently published in the earning hub.
- Source records and product image references are preserved; nothing is deleted.
- The catalogue was imported on 4 November 2026; no partner-confirmed link-level update has been received since import.

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

## Partner confirmation checklist
1. Confirm the offer is active in the partner dashboard.
2. Generate and test the publisher-specific tracking URL.
3. Confirm the commission amount/rule and eligible conversion event.
4. Confirm India and Kerala traffic eligibility, including state/PIN/route restrictions.
5. Confirm FICTION CLUB is allowed to promote the offer and use its product image.
6. Record the confirmation date and partner source before setting verification fields to true.

## Partner follow-up status — 25 November 2026
- GroMo ticket #667691: requested audit of all 87 links; ticket closed without the link-wise report. Do not mark any offer approved.
- Cuelinks AbhiBus ticket #149111: acknowledgement received; review pending. No campaign approval.
- Admitad/Mitgo request #20722: acknowledgement received; response promised within three business days. No publisher/campaign approval.
- vCommission: follow-up sent; no response recorded.
- See `PARTNER-AUDIT-2026-11-25.md` for details.

## Demo UI
- Home page points to the verified earning hub only.
- Credit-card and finance pages hide unverified offers.
- The earning hub renders approved products and partner-supplied images only.
- Production `fictionclub.in`, production Firebase and AdSense are not changed.
