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

LetsGetChecked (operating as LetsGetChecked powered by FuzeHealth) runs an end-to-end virtual
care and diagnostics platform: it manufactures at-home sample-collection kits, operates its own
accredited laboratories in the United States and Europe, and layers telehealth, clinical review
and affiliate-pharmacy prescription delivery on top of the results. Its Halo platform exposes
B2B REST APIs — Orders (v1 and v2), Results and Outreach — plus event-driven webhook
notifications, so employers, health plans, providers, public-sector programs and life-sciences
partners can order pre-activated test kits, track fulfillment, and retrieve laboratory results
in JSON, HL7 or PDF inside their own systems.

- Website: https://www.letsgetchecked.com/
- Developer documentation: https://docs.letsgetchecked.com/
- Trust centre: https://trust.letsgetchecked.com/
- Report a vulnerability: https://www.letsgetchecked.com/security.txt

## What this profile found

The API surface is **documented but partner-gated**. LetsGetChecked publishes a full prose API
reference — authentication, four API surfaces, a webhook catalogue, an error-code table, a
37-term glossary and dated release notes — but no machine-readable contract of any kind, and no
API hostname. Every documented endpoint is templated as `{LGC-API}`; the host, credentials and
staging access are issued privately during onboarding.

Confirmed absent after direct probing on 2026-08-04: no OpenAPI or Swagger (checked the docs
host root, `/openapi.json`, `/openapi.yaml`, `/swagger.json`, the GitHub org, and the Halo
host), no AsyncAPI, no GraphQL, no gRPC, no MCP server, no A2A agent card, no client libraries
on any public package registry, no CLI, no Postman collection, no status page and no SLA.

Two probe results are recorded specifically so a later pass does not repeat the mistake:
`halo.letsgetchecked.com` and `trust.letsgetchecked.com` answer **HTTP 200 with an HTML
application shell for every `/.well-known/*` path** — those are SPA catch-alls, not documents.
And the trust centre is a shared Conveyor page that embeds other vendors' certification lists;
LetsGetChecked's own record claims **GDPR, HITRUST, NIST and ISO 13485**, and does *not* claim
SOC 2 or ISO 27001.

Three defects worth reporting back to the provider:

1. The Docusaurus docs site is deployed with `url`/`baseUrl` unset — `sitemap.xml` emits every
   entry as `http://localhost/...`, so crawlers and agents following it resolve nothing.
2. `security.txt` is served only from the legacy `/security.txt` path, not the RFC 9116
   `/.well-known/security.txt`, and its `Expires` value (2024-03-01) has passed.
3. No release note has been published since 14 September 2023.
