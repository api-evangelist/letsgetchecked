# LetsGetChecked

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

LetsGetChecked (operating as LetsGetChecked powered by FuzeHealth) is an Irish-American virtual care company that runs an end-to-end diagnostics and care platform: it manufactures at-home sample-collection kits, operates its own CLIA-accredited laboratories in the United States and Europe, and layers telehealth consultations, clinical review and affiliate-pharmacy prescription delivery on top of the results. Its Halo platform is a purpose-built EMR that exposes B2B REST APIs — the Orders API (v1 and v2), the Results API and the Outreach API — plus event-driven webhook notifications, so employers, health plans, providers, public-sector programs and life-sciences partners can order pre-activated test kits, track kit fulfillment, and retrieve laboratory results in JSON, HL7 or PDF form inside their own systems.

**Areas:** Company · Health · Healthcare · Diagnostics · Laboratory · Telehealth · Medical Testing · Pharmacy · Order · Results · Webhook · HL7

## LetsGetChecked on APIs.io

Everything profiled for LetsGetChecked is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/letsgetchecked/](https://apis.io/providers/letsgetchecked/)** — or go straight to one of the APIs or properties below.

### APIs (5)

- [LetsGetChecked Orders API (Version 1)](https://apis.io/apis/letsgetchecked/orders-api-v1/) — Version 1 of the LetsGetChecked Orders API. Create a pre-activated test-kit order against a client-supplied order identifier (PUT is documented as…
- [LetsGetChecked Orders API (Version 2)](https://apis.io/apis/letsgetchecked/orders-api-v2/) — Version 2 of the LetsGetChecked Orders API, documented September 2023. Adds an order-item model with per-item identifiers and statuses, a PATCH endpoint for…
- [LetsGetChecked Results API](https://apis.io/apis/letsgetchecked/results-api/) — Read laboratory results for test kits processed by the LetsGetChecked lab. Retrieve a full result set for a barcode (with optional alpha code), fetch just…
- [LetsGetChecked Outreach API](https://apis.io/apis/letsgetchecked/outreach-api/) — Retrieve and download the results letters LetsGetChecked generates for patients and for a patient's Primary Care Provider. List outreach notifications for a…
- [LetsGetChecked API Notifications (Webhooks)](https://apis.io/apis/letsgetchecked/api-notifications/) — Event-driven webhook notifications delivered by POST to client-supplied endpoints whenever an order, result or outreach resource changes. Payloads carry a…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Letsgetchecked Notifications Webhooks](https://apis.io/asyncapis/letsgetchecked/letsgetchecked-notifications-webhooks/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Letsgetchecked Authentication](https://apis.io/security/letsgetchecked/letsgetchecked-authentication/)
- [Letsgetchecked Domain Security](https://apis.io/security/letsgetchecked/letsgetchecked-domain-security/)
- [Letsgetchecked Trust Center](https://apis.io/security/letsgetchecked/letsgetchecked-trust-center/)
- [Letsgetchecked Vulnerability Disclosure](https://apis.io/security/letsgetchecked/letsgetchecked-vulnerability-disclosure/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.letsgetchecked.com/)
- [Documentation](https://docs.letsgetchecked.com/)
- [Getting started](https://docs.letsgetchecked.com/documentation/API%20Reference/Getting%20Started/integration-process/)
- [API reference](https://docs.letsgetchecked.com/documentation/API%20Reference/Getting%20Started/api-operations/)
- [Sign up](https://www.letsgetchecked.com/register/)
- [Support](https://help.letsgetchecked.com/s/)
- [Changelog](https://docs.letsgetchecked.com/documentation/release-notes/release_notes/)
- [Blog](https://www.letsgetchecked.com/articles/)
- [Security](https://www.letsgetchecked.com/security.txt)
- [Compliance](https://trust.letsgetchecked.com/)
- [Terms of service](https://www.letsgetchecked.com/terms-of-use/)
- [Privacy policy](https://www.letsgetchecked.com/privacy-policy/)
- [GitHub](https://github.com/LetsGetChecked)

## API Evangelist rating

**Kin Score 48.1** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 62.5 |
| Contract quality | 39.0 |
| Contract governance | 33.3 |
| Operational transparency | 31.6 |
| Developer ergonomics | 64.3 |
| Access clarity | 42.1 |

**Agent readiness 34.2** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | served (partial credit) |
| Idempotency | documented (partial credit) |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | yes |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 30.5** — Health

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/letsgetchecked/](https://apis.io/providers/letsgetchecked/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for LetsGetChecked: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/letsgetchecked/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
