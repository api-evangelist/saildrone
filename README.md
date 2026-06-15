# Saildrone (saildrone)

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
