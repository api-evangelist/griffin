# Griffin

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Griffin is a UK-regulated bank (Financial Conduct Authority authorised, Prudential Regulation Authority regulated) offering Banking-as-a-Service via a REST API. Fintechs and businesses embed FSCS-eligible bank accounts, payments (Faster Payments, BACS, CHAPS, book transfers, Confirmation of Payee), automated KYC/KYB onboarding (Verify), client-money and safeguarding accounts, savings accounts, and open banking directly into their own products. The v0 API uses API-key authentication with mandatory HTTP message signatures in live, documented webhooks, a full sandbox, and a first-party MCP server.

**Areas:** Company · Fintech · Banking · Banking as a Service · Payments · KYC · Open Banking · Bank Accounts · Financial Services

## Griffin on APIs.io

Everything profiled for Griffin is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/griffin/](https://apis.io/providers/griffin/)** — or go straight to one of the APIs or properties below.

### APIs (28)

- [Griffin API keys API](https://apis.io/apis/griffin/griffin-api-keys-api/) — The `api-key-secret` field is only shown once when you create an API key. We cannot recover the value, so you should store it securely. Pass an…
- [Griffin Bank account holds API](https://apis.io/apis/griffin/griffin-bank-account-holds-api/) — The Bank account holds API from Griffin — 2 operation(s) for bank account holds.
- [Griffin Bank account restrictions API](https://apis.io/apis/griffin/griffin-bank-account-restrictions-api/) — Restrictions prevent payments on a bank account. A `freeze` blocks outbound payments while still allowing inbound payments. A `block` prevents both inbound…
- [Griffin Bank accounts API](https://apis.io/apis/griffin/griffin-bank-accounts-api/) — Bank accounts are used for managing funds. Every bank account is opened against a [bank product](/docs/guides/bank-products), which determines the account's…
- [Griffin Claims API](https://apis.io/apis/griffin/griffin-claims-api/) — A [claim](/docs/terms/claim) is an unverified data point or series of data points attached to a [legal person](#tag/Legal-persons). Claims are verified by…
- [Griffin Companies House API](https://apis.io/apis/griffin/griffin-companies-house-api/) — The Companies House API from Griffin — 1 operation(s) for companies house.
- [Griffin Confirmation of payee API](https://apis.io/apis/griffin/griffin-confirmation-of-payee-api/) — The Confirmation of payee API from Griffin — 2 operation(s) for confirmation of payee.
- [Griffin Connectivity API](https://apis.io/apis/griffin/griffin-connectivity-api/) — The Connectivity API from Griffin — 1 operation(s) for connectivity.
- [Griffin Decisions API](https://apis.io/apis/griffin/griffin-decisions-api/) — The Decisions API from Griffin — 1 operation(s) for decisions.
- [Griffin Events API](https://apis.io/apis/griffin/griffin-events-api/) — The Events API from Griffin — 2 operation(s) for events.
- [Griffin Invitations API](https://apis.io/apis/griffin/griffin-invitations-api/) — Invitations enable [users](#tag/Users) to create new [memberships](#tag/Memberships) for their [organization](#tag/Organizations). The new membership is…
- [Griffin Legal person history API](https://apis.io/apis/griffin/griffin-legal-person-history-api/) — The Legal person history API from Griffin — 1 operation(s) for legal person history.
- [Griffin Legal persons API](https://apis.io/apis/griffin/griffin-legal-persons-api/) — In the Griffin API, your organization and your customers are all represented by [legal persons](/docs/terms/legal-person). When you sign up with Griffin,…
- [Griffin Memberships API](https://apis.io/apis/griffin/griffin-memberships-api/) — Memberships represents the relationship between a [user](#tag/Users) and an [organization](#tag/Organizations). A membership must have at least one…
- [Griffin Message Signatures API](https://apis.io/apis/griffin/griffin-message-signatures-api/) — Message Signatures confirm the identity of the sender and integrity of request messages. Key points: - Uses Ed25519 algorithm - Requires registering a…
- [Griffin Navigation API](https://apis.io/apis/griffin/griffin-navigation-api/) — The Navigation API from Griffin — 1 operation(s) for navigation.
- [Griffin Open banking API](https://apis.io/apis/griffin/griffin-open-banking-api/) — Open banking allows regulated third-party providers (TPPs) to access your customers' account data or initiate payments on their behalf. Griffin partners…
- [Griffin Organizations API](https://apis.io/apis/griffin/griffin-organizations-api/) — The organization resource represents your company and acts as a container for the majority of other resources, including [legal persons](#tag/Legal-Persons)…
- [Griffin Payees API](https://apis.io/apis/griffin/griffin-payees-api/) — A payee is the person or business to whom you are paying money. When you create a payee, you need to provide their name (`"account-holder"`), and their bank…
- [Griffin Payments API](https://apis.io/apis/griffin/griffin-payments-api/) — A payment captures the intent to move funds from a bank account to another bank account. Outbound payments can be made from your [bank…
- [Griffin Pooled account membership API](https://apis.io/apis/griffin/griffin-pooled-account-membership-api/) — The Pooled account membership API from Griffin — 2 operation(s) for pooled account membership.
- [Griffin Reliance onboarding API](https://apis.io/apis/griffin/griffin-reliance-onboarding-api/) — Reliance onboarding allows you to create and submit an application on behalf of your customer, using information about them you have already collected. For…
- [Griffin Roles API](https://apis.io/apis/griffin/griffin-roles-api/) — A role represents a pre-defined set of capabilities that can be assigned to a [user](#tag/Users) via their [membership](#tag/Memberships) in an…
- [Griffin Transactions API](https://apis.io/apis/griffin/griffin-transactions-api/) — A transaction represents funds deposited or withdrawn from a bank account. Read more about transactions [in our guides](/docs/guides/transactions).
- [Griffin Users API](https://apis.io/apis/griffin/griffin-users-api/) — Users represent individuals who use the Griffin platform. A user must have a [membership](#tag/Memberships) in at least one…
- [Griffin Verifications API](https://apis.io/apis/griffin/griffin-verifications-api/) — The Verifications API from Griffin — 4 operation(s) for verifications.
- [Griffin Webhooks API](https://apis.io/apis/griffin/griffin-webhooks-api/) — The Webhooks API from Griffin — 5 operation(s) for webhooks.
- [Griffin Workflows API](https://apis.io/apis/griffin/griffin-workflows-api/) — A [workflow](/docs/terms/workflow) determines which checks will be run against a [legal person](#tag/Legal-persons) as part of a…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Griffin Webhooks](https://apis.io/asyncapis/griffin/griffin-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [griffin](https://apis.io/servers/griffin/griffin/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Griffin Agentic Access](https://apis.io/agentic-access/griffin/griffin-agentic-access/)

#### Collections (28)

Postman and Open Collection request collections.

- [The Griffin API keys API](https://apis.io/collections/griffin/open-griffin-api-keys-api/)
- [The Griffin API keys Bank account holds API](https://apis.io/collections/griffin/open-griffin-bank-account-holds-api/)
- [The Griffin API keys Bank account restrictions API](https://apis.io/collections/griffin/open-griffin-bank-account-restrictions-api/)
- [The Griffin API keys Bank accounts API](https://apis.io/collections/griffin/open-griffin-bank-accounts-api/)
- [The Griffin API keys Claims API](https://apis.io/collections/griffin/open-griffin-claims-api/)
- [The Griffin API keys Companies House API](https://apis.io/collections/griffin/open-griffin-companies-house-api/)
- [The Griffin API keys Confirmation of payee API](https://apis.io/collections/griffin/open-griffin-confirmation-of-payee-api/)
- [The Griffin API keys Connectivity API](https://apis.io/collections/griffin/open-griffin-connectivity-api/)
- [The Griffin API keys Decisions API](https://apis.io/collections/griffin/open-griffin-decisions-api/)
- [The Griffin API keys Events API](https://apis.io/collections/griffin/open-griffin-events-api/)
- [The Griffin API keys Invitations API](https://apis.io/collections/griffin/open-griffin-invitations-api/)
- [The Griffin API keys Legal person history API](https://apis.io/collections/griffin/open-griffin-legal-person-history-api/)
- [The Griffin API keys Legal persons API](https://apis.io/collections/griffin/open-griffin-legal-persons-api/)
- [The Griffin API keys Memberships API](https://apis.io/collections/griffin/open-griffin-memberships-api/)
- [The Griffin API keys Message Signatures API](https://apis.io/collections/griffin/open-griffin-message-signatures-api/)
- [The Griffin API keys Navigation API](https://apis.io/collections/griffin/open-griffin-navigation-api/)
- [The Griffin API keys Open banking API](https://apis.io/collections/griffin/open-griffin-open-banking-api/)
- [The Griffin API keys Organizations API](https://apis.io/collections/griffin/open-griffin-organizations-api/)
- [The Griffin API keys Payees API](https://apis.io/collections/griffin/open-griffin-payees-api/)
- [The Griffin API keys Payments API](https://apis.io/collections/griffin/open-griffin-payments-api/)
- [The Griffin API keys Pooled account membership API](https://apis.io/collections/griffin/open-griffin-pooled-account-membership-api/)
- [The Griffin API keys Reliance onboarding API](https://apis.io/collections/griffin/open-griffin-reliance-onboarding-api/)
- [The Griffin API keys Roles API](https://apis.io/collections/griffin/open-griffin-roles-api/)
- [The Griffin API keys Transactions API](https://apis.io/collections/griffin/open-griffin-transactions-api/)
- [The Griffin API keys Users API](https://apis.io/collections/griffin/open-griffin-users-api/)
- …and 3 more published on APIs.io

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Griffin Api Overlay](https://apis.io/overlays/griffin/griffin-api-overlay/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Griffin API Rules](https://apis.io/rules/griffin/griffin-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Griffin Authentication](https://apis.io/security/griffin/griffin-authentication/)
- [Griffin Domain Security](https://apis.io/security/griffin/griffin-domain-security/)

#### Plans and pricing (2)

Published plans, tiers and prices.

- [Griffin Plans Pricing](https://apis.io/plans/griffin/griffin-plans-pricing/)
- [Griffin Price Estimates](https://apis.io/plans/griffin/griffin-price-estimates/)

#### Rate limits (1)

Published request limits.

- [Griffin Rate Limits](https://apis.io/rate-limits/griffin/griffin-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://griffin.com/)
- [Documentation](https://docs.griffin.com/)
- [Getting started](https://docs.griffin.com/docs/guides/get-started-with-the-api)
- [API reference](https://docs.griffin.com/api)
- [Pricing](https://griffin.com/pricing)
- [Sign up](https://app.griffin.com/register)
- [Support](https://docs.griffin.com/)
- [Changelog](https://updates.griffin.com/)
- [Blog](https://griffin.com/blog)
- [Terms of service](https://griffin.com/terms)
- [Privacy policy](https://griffin.com/privacy)
- [GitHub](https://github.com/griffinbank)
- [Status](https://status.griffin.com/)

## API Evangelist rating

**Kin Score 65.2** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 75.0 |
| Contract quality | 61.7 |
| Contract governance | 35.6 |
| Operational transparency | 71.1 |
| Developer ergonomics | 78.0 |
| Access clarity | 69.7 |

**Agent readiness 36.7** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | documented (partial credit) |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | verified |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | mostly |

**Regulatory alignment 19.7** — Banking & Open Finance

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/griffin/](https://apis.io/providers/griffin/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Griffin: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/griffin/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
