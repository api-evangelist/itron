# Itron

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

Itron, Inc. (NASDAQ: ITRI) is a Liberty Lake, Washington–based industrial technology
company providing smart-meter, grid-edge, and IoT infrastructure to electric, gas,
and water utilities and cities. Itron's self-described mission is "Creating a more
resourceful world" and the company reports 7,700+ customers in 100+ countries with
310M+ communicating endpoints delivered and 112M+ endpoints under management.

The Itron developer surface is partner-gated rather than self-serve, centered on
three platform families: (1) Distributed Intelligence (DI) — purpose-built apps that
run at the grid edge on Itron smart meters; (2) Intelligent Connectivity (IC) — an
IPv6/RF-mesh network platform (Itron Networks, formerly Cisco IoT FAN); and (3) the
Starfish / Itron Networked Solutions Data Platform — a REST API + JavaScript SDK for
device management and observation data, inherited from the Silver Spring Networks
acquisition. A separate Data Warehouse OData API serves the Itron Analytics product,
a Third-Party Gateway REST API bridges utility customer portals into DI enrollment,
and legacy IEE web services (WCF/SOAP) and Consumer Energy Stream (CES) APIs
document the Itron Enterprise Edition stack.

Public OpenAPI/AsyncAPI artifacts are not published — access to specs, SDKs, and
sandboxes is brokered through partner.itron.com after program acceptance. The
developer.itron.com hostname now redirects to na.itron.com/developers/.

**Areas:** Itron · Utilities · Smart Meter · Smart Grid · Smart Cities · IoT · Energy · Water · Gas · Electricity · Distributed Intelligence · Grid Edge

## Itron on APIs.io

Everything profiled for Itron is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/itron/](https://apis.io/providers/itron/)** — or go straight to one of the APIs or properties below.

### APIs (11)

- [Itron Distributed Intelligence (DI) Platform](https://apis.io/apis/itron/itron-distributed-intelligence-di-platform/) — Partner-gated platform for building purpose-built applications that execute on Itron-DI-enabled electric meters at the grid edge. Itron describes DI as…
- [Itron Intelligent Connectivity (IC) Platform](https://apis.io/apis/itron/itron-intelligent-connectivity-ic-platform/) — The IC platform combines Itron's IPv6-enabled RF mesh Network Platform with a Control Platform that manages the lifecycle of connected devices. Itron…
- [Itron Analytics Data Warehouse API](https://apis.io/apis/itron/itron-analytics-data-warehouse-api/) — REST-based OData 4.0 query API exposing the Itron Analytics data warehouse for Itron Enterprise Edition / IA Platform tenants. Authentication uses a JWT…
- [Itron Third-Party Gateway API](https://apis.io/apis/itron/itron-third-party-gateway-api/) — REST/JSON API that enables utility customer portals to enroll consumers into Distributed Intelligence (DI) programs by forwarding requests into the Itron…
- [Itron IEE Web Services](https://apis.io/apis/itron/itron-iee-web-services/) — Legacy web-service surface for Itron Enterprise Edition (IEE) Meter Data Management. Documented as a mix of WCF services (with annotated WSDL and XSD files…
- [Itron Consumer Energy Stream (CES) API](https://apis.io/apis/itron/itron-consumer-energy-stream-ces-api/) — Itron describes Consumer Energy Stream as a data product that allows electricity meter consumption data "from a consumer's meter to stream to an…
- [Itron GenX / Starfish Studio](https://apis.io/apis/itron/itron-genx-starfish-studio/) — GenX is the marketing umbrella under which Itron positions next-generation grid-edge solutions for developer partners; Starfish Studio is a related…
- [Itron Device Templates API](https://apis.io/apis/itron/itron-device-templates-api/) — Reusable sensor-shape templates for devices.
- [Itron Devices API](https://apis.io/apis/itron/itron-devices-api/) — Device registration, lookup, and querying.
- [Itron Observations API](https://apis.io/apis/itron/itron-observations-api/) — Time-series sensor observation ingest and query.
- [Itron Tokens API](https://apis.io/apis/itron/itron-tokens-api/) — OAuth 2.0 token issuance for browser-suitable, short-lived bearer tokens.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Itron Agentic Access](https://apis.io/agentic-access/itron/itron-agentic-access/)

#### JSON Schema (3)

The data models the API reads and writes.

- [Itron Starfish Device](https://apis.io/schemas/itron/starfish-device/)
- [Itron Starfish Device Template](https://apis.io/schemas/itron/starfish-device-template/)
- [Itron Starfish Observation](https://apis.io/schemas/itron/starfish-observation/)

#### JSON Structure (1)

Data models expressed in JSON Structure.

- [Starfish Data Platform Structure](https://apis.io/json-structure/itron/starfish-data-platform-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Itron Context](https://apis.io/jsonld/itron/itron-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Itron Vocabulary](https://apis.io/vocabularies/itron/itron-vocabulary/)

#### Examples (5)

Example requests and responses.

- [Starfish Device Template Example](https://apis.io/examples/itron/starfish-device-template-example/)
- [Starfish List Devices Example](https://apis.io/examples/itron/starfish-list-devices-example/)
- [Starfish Post Observation Example](https://apis.io/examples/itron/starfish-post-observation-example/)
- [Starfish Query Observations Example](https://apis.io/examples/itron/starfish-query-observations-example/)
- [Starfish Token Request Example](https://apis.io/examples/itron/starfish-token-request-example/)

#### Collections (5)

Postman and Open Collection request collections.

- [Itron Starfish Data Platform Device Templates API](https://apis.io/collections/itron/open-itron-device-templates-api/)
- [Itron Starfish Data Platform Device Templates Devices API](https://apis.io/collections/itron/open-itron-devices-api/)
- [Itron Starfish Data Platform Device Templates Observations API](https://apis.io/collections/itron/open-itron-observations-api/)
- [Itron Starfish Data Platform Device Templates Tokens API](https://apis.io/collections/itron/open-itron-tokens-api/)
- [Itron Starfish Data Platform API](https://apis.io/collections/itron/open-starfish-data-platform/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Itron — jsonschema rules](https://apis.io/rules/itron/itron-jsonschema-spectral-rules/)
- [Itron — starfish data platform rules](https://apis.io/rules/itron/starfish-data-platform-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Itron Authentication](https://apis.io/security/itron/itron-authentication/)
- [Itron Domain Security](https://apis.io/security/itron/itron-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Itron Plans Pricing](https://apis.io/plans/itron/itron-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Itron Rate Limits](https://apis.io/rate-limits/itron/itron-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Itron Finops](https://apis.io/finops/itron/itron-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.itron.com/)
- [Documentation](https://docs.itrontotal.com/)
- [Blog](https://na.itron.com/w)
- [GitHub](https://github.com/silverspringnetworks)

## API Evangelist rating

**Kin Score 40.5** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 67.0 |
| Contract quality | 55.9 |
| Contract governance | 27.3 |
| Operational transparency | 26.3 |
| Developer ergonomics | 47.6 |
| Access clarity | 21.1 |

**Agent readiness 25.3** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | documented (partial credit) |
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
| Pagination Ratio | paginated |
| Operation Distinctiveness | distinct |

**Regulatory alignment 13.9** — Energy & Utilities

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/itron/](https://apis.io/providers/itron/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Itron: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/itron/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
