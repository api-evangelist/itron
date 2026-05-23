# itron

API Evangelist network profile for **Itron, Inc.** (NASDAQ: ITRI) — Liberty Lake, Washington–based industrial technology company providing smart-meter, grid-edge, and IoT infrastructure to electric, gas, and water utilities and cities. Self-described mission: *"Creating a more resourceful world."* Reported scale: **7,700+ customers in 100+ countries**, **310M+ communicating endpoints delivered**, **112M+ endpoints under management**. Fortune 1000 (rank 870).

This repository indexes Itron's public API and developer surface for the API Evangelist network. The Itron developer ecosystem is partner-gated (sign-in flow at `partner.itron.com`) rather than self-serve, so most spec material is reconstructed from the public SDK and documentation portals.

## APIs documented (8)

| API | Description | Public Surface |
|---|---|---|
| **Distributed Intelligence (DI) Platform** | Edge apps that run on Itron smart meters at the grid edge. | Partner-gated SDK |
| **Intelligent Connectivity (IC) Platform** | IPv6 RF mesh network + control software; NIC / Edge Router / Access Points. | Partner-gated + CoAP sample apps on GitHub |
| **Starfish Data Platform API** | REST device/observation API inherited from Silver Spring Networks. | OpenAPI 3.1 reconstructed in `openapi/`; JS SDK on GitHub |
| **Itron Analytics Data Warehouse API** | OData 4.0 query API over the IA Platform warehouse, JWT auth. | Public docs (`docs.itrontotal.com`) |
| **Third-Party Gateway API** | REST/JSON bridge from utility customer portals into DI enrollment via the EAC. | Public docs |
| **IEE Web Services** | Legacy WCF / `.asmx` MDM web services bundled with Itron Enterprise Edition. | Gated PDF guides |
| **Consumer Energy Stream (CES) API** | Streaming consumer-meter data product on the IEOS edge OS. | Public intro docs |
| **GenX / Starfish Studio** | Umbrella for next-gen developer platforms; details gated behind partner program. | Marketing only |

## Repository layout

```
itron/
├── apis.yml                        # Network registry entry — every API + common properties
├── README.md                       # This file
├── openapi/
│   └── starfish-data-platform-openapi.yml
├── json-schema/
│   ├── starfish-device-schema.json
│   ├── starfish-observation-schema.json
│   └── starfish-device-template-schema.json
├── json-structure/
│   └── starfish-data-platform-structure.json
├── json-ld/
│   └── itron-context.jsonld
├── examples/
│   ├── starfish-list-devices-example.json
│   ├── starfish-post-observation-example.json
│   ├── starfish-query-observations-example.json
│   ├── starfish-device-template-example.json
│   └── starfish-token-request-example.json
├── rules/
│   └── starfish-data-platform-rules.yml
├── capabilities/
│   ├── shared/
│   │   └── starfish-data-platform.yaml
│   ├── iot-device-onboarding.yaml
│   └── grid-edge-observation-pull.yaml
├── vocabulary/
│   └── itron-vocabulary.yml
├── plans/
│   └── itron-plans-pricing.yml
├── rate-limits/
│   └── itron-rate-limits.yml
└── finops/
    └── itron-finops.yml
```

## Key links

- Developer Program: <https://na.itron.com/developers/itron-developer-program>
- DI for developers: <https://na.itron.com/developers/distributed-intelligence>
- IC for developers: <https://na.itron.com/developers/intelligent-connectivity>
- Starfish JS SDK: <https://github.com/silverspringnetworks/starfish-js>
- Networked Solutions developer repo (Milli5, CoAP, Edge Router samples): <https://github.com/silverspringnetworks/developer_program>
- Data Warehouse API (OData): <https://docs.itrontotal.com/IAPlatform/Cloud/AdminPortal/help/Content/DataWarehouseAPI.htm>
- Third-Party Gateway API: <https://docs.itrontotal.com/ThirdPartyGWAPI/Content/Topics/IntroMod.htm>
- IEE web services overview: <https://docs.itrontotal.com/IEEOtherAPI/Content/Topics/Service%20Documentation.htm>
- Partner application: <https://partner.itron.com/flow/af4b0f91-1acd-4c07-9425-7fb4c31ac22b>

## Notable findings

- The only publicly published Itron SDK is **`starfish-sdk`** (npm), targeting the Silver Spring Networks-era Data Platform. The DI SDK is gated behind a request form.
- The canonical hostname `developer.itron.com` now redirects to `na.itron.com/developers/`.
- The Starfish Studio landing page (`na.itron.com/developers/starfish-studio`) returns **404** as of May 2026; the program persists but the URL has rotted.
- The **`Itron-Idea-Labs`** GitHub org referenced in older material is **404**; the surviving public org is **`silverspringnetworks`** (3 repos).
- Itron Analytics' Data Warehouse API publishes the only quantitative public limit: an unfiltered query is capped at **10,000 records**.

## Notable absences

- No public OpenAPI/Swagger downloads for any Itron API surface.
- No public developer pricing / self-serve plan page.
- No public status page or RSS-style changelog for the developer APIs.
- No first-party CLI for any Itron platform.
- No public AsyncAPI / event-stream specification for CES.
