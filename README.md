# Saildrone (saildrone)

Saildrone is an Alameda, California maritime autonomy company that designs, manufactures, and operates a global fleet of wind/solar-powered autonomous surface vehicles (USVs) for ocean science, maritime domain awareness, and defense applications. Founded in 2012 by Richard Jenkins, the company runs four USV classes — Explorer (23ft environmental sensing), Voyager (33ft MDA and counter-narcotics), Surveyor (65ft deep-ocean mapping), and Spectre (ISR / anti-submarine warfare / kinetic payloads) — and has logged over 2.5M nautical miles and 65,000 days at sea for customers including NOAA, the US Navy (Task Force 59), NASA, EUMETSAT, BOEM, and Lockheed Martin.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/saildrone/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - Maritime, Ocean Data, USV, Unmanned Surface Vehicle, Autonomous Systems, METOC, Maritime Domain Awareness, Anti Submarine Warfare, Defense, Climate, Oceanography, Bathymetry, Biogeochemical

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## Platforms

| Platform | Length | Primary Use |
|---|---|---|
| Saildrone Explorer | 23 ft | Environmental sensing, METOC |
| Saildrone Voyager | 33 ft | Maritime domain awareness, counter-narcotics |
| Saildrone Surveyor | 65 ft | Deep-ocean seafloor mapping |
| Saildrone Spectre | — | ISR / ASW (Silent Endurance) and kinetic (Stealth Strike) |

## APIs

### Saildrone Mission API
Saildrone Public Mission API (BETA). Bearer-token authenticated REST API exposing health, key/secret auth, drone access discovery, and per-mission time-series retrieval across four datasets — vehicle, atmospheric, oceanographic, and biogeochemical. Hosted at `developer-mission.saildrone.com`.

**Human URL:** [https://www.saildrone.com/data-delivery/api](https://www.saildrone.com/data-delivery/api)

- [Documentation](https://www.saildrone.com/data-delivery/api)
- [Swagger UI](https://developer-mission.saildrone.com/api-docs)
- [OpenAPI](openapi/saildrone-mission-api-openapi.yml)
- [JSON Schema — Mission Access](json-schema/saildrone-mission-access-schema.json)
- [JSON Schema — Time Series Record](json-schema/saildrone-mission-time-series-record-schema.json)
- [JSON-LD Context](json-ld/saildrone-context.jsonld)
- [Example — Authenticate](examples/saildrone-authenticate-example.json)
- [Example — List Access](examples/saildrone-list-access-example.json)
- [Example — Get Time Series](examples/saildrone-get-time-series-example.json)
- [Spectral Rules](rules/saildrone-rules.yml)
- [Naftiko Capability — Health](capabilities/mission-health.yaml)
- [Naftiko Capability — Authentication](capabilities/mission-authentication.yaml)
- [Naftiko Capability — Time Series](capabilities/mission-time-series.yaml)

## Datasets

The Mission API returns time-series data in four canonical datasets:

| Dataset | Description |
|---|---|
| `vehicle` | USV telemetry — SOG, COG, HDG, battery voltage, solar input |
| `atmospheric` | METOC atmosphere — air temperature, RH, barometric pressure, wind, waves |
| `oceanographic` | Ocean surface — sea surface temperature, salinity, conductivity |
| `biogeochemical` | BGC — dissolved oxygen, chlorophyll-a, CO2 (dry mole fraction and seawater partial pressure) |

## Mission Portal

The [Saildrone Mission Portal](https://www.saildrone.com/data-delivery/mission-portal) is the secure web command-and-control application bundled with Fully Managed engagements. It delivers live multi-INT visualization (radar tracks, AIS, EO/IR, acoustic, environmental), geofences, on-the-fly retasking, automated alerts, event logging, and mission replay. Public profiling of the Portal's internal API surface is gated; the OpenAPI in this repo covers the public developer-mission.saildrone.com BETA.

## Open Data

Past Saildrone mission data is published openly via:

- [NOAA PMEL Ocean Climate Stations — Saildrone Data Access](https://www.pmel.noaa.gov/ocs/saildrone/data-access)
- [PMEL ERDDAP — Saildrone GTS](https://data.pmel.noaa.gov/generic/erddap/tabledap/saildrone_gts.html)
- Per-mission ERDDAP endpoints (Arctic 2018, TPOS, SWFSC, US Navy Task Force 59, etc.)
- NCEI Ocean Carbon and Acidification Data System (CO2 / pCO2)

Formats include NetCDF (CF/ACDD), CSV, JSON, and Parquet, with DOIs assigned per mission.

## Commercial Surface

- [Plans & Pricing](plans/saildrone-plans-pricing.yml) — Mission-as-a-Service is contract-priced; API access is bundled.
- [Rate Limits](rate-limits/saildrone-rate-limits.yml) — pagination + interval thinning, short-lived bearer tokens.
- [FinOps](finops/saildrone-finops.yml) — FOCUS mapping of MaaS vehicle-day spend.

## Common Links

- [Saildrone Website](https://www.saildrone.com)
- [About / Leadership](https://www.saildrone.com/about)
- [Data Products](https://www.saildrone.com/technology/data)
- [Fully Managed (MaaS)](https://www.saildrone.com/service-model/fully-managed)
- [News](https://www.saildrone.com/news) · [Press](https://www.saildrone.com/press) · [Careers](https://www.saildrone.com/careers) · [Contact](https://www.saildrone.com/contact)
- [GitHub org](https://github.com/Saildrone) · [LinkedIn](https://www.linkedin.com/company/saildrone) · [YouTube](https://www.youtube.com/@saildrone)
