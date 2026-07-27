---
name: Open a bank account for a verified legal person
description: Select a bank product and open a bank account for a verified legal person using the Griffin v0 API.
api: openapi/griffin-openapi-original.yml
operations:
  - GET /v0/bank/products/{bank-product-id}
  - POST /v0/bank/products/{bank-product-id}/accounts
  - GET /v0/bank/accounts/{bank-account-id}
---

# Open a bank account

Open a Griffin bank account (operational, client-money, safeguarding, savings, or embedded) once the account owner is a verified `legal-person`.

## Auth
- `Authorization: GriffinAPIKey $GRIFFIN_API_KEY` (+ message signature in live).

## Steps
1. **Inspect the product** — `GET /v0/bank/products/{bank-product-id}` to confirm the product type and constraints for the account you want to open.
2. **Open the account** — `POST /v0/bank/products/{bank-product-id}/accounts`, referencing the verified `legal-person-id` as the account owner. Capture the returned `bank-account-id`.
3. **Confirm** — `GET /v0/bank/accounts/{bank-account-id}` and check the account status.

## Rules
- In sandbox each new account is auto-credited with £1,000,000 of test money and has simulated sort code/account number (not reachable by real schemes). See `sandbox/griffin-sandbox.yml`.
- The owner must be an onboarded, verified legal person first (see the onboard-a-legal-person skill).
- Errors: JSON:API-influenced envelope with `source`/`detail` (`errors/griffin-problem-types.yml`).
