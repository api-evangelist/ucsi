# UCSI University (ucsi)

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
