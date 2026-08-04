# DataCite (datacite)

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

DataCite is a leading global non-profit organization that provides DOI (Digital Object Identifier) registration and persistent identifier services for research outputs, enabling researchers to cite, discover, and access scholarly data. DataCite maintains a REST API for minting and managing DOIs, querying metadata records, and accessing the global research data graph. Membership-based access allows institutions to register DOIs through APIs and the Fabrica web interface, while public metadata retrieval is freely available to anyone. DataCite also offers a GraphQL API, a legacy Metadata Store (MDS) API, usage statistics via its Usage Reports API, and scholarly event tracking via the Event Data API.

APIs.json: [https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/apis.yml)

Manage and deploy this API using Naftiko: [https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=datacite-api-evangelist&utm_content=repo](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=datacite-api-evangelist&utm_content=repo)

## Tags

- DOI
- Persistent Identifiers
- Scholarly Metadata
- Research Data
- Open Science
- Linked Data

## APIs

| Name | Description | Human URL |
|------|-------------|-----------|
| DataCite REST API | Primary interface for retrieving, creating, and updating DOI metadata records following JSON:API spec. | https://support.datacite.org/docs/api |
| DataCite GraphQL API | Alternative query interface for DOI metadata retrieval using the GraphQL query language. | https://support.datacite.org/docs/datacite-graphql-api-guide |
| DataCite MDS API | Legacy Metadata Store API for DOI registration and metadata management. | https://support.datacite.org/docs/mds-api-guide |
| DataCite Event Data API | Tracks mentions, citations, and scholarly events related to registered DOIs. | https://support.datacite.org/docs/apis |
| DataCite Usage Reports API | COUNTER-compliant usage statistics for registered DOIs. | https://support.datacite.org/docs/usage-reports-api-guide |

## Plans / Rate Limits / FinOps

| Resource | File |
|----------|------|
| Plans & Pricing | [plans/datacite-plans-pricing.yml](plans/datacite-plans-pricing.yml) |
| Rate Limits | [rate-limits/datacite-rate-limits.yml](rate-limits/datacite-rate-limits.yml) |
| FinOps | [finops/datacite-finops.yml](finops/datacite-finops.yml) |

**Pricing Model:** Freemium. Public read access is free. DOI registration requires institutional membership. Annual membership fee of EUR 2,000 (direct/consortium lead) plus shared infrastructure fee (EUR 200–700 for non-profits; revenue-based for commercial). High-volume overage fees apply above 100,000 DOIs/year.

**Rate Limits Summary:**
- Authenticated: 3,000 requests / 5 min / IP
- Identified (email): 1,000 requests / 5 min / IP
- Public (anonymous): 500 requests / 5 min / IP
- HTTP 429 returned when limit exceeded

## Timestamps

- Created: 2026-06-12
- Modified: 2026-06-12

## Common Properties

| Type | URL |
|------|-----|
| Website | https://datacite.org |
| Documentation | https://support.datacite.org |
| GitHub Organization | https://github.com/datacite |
| LinkedIn | https://www.linkedin.com/company/datacite/ |
| Blog | https://datacite.org/blog/ |
| Pricing | https://datacite.org/fees/ |
| Status Page | https://status.datacite.org/ |
| X / Twitter | https://x.com/DataCite |
| Best Practices | https://support.datacite.org/docs/best-practices-for-integrators |
| Upcoming Changes | https://support.datacite.org/docs/upcoming-changes |

## Maintainers

- Kin Lane / kin@apievangelist.com
