# Diligent (diligent-boards)

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
