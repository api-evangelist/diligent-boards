# Diligent (diligent-boards)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Diligent Corporation is a governance, risk, and compliance (GRC) software company best known for its board management portal - **Diligent Boards / Boardbooks** - and the broader **Diligent One Platform**, which unifies board management, enterprise risk, audit, compliance, entity management, and ESG.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/diligent-boards/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/diligent-boards/refs/heads/main/apis.yml)

## Access Model (read this first)

Diligent's API footprint is split, and it is important to be honest about it:

- **The board portal itself (Diligent Boards / Boardbooks) has no public developer API.** It is a security-hardened product integrated only through **SSO (SAML 2.0)**, **SCIM provisioning**, and packaged connectors (Okta, Microsoft 365 / Teams, Zoom, DocuSign). There is no documented REST/GraphQL surface for meetings, board books, minutes, or director records.
- **The GRC side of the platform does have a real developer portal** at [developer.diligent.com](https://developer.diligent.com/). This covers the HighBond (Diligent One) REST API, a GraphQL Entities API, an ESG API, and a Workflow API.
- **All access is customer / partner-gated.** You need a HighBond API key (Bearer token, with read/write/admin scopes and an expiry) or an Entities Reports API access token. There is no open self-serve tier.
- **Pricing is quote-based** - contact Diligent sales. There is no public pricing page or public rate-limit table, so no `plans/`, `rate-limits/`, or `finops/` artifacts were fabricated for this entry.
- **Endpoints are modeled from public help/reference docs**, not from a published OpenAPI definition. No OpenAPI or Postman artifacts were invented.

## Tags

- Governance
- Risk
- Compliance
- GRC
- Board Management
- Audit
- Entity Management
- ESG
- Enterprise

## Timestamps

- **Created:** 2026-07-05
- **Modified:** 2026-07-05

## APIs

### Diligent HighBond API (Diligent One)

REST API for the Diligent One Platform (formerly HighBond) covering the governance, risk, and compliance surface - organizations, projects, control tests, risks, controls, issues, frameworks, results collections, and records. JSON over HTTPS, authenticated with a HighBond API key (Bearer token). Base URLs are region-scoped (`apis-us` / `apis-ca` / `apis-eu` / `apis-ap` / `apis-au` / `apis-af` / `apis-sa` / `apis-jp`.highbond.com, plus `diligentoneplatform.com`).

- **Human URL:** [https://developer.diligent.com/api/highbond](https://developer.diligent.com/api/highbond)
- **Base URL:** `https://apis-us.highbond.com/v1`
- **Reference:** [docs-apis.highbond.com](https://docs-apis.highbond.com/)

### Diligent Entities API

GraphQL API for Diligent Entities - managing company / legal-entity records, their structure, obligations, and legal characteristics, plus an Entities Reports API. Root-level mutations create, update, and delete entities. The full schema is downloadable as `schema.graphql`, and Diligent recommends generating a typed client (e.g. Strawberry Shake for .NET). Requires a Reports API access token.

- **Human URL:** [https://developer.diligent.com/api/entities](https://developer.diligent.com/api/entities)
- **Guidelines:** [Consuming the Entities GraphQL API](https://developer.diligent.com/docs/entities_graphql_api_guidelines)

### Diligent ESG API

Developer interface for the Diligent ESG platform, used to send activity-entry (usage) data into Diligent ESG from internal systems for sustainability and emissions reporting. REST over HTTPS with JSON, gated by a HighBond / Diligent One API key.

- **Human URL:** [https://developer.diligent.com/api/esg](https://developer.diligent.com/api/esg)

### Diligent Workflow API

REST API built around standard HTTPS requests with JSON responses for the Diligent Workflow product. Reports across Business Areas, Job Owners, Jobs, Tasks, Campaigns, and expiries, plus creating and updating jobs with files and folders.

- **Human URL:** [https://developer.diligent.com/api/workflow](https://developer.diligent.com/api/workflow)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/diligent)
- [Website](https://www.diligent.com/)
- [Documentation (Developer Portal)](https://developer.diligent.com/)
- [Partners](https://www.diligent.com/company/partners)
- [API Terms of Use](https://developer.diligent.com/docs/api_terms_of_use)
- [Board Management (product)](https://www.diligent.com/lp/more-than-a-board-portal)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
