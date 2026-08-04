# UCSI University (ucsi)

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

UCSI University is a private, multi-campus university in Malaysia (Kuala Lumpur, Terengganu and Sarawak), ranked #265 in the QS World University Rankings 2025. This repository catalogs UCSI University's public developer/API footprint as an [APIs.json](https://apisjson.org) profile. UCSI does not publish a public developer portal or documented, openly accessible APIs; the systems that exist (student portal, mobile-app backends, identity, and a Koha library catalog) are gated behind authentication and a web application firewall.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/ucsi/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=ucsi-api-evangelist&utm_content=repo

## Type

- Index
- Consumer
- 3rd-Party

## Tags

Education, Higher Education, University, Malaysia, Library, Koha

## APIs

- **UCSI University Library Catalog (Koha)** — Koha-based library OPAC at https://koha.ucsiuniversity.edu.my/. Koha can expose OAI-PMH and ILS-DI / REST web services, but no public endpoint could be confirmed as enabled during review. Docs: https://lib.ucsiuniversity.edu.my/

No public developer portal or documented APIs were found beyond the gated/library systems above.

## Plans

- [plans/ucsi-plans-pricing.yml](plans/ucsi-plans-pricing.yml)

## Rate Limits

- [rate-limits/ucsi-rate-limits.yml](rate-limits/ucsi-rate-limits.yml)

## FinOps

- [finops/ucsi-finops.yml](finops/ucsi-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.ucsiuniversity.edu.my/
- LinkedIn: https://www.linkedin.com/school/ucsi-education/
- Plans: [plans/ucsi-plans-pricing.yml](plans/ucsi-plans-pricing.yml)
- Rate Limits: [rate-limits/ucsi-rate-limits.yml](rate-limits/ucsi-rate-limits.yml)
- FinOps: [finops/ucsi-finops.yml](finops/ucsi-finops.yml)
- Review: [review.yml](review.yml)

## Notes

- Verification caveats: The official website (https://www.ucsiuniversity.edu.my/), Library Services (https://lib.ucsiuniversity.edu.my/), and Koha catalog (https://koha.ucsiuniversity.edu.my/) are all live in a browser but return HTTP 403 to automated requests due to a web application firewall.
- Potential Koha OAI-PMH, ILS-DI, and REST endpoints were probed but could not be confirmed as publicly enabled (all returned 403).
- No official UCSI University GitHub organization was found.
- No endpoints were fabricated; only confirmed URLs are listed.

## Maintainers

- Kin Lane — kin@apievangelist.com
