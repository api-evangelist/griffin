---
name: Create and submit a Faster Payment
description: Create a payee and send an outbound payment from a Griffin bank account, then reconcile via transactions, using the v0 API.
api: openapi/griffin-openapi-original.yml
operations:
  - POST /v0/legal-persons/{legal-person-id}/bank/payees
  - POST /v0/bank/accounts/{bank-account-id}/payments
  - GET /v0/bank/accounts/{bank-account-id}/transactions
---

# Create and submit a payment

Send money out of a Griffin bank account to a payee (Faster Payments / book transfer).

## Auth
- `Authorization: GriffinAPIKey $GRIFFIN_API_KEY` (+ RFC 9421 message signature, mandatory in live).

## Steps
1. **Create the payee** — `POST /v0/legal-persons/{legal-person-id}/bank/payees` with the beneficiary sort code/account number. Optionally run Confirmation of Payee (`POST /v0/organizations/{organization-id}/cop-request`) first. Capture `payee-id`.
2. **Create the payment** — `POST /v0/bank/accounts/{bank-account-id}/payments` referencing the payee and amount. This creates and submits the payment.
3. **Reconcile** — `GET /v0/bank/accounts/{bank-account-id}/transactions` (and listen for the `transaction-created` webhook) to confirm settlement. Do not treat webhook receipt as sole proof — verify via the API.

## Rules
- Sandbox payments never reach real schemes and always succeed; live payments can be rejected (see `payment-errors` and `errors/griffin-problem-types.yml`).
- No idempotency-key header — avoid blind retries on `POST payments`; re-list payments before re-sending.
- Webhook delivery is at-least-once and unordered (`asyncapi/griffin-webhooks.yml`).
