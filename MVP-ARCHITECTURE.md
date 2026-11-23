# FICTION CLUB — Kerala Recharge & Bill Pay MVP

## Scope
- Product: Full Kerala-first recharge and bill-payment platform.
- AutoPay: explicitly deferred to a later phase.
- Production: untouched. This work exists only in the public isolated demo repository.
- Demo is noindex/nofollow and does not move real money.

## MVP user journey
1. Choose a service: prepaid mobile, DTH, electricity, water, gas, broadband, FASTag or landline.
2. Choose a provider and enter a customer identifier and demo amount.
3. Fetch a clearly labelled simulated bill.
4. Review amount and reference.
5. Simulate payment and receive a demo transaction ID.
6. View / clear transaction history stored only in the current browser.

## Architecture boundary
- Current frontend: static HTML/CSS/vanilla JavaScript.
- Current persistence: browser localStorage for demo history only.
- No backend, real customer lookup, BBPS connection, payment gateway, settlement, refund API, or AutoPay.
- No UPI PIN, OTP, card, bank credentials, or secret collection.

## Real-service architecture (future, after partner onboarding)
Browser UI → FICTION CLUB backend/API → authorized BBPS / payment partner → biller / payment network.
Backend owns customer/session validation, idempotency keys, signed webhook verification, transaction state machine, reconciliation, refund handling, audit logs, rate limits, and support escalation. Never trust a browser success redirect as proof of payment.

## Compliance and commercial gate
Before enabling live bill payments/recharges, select and contract with an authorized BBPS participant / suitable payment partner, complete business KYC and technical certification, obtain production credentials, confirm permitted biller categories, fees, settlement timelines, refunds/disputes and customer support responsibilities. Do not independently operate a regulated bill-payment system without the required authorization/partner arrangement.

## Release gates
- [ ] Verify demo UI on mobile and desktop browsers.
- [ ] Test all service selection buttons.
- [ ] Test validation for missing customer ID and invalid amount.
- [ ] Test simulated bill summary, simulated payment, transaction ID and local history.
- [ ] Confirm no external payment calls and no real personal/banking data is requested.
- [ ] Keep AdSense scripts off payment/checkout/status flows.
- [ ] Live mode remains disabled until partner, legal/compliance and security reviews pass.

## AutoPay — later
Only consider user-authorized recurring mandates through a supported regulated partner, with clear consent, mandate terms, pause/cancel controls, notifications, failure handling and audit trail.
