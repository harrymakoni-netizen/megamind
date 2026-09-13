# Megamind

A working local innovation-fair prototype based on Megamind Development Proposal v2. The interface demonstrates evidence-graded financial identity, separate USD/ZiG cash records and an anchor-owned network view.

## Run

Requires Node.js 22.12+ (Node 24 used here).

```sh
npm install
npm run dev
```

Open http://127.0.0.1:5173. `npm run build` creates `dist/`. `npm test` checks the calculation and data-boundary functions.

## Working features

- Responsive business dashboard with the supplied logo.
- Review-before-post transaction capture, persisted in localStorage.
- Currency filter, counterparty search and transaction evidence details.
- Separate currency balances and per-currency passport sales evidence.
- Replacement-cost margin calculator with explicit manual rate and date.
- Business passport JSON export and browser print / PDF layout.
- Anchor signals from a separate fictional dataset, using an explicit field allowlist.
- Privacy explanation and a three-minute presentation guide.

## Demonstration boundaries

All businesses, transactions, counterparties and confirmation statuses are fictional examples. The prototype is not the full production system from the proposal. localStorage is not encrypted, authenticated, backed up or synchronized. The anchor screen is a demonstration perspective, not a security role: the browser bundle contains both fictional datasets. Use no real personal or financial records.

This is a cash-movement ledger, not a complete double-entry accounting engine. No live anchor imports, identity matching, voice/OCR parsing, SMS confirmations, banking, lending, rate feeds, forecasts or production consent/access-log services are connected. Browser persistence works after loading; offline cold-start installation and synchronization are not implemented. Fonts use Google Fonts with local sans-serif fallbacks.

The anchor constraint label is a transparent heuristic, not a validated financial diagnosis. Passport grades refer to demonstration evidence; no real supporting source artefacts or lender acceptance are claimed.

## Next implementation milestones

1. Confirm the fair date, judging criteria and demonstration time, then rehearse the in-app presentation guide.
2. Add a transactional database, double-entry posting rules, server authentication and tenant authorization. Test anchor/private data isolation at the API layer.
3. Build historical CSV ingestion with source provenance, duplicates, reconciliation and business-confirmed identity matches. Keep unmatched records unattributed.
4. Add consent grants with recipient, scope, purpose and expiry; immediate revocation; business-visible access logs; and tests for refusal invisibility.
5. Implement an offline PWA queue and recoverable synchronization before field trials, followed by multilingual capture with mandatory confirmation.
6. Validate accounting and currency treatment with a qualified reviewer, arrange appropriate data-transfer safeguards before real extracts, and test with businesses and prospective anchors/lenders.

No messages were sent, external services provisioned or public deployment made during this build.
