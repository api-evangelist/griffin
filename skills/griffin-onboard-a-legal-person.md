---
name: Onboard and verify a legal person (KYC/KYB)
description: Create a legal person under an organization, run a KYC/KYB verification, and read the resulting decision using the Griffin v0 API.
api: openapi/griffin-openapi-original.yml
operations:
  - POST /v0/organizations/{organization-id}/legal-persons
  - POST /v0/legal-persons/{legal-person-id}/verifications
  - GET /v0/legal-persons/{legal-person-id}/decisions
---

# Onboard and verify a legal person

Use this to bring an individual or company into Griffin as a verified `legal-person` before opening accounts or moving money.

## Auth
- Header: `Authorization: GriffinAPIKey $GRIFFIN_API_KEY` (sandbox keys are prefixed `g-test-`).
- In live, every request must also carry an HTTP message signature (RFC 9421). In sandbox this is optional unless "Validate all requests" is on.
- `Content-Type: application/json` on bodies; `Accept: application/json`.

## Steps
1. **Create the legal person** — `POST /v0/organizations/{organization-id}/legal-persons`. Supply the individual/company details Griffin onboards (see docs: entities-we-onboard). Capture the returned `legal-person-id`.
2. **Run verification** — `POST /v0/legal-persons/{legal-person-id}/verifications` to perform KYC/KYB. In sandbox no third-party checks run; results are simulated.
3. **Read the decision** — `GET /v0/legal-persons/{legal-person-id}/decisions` to retrieve the onboarding decision. Poll until a decision is present.

## Rules
- Errors follow a JSON:API-influenced shape (not RFC 9457); field errors carry a `source` JSON pointer — surface `source` + `detail` to the user. See `errors/griffin-problem-types.yml`.
- No idempotency-key header exists; do not retry a create blindly — re-list before re-creating.
- Rate limit: 50 concurrent in-flight requests per org → `429`; back off.
