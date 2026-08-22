# Saildrone (saildrone)

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

Saildrone is an Alameda, California maritime autonomy company that designs, manufactures, and operates a global fleet of wind/solar-powered autonomous surface vehicles (USVs) for ocean science, maritime domain awareness, and defense applications. Founded in 2012 by Richard Jenkins, the company runs four USV classes — Explorer (23ft, environmental sensing), Voyager (33ft, MDA and counter-narcotics), Surveyor (65ft, deep-ocean bathymetric mapping), and the newer Spectre (ISR / anti-submarine warfare / kinetic payloads). Saildrone has logged over 2.5M nautical miles and 65,000 days at sea across customers including NOAA PMEL, NOAA SWFSC, the US Navy (Task Force 59), NASA, EUMETSAT, BOEM, and Lockheed Martin (which invested $50M in October 2025). Saildrone delivers data through two product surfaces — the Saildrone Mission Portal (secure web app for tasking and live multi-INT visualization) and the Saildrone Public Mission API (BETA) at developer-mission.saildrone.com, which exposes key/secret authenticated endpoints for health, drone access discovery, and time-series retrieval across vehicle, atmospheric, oceanographic, and biogeochemical datasets. Open ocean data from past missions is published via NOAA PMEL ERDDAP and NCEI under open-data terms.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/saildrone/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/saildrone/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Provider
- **Access:** 3rd-Party

## Tags

- Maritime
- Ocean Data
- USV
- Unmanned Surface Vehicle
- Autonomous Systems
- METOC
- Maritime Domain Awareness
- Anti Submarine Warfare
- Defense
- Climate
- Oceanography
- Bathymetry
- Biogeochemical

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## APIs

### Saildrone Mission API

Saildrone Public Mission API (BETA). Provides authenticated access via a key/secret bearer flow to per-mission time-series telemetry across the four canonical Saildrone datasets — vehicle, atmospheric, oceanographic, and biogeochemical — plus drone access discovery and a health probe. Hosted at developer-mission.saildrone.com.

- **Human URL:** [https://www.saildrone.com/data-delivery/api](https://www.saildrone.com/data-delivery/api)

#### Tags

- Saildrone
- Mission
- Time Series
- Ocean Data
- METOC

#### Properties

- [Documentation](https://www.saildrone.com/data-delivery/api)
- [Swagger U I](https://developer-mission.saildrone.com/api-docs)
- [OpenAPI](openapi/saildrone-mission-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [JSON Schema](json-schema/saildrone-mission-access-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/saildrone-mission-time-series-record-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/saildrone-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Example](examples/saildrone-authenticate-example.json)
- [Example](examples/saildrone-list-access-example.json)
- [Example](examples/saildrone-get-time-series-example.json)
- [Spectral Rules](rules/saildrone-rules.yml)

## Common Properties

- [Website](https://www.saildrone.com)
- [About](https://www.saildrone.com/about)
- [A P I](https://www.saildrone.com/data-delivery/api)
- [Swagger U I](https://developer-mission.saildrone.com/api-docs)
- [Mission Portal](https://www.saildrone.com/data-delivery/mission-portal)
- [Data Products](https://www.saildrone.com/technology/data)
- [Platform](https://www.saildrone.com/platform/spectre)
- [Platform](https://www.saildrone.com/platform/surveyor)
- [Platform](https://www.saildrone.com/platform/voyager)
- [Platform](https://www.saildrone.com/platform/explorer)
- [Service](https://www.saildrone.com/service-model/fully-managed)
- [Capability](https://www.saildrone.com/capabilities/metocean-survey)
- [News](https://www.saildrone.com/news)
- [Press](https://www.saildrone.com/press)
- [Careers](https://www.saildrone.com/careers)
- [Contact](https://www.saildrone.com/contact)
- [Partner Open Data](https://www.pmel.noaa.gov/ocs/saildrone/data-access)
- [Partner Open Data](https://data.pmel.noaa.gov/generic/erddap/tabledap/saildrone_gts.html)
- [Git Hub](https://github.com/Saildrone)
- [LinkedIn](https://www.linkedin.com/company/saildrone)
- [Twitter](https://twitter.com/saildrone)
- [YouTube](https://www.youtube.com/@saildrone)
- [Plans](plans/saildrone-plans-pricing.yml)
- [Rate Limits](rate-limits/saildrone-rate-limits.yml)
- [Fin Ops](finops/saildrone-finops.yml)
- [Vocabulary](vocabulary/saildrone-vocabulary.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
