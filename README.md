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

UCSI University is a private, multi-campus university in Kuala Lumpur, Terengganu and Sarawak, Malaysia, established in 1986 and ranked #265 in the QS World University Rankings 2025. This repository catalogs UCSI University's public developer/API footprint as an [APIs.json](https://apisjson.org) profile, under the API Evangelist university pipeline — which settles **who operates** each surface before recording it, because a university is a federation of buyers rather than a producer.

UCSI operates no developer portal, no public API programme, no open data portal, no institutional repository on its own domain, and no verifiable public code. Its entire `ucsiuniversity.edu.my` estate sits behind a Cloudflare bot-management challenge that answers HTTP 403 to every automated client, so nothing it hosts can be read programmatically. Three surfaces were established off-host: a Microsoft Entra ID identity tenant that is the institution's own IdP, a CourseNetworking LMS tenancy, and a ROR registration.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/ucsi/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=ucsi-api-evangelist&utm_content=repo

## Type

- Index
- Consumer
- 3rd-Party
- x-type: university
- x-category: Private Research University

## Tags

Education, Higher Education, University, Private University, Malaysia, Asia, Library, Library Catalog, Koha, Identity Federation, Learning Management, Registry

## Surfaces

Every entry carries an `x-operator` saying who runs the thing it describes.

- **UCSI University Library Catalog (Koha)** — `x-operator: institution`. Koha ILS on UCSI's own host, https://koha.ucsiuniversity.edu.my/. Koha can expose OAI-PMH, ILS-DI and a `/api/v1` REST API; whether UCSI has them enabled is **unverifiable** — Cloudflare returns 403 to automated clients. No OpenAPI is registered, and none was generated.
- **UCSI University Identity Federation (Microsoft Entra ID)** — `x-operator: federation`. Tenant `3c5f2d31-81d8-4455-a2bf-531fbc398144`, FederationBrandName "UCSI University", Managed realm. Signed SAML 2.0 IdP metadata and an OpenID Connect discovery document are publicly retrievable. The strongest programmable surface in this profile; the contract is Microsoft's and is not saved here.
- **UCSI University LMS Tenancy (CourseNetworking)** — `x-operator: tenant`. `lms.ucsiuniversity.edu.my` CNAMEs and 301s to https://ucsi.thecn.com/. The tenancy is UCSI's; the platform and any API are CourseNetworking's.
- **UCSI University ROR Registration** — `x-operator: registry`. https://ror.org/019787q29 — a registration the institution holds, never a contract it operates.

Confirmed absences: no UCSI entity in the eduGAIN metadata aggregate and none in Malaysia's SIFULAN federation; no Crossref member; no DataCite repository client; no verifiable official GitHub organisation.

## Conformance (Kin Score `education` regime)

- [conformance/ucsi-conformance.yml](conformance/ucsi-conformance.yml) — `saml` conformant (Entra ID IdP metadata); `oai-pmh` and `lti` unverifiable; `shibboleth`, `crossref`, `datacite`, `scim`, `oneroster`, `ed-fi`, `caliper`, `qti`, `orcid` not found.
- [authentication/ucsi-authentication.yml](authentication/ucsi-authentication.yml) — the tenant's OIDC and SAML 2.0 endpoints, probed.

## Plans / Rate Limits / FinOps

- [plans/ucsi-plans-pricing.yml](plans/ucsi-plans-pricing.yml)
- [rate-limits/ucsi-rate-limits.yml](rate-limits/ucsi-rate-limits.yml)
- [finops/ucsi-finops.yml](finops/ucsi-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-09-01

## Common Properties

- Website: https://www.ucsiuniversity.edu.my/
- Library Catalog: https://koha.ucsiuniversity.edu.my/
- Identity Federation: https://login.microsoftonline.com/ucsiuniversity.edu.my/v2.0/.well-known/openid-configuration
- LinkedIn: https://www.linkedin.com/school/ucsi-education/
- Conformance: [conformance/ucsi-conformance.yml](conformance/ucsi-conformance.yml)
- Authentication: [authentication/ucsi-authentication.yml](authentication/ucsi-authentication.yml)
- JSON-LD: [json-ld/ucsi-context.jsonld](json-ld/ucsi-context.jsonld)
- Domain Security: [security/ucsi-domain-security.yml](security/ucsi-domain-security.yml)
- Review: [review.yml](review.yml)

## Notes

- **Coverage: unreadable / bot_blocked.** www, lib, koha, iis, apps, alumni, library and m under `ucsiuniversity.edu.my` all return HTTP 403 from Cloudflare (`cf-mitigated: challenge`), with a plain client and again with full Chrome browser headers. The hosts are live for humans; they are unreadable to clients. That is a finding about our access, not a claim that UCSI publishes nothing.
- `api.`, `developer.`, `data.`, `courses.`, `portal.`, `idp.` and `journals.` under `ucsiuniversity.edu.my` have no DNS record at all.
- No endpoints were fabricated and no contract was generated. Every status code in `review.yml` and `apis.yml` `x-coverage` came from a live probe on 2026-09-01.

## Maintainers

- Kin Lane — kin@apievangelist.com
