# Diligent

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

Diligent Corporation is a governance, risk, and compliance (GRC) software company best known for its board management portal (Diligent Boards / Boardbooks) and the broader Diligent One Platform, which unifies board management, enterprise risk, audit, compliance, entity management, and ESG. The board portal itself is a security-hardened product with no public developer API - it is integrated through SSO (SAML 2.0), SCIM provisioning, and packaged connectors (Okta, Microsoft 365/Teams, Zoom, DocuSign). Diligent does, however, publish a real developer portal at developer.diligent.com covering the GRC side of the platform - the HighBond (Diligent One) REST API for audit/risk/compliance data, a GraphQL Entities API for legal-entity and subsidiary management, an ESG API for activity/usage data, and a Workflow API for jobs, tasks, and campaigns. API access is customer/partner-gated (a HighBond API key or SSO-scoped token is required) and pricing is quote-based via Diligent sales.

**Areas:** Governance · Risk Management · Compliance · GRC · Board Management · Audit · Entity Management · ESG · Enterprise

## Diligent on APIs.io

Everything profiled for Diligent is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/diligent-boards/](https://apis.io/providers/diligent-boards/)** — or go straight to one of the APIs or properties below.

### APIs (4)

- [Diligent HighBond API (Diligent One)](https://apis.io/apis/diligent-boards/diligent-highbond-api/) — REST API for the Diligent One Platform (formerly HighBond) covering the governance, risk, and compliance surface - organizations, projects, control tests,…
- [Diligent Entities API](https://apis.io/apis/diligent-boards/diligent-entities-api/) — GraphQL API for Diligent Entities - managing company/legal-entity records, their structure, obligations, and legal characteristics, plus an Entities Reports…
- [Diligent ESG API](https://apis.io/apis/diligent-boards/diligent-esg-api/) — Developer interface for the Diligent ESG platform, used to send activity-entry (usage) data into Diligent ESG from internal systems for sustainability and…
- [Diligent Workflow API](https://apis.io/apis/diligent-boards/diligent-workflow-api/) — REST API built around standard HTTPS requests with JSON responses for the Diligent Workflow product. Reports across Business Areas, Job Owners, Jobs, Tasks,…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Diligent Boards Domain Security](https://apis.io/security/diligent-boards/diligent-boards-domain-security/)
- [Diligent Boards Trust Center](https://apis.io/security/diligent-boards/diligent-boards-trust-center/)
- [Diligent Boards Vulnerability Disclosure](https://apis.io/security/diligent-boards/diligent-boards-vulnerability-disclosure/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.diligent.com/)
- [Documentation](https://developer.diligent.com/)
- [Blog](https://www.diligent.com/resources/blog)
- [Terms of service](https://developer.diligent.com/docs/api_terms_of_use)

## API Evangelist rating

**Kin Score 13.5** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 0.0 |
| Contract governance | 0.0 |
| Operational transparency | 0.0 |
| Developer ergonomics | 9.5 |
| Access clarity | 18.4 |

**Agent readiness 0.0** — human-only

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | — |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 20.6** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/diligent-boards/](https://apis.io/providers/diligent-boards/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Diligent: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/diligent-boards/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
