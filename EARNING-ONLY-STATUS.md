# FICTION CLUB — earning-only demo status

## Current result
- Source catalogue: 87 GroMo entries.
- Verified for promotion: 0.
- Verified commission and Kerala/India eligibility: 0.
- No product is currently published in the earning hub.
- Source records and product image references are preserved; nothing is deleted.

## Strict display gate
An offer appears only when all of these fields are confirmed in assets/gromo-products.json:
- verified = true
- indiaEligible = true
- commissionVerified = true
- promotionPermission = true
- trackingUrlVerified = true
- conversionEventVerified = true
- url is a valid HTTPS tracking URL
- commissionDetails is a non-empty, partner-confirmed description

## Partner confirmation checklist
1. Confirm the offer is active in the partner dashboard.
2. Generate and test the publisher-specific tracking URL.
3. Confirm the commission amount/rule and eligible conversion event.
4. Confirm India and Kerala traffic eligibility.
5. Confirm FICTION CLUB is allowed to promote the offer and use its product image.
6. Record the confirmation date and partner source before setting the verification fields to true.

## Demo UI
- Home page points to the verified earning hub only.
- Credit-card and finance pages hide unverified offers.
- The earning hub renders approved products and partner-supplied images only.
- Production fictionclub.in, production Firebase and AdSense are not changed.
