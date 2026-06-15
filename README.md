# Itron (itron)

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

**APIs.json:** [https://github.com/api-evangelist/itron](https://github.com/api-evangelist/itron)

## Scope

- **Type:** Index

## Tags

- Itron
- Utilities
- Smart Meters
- Smart Grid
- Smart Cities
- Internet Of Things
- IoT
- Energy
- Water
- Gas
- Electricity
- Distributed Intelligence
- Grid Edge
- AMI
- AMR
- RF Mesh
- IPv6
- OData
- Industrial IoT
- Fortune 1000
- NASDAQ ITRI

## Timestamps

- **Created:** 2026-05-22
- **Modified:** 2026-05-23

## APIs

### Itron Distributed Intelligence (DI) Platform

Partner-gated platform for building purpose-built applications that execute on
Itron-DI-enabled electric meters at the grid edge. Itron describes DI as moving
"grid analysis, decision-making and control to the grid's edge, resulting in
significantly reduced latency, greatly improved situational awareness, more
accurate analysis and advanced event detection." A DI SDK (request-gated) and
a Third-Party Gateway REST API support the build/sign/deploy/enroll lifecycle.

- **Human URL:** [https://na.itron.com/developers/distributed-intelligence](https://na.itron.com/developers/distributed-intelligence)
- **Base URL:** `https://partner.itron.com/`

#### Tags

- Distributed Intelligence
- Grid Edge
- Smart Meters
- Edge Computing
- Partner Platform

#### Properties

- [Documentation](https://na.itron.com/developers/distributed-intelligence)
- [SDK](https://docs.itrontotal.com/DI_SDK/Content/Topics/Request%20SDK%20files.htm)
- [Developer Portal](https://na.itron.com/developers/itron-developer-program)
- [Sign Up](https://partner.itron.com/flow/af4b0f91-1acd-4c07-9425-7fb4c31ac22b)
- [Use Cases](https://na.itron.com/w/unlock-your-iot-potential-with-itron-di-developer-program)
- [Blog](https://na.itron.com/w/unlock-your-iot-potential-with-itron-di-developer-program)
- [Postman Collection](collections/starfish-data-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/starfish-data-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Itron Intelligent Connectivity (IC) Platform

The IC platform combines Itron's IPv6-enabled RF mesh Network Platform with a
Control Platform that manages the lifecycle of connected devices. Itron describes
it as "an open, standards-based IPv6-enabled wireless network that provides
unsurpassed, ubiquitous coverage," with Access Points supporting thousands of
devices at data rates up to 2.4 Mbps. Developers integrate via the Network
Interface Card (NIC) or Edge Router. Underlying CoAP sample apps and the
Milli5 sensor reference designs are published in the Itron Networked Solutions
GitHub org.

- **Human URL:** [https://na.itron.com/developers/intelligent-connectivity](https://na.itron.com/developers/intelligent-connectivity)
- **Base URL:** `https://partner.itron.com/`

#### Tags

- Intelligent Connectivity
- RF Mesh
- IPv6
- CoAP
- IIoT
- Network Platform

#### Properties

- [Documentation](https://na.itron.com/developers/intelligent-connectivity)
- [Sign Up](https://partner.itron.com/flow/af4b0f91-1acd-4c07-9425-7fb4c31ac22b)
- [GitHub Organization](https://github.com/silverspringnetworks)
- [Code Examples](https://github.com/silverspringnetworks/developer_program)
- [Postman Collection](collections/starfish-data-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/starfish-data-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Itron Starfish Data Platform API

REST-based device-and-observation API inherited from the Silver Spring Networks
acquisition, now branded under Itron Networked Solutions. Exposes Devices,
Observations, and Device Templates resources with OAuth 2.0 client-credentials
authentication, plus a short-lived browser token flow via the Tokens API.
A first-party JavaScript SDK (`starfish-sdk` on npm) wraps all operations.
This is the only Itron API with a publicly published SDK and README-grade
reference material; the spec below is reconstructed from the SDK source.

- **Human URL:** [https://developer.ssni.com/api-overview](https://developer.ssni.com/api-overview)
- **Base URL:** `https://api.data.sentience.ssni.com/`

#### Tags

- Starfish
- Silver Spring Networks
- Data Platform
- IoT
- Devices
- Observations
- OAuth

#### Properties

- [OpenAPI](openapi/starfish-data-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/starfish-data-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/starfish-data-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [SDK](https://github.com/silverspringnetworks/starfish-js)
- [API Reference](https://developer.ssni.com/api-overview)
- [Documentation](https://developer.ssni.com/api-overview)
- [GitHub Repository](https://github.com/silverspringnetworks/starfish-js)
- [Code Examples](https://github.com/silverspringnetworks/starfish-js#readme)
- [Authentication](https://developer.ssni.com/api-overview)

### Itron Analytics Data Warehouse API

REST-based OData 4.0 query API exposing the Itron Analytics data warehouse for
Itron Enterprise Edition / IA Platform tenants. Authentication uses a JWT
obtained from the Itron Identity Service with a 36-character ClientID and a
32-character Client Secret. The service documents protections that "will limit
the result set to 10,000 records if there are not filters in the request" and
supports OData filter/select/expand semantics over interval reads, accounts,
service points, and related entities.

- **Human URL:** [https://docs.itrontotal.com/IAPlatform/Cloud/AdminPortal/help/Content/DataWarehouseAPI.htm](https://docs.itrontotal.com/IAPlatform/Cloud/AdminPortal/help/Content/DataWarehouseAPI.htm)
- **Base URL:** `https://docs.itrontotal.com/IAPlatform/`

#### Tags

- Itron Analytics
- Data Warehouse
- OData
- Reporting
- Itron Enterprise Edition

#### Properties

- [Documentation](https://docs.itrontotal.com/IAPlatform/Cloud/AdminPortal/help/Content/DataWarehouseAPI.htm)
- [Authentication](https://docs.itrontotal.com/IAPlatform/Cloud/AdminPortal/help/Content/DataWarehouseAPI.htm)
- [Rate Limits](https://docs.itrontotal.com/IAPlatform/Cloud/AdminPortal/help/Content/DataWarehouseAPI.htm)
- [Postman Collection](collections/starfish-data-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/starfish-data-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Itron Third-Party Gateway API

REST/JSON API that enables utility customer portals to enroll consumers into
Distributed Intelligence (DI) programs by forwarding requests into the Itron
Enterprise Application Center (EAC) and orchestrating service-bus queues for
request/response/notification handling, application downloads, and licensing.
Authentication uses Itron Identity client credentials and an AAA
(authentication, authorization, accounting) framework.

- **Human URL:** [https://docs.itrontotal.com/ThirdPartyGWAPI/Content/Topics/IntroMod.htm](https://docs.itrontotal.com/ThirdPartyGWAPI/Content/Topics/IntroMod.htm)
- **Base URL:** `https://docs.itrontotal.com/ThirdPartyGWAPI/`

#### Tags

- Third Party Gateway
- Distributed Intelligence
- Enrollment
- EAC
- Customer Portal

#### Properties

- [Documentation](https://docs.itrontotal.com/ThirdPartyGWAPI/Content/Topics/IntroMod.htm)
- [Authentication](https://docs.itrontotal.com/ThirdPartyGWAPI/Content/Topics/IntroMod.htm)
- [Postman Collection](collections/starfish-data-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/starfish-data-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Itron IEE Web Services

Legacy web-service surface for Itron Enterprise Edition (IEE) Meter Data
Management. Documented as a mix of WCF services (with annotated WSDL and XSD
files shipped in the installation's `bin\ServiceMetadata` directory) and older
.asmx ASP.NET web services. Per-service PDF API guides are distributed through
the gated Itron Customer Center rather than a public developer portal.

- **Human URL:** [https://docs.itrontotal.com/IEEOtherAPI/Content/Topics/Service%20Documentation.htm](https://docs.itrontotal.com/IEEOtherAPI/Content/Topics/Service%20Documentation.htm)
- **Base URL:** `https://docs.itrontotal.com/IEEOtherAPI/`

#### Tags

- IEE
- Itron Enterprise Edition
- MDM
- SOAP
- WCF
- WSDL
- Legacy

#### Properties

- [Documentation](https://docs.itrontotal.com/IEEOtherAPI/Content/Topics/Service%20Documentation.htm)
- [API Reference](https://customer.itron.com/)
- [Postman Collection](collections/starfish-data-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/starfish-data-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Itron Consumer Energy Stream (CES) API

Itron describes Consumer Energy Stream as a data product that allows electricity
meter consumption data "from a consumer's meter to stream to an Itron-authenticated
receiver over the consumer's internet connection and wireless network to a
utility's consumer application and third-party data subscribers who offer products
and services to consumers." CES is delivered as a component of the Intelligent
Edge Operating System (IEOS) and exposes its own APIs documented inside the
Itron Total help center.

- **Human URL:** [https://docs.itrontotal.com/CES_API/Content/Topics/Intro_CES.htm](https://docs.itrontotal.com/CES_API/Content/Topics/Intro_CES.htm)
- **Base URL:** `https://docs.itrontotal.com/CES_API/`

#### Tags

- Consumer Energy Stream
- CES
- IEOS
- Consumer Data
- Streaming
- Smart Meters

#### Properties

- [Documentation](https://docs.itrontotal.com/CES_API/Content/Topics/Intro_CES.htm)
- [API Reference](https://docs.itrontotal.com/CES_API/Content/Topics/Intro_CES.htm)
- [Postman Collection](collections/starfish-data-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/starfish-data-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Itron GenX / Starfish Studio

GenX is the marketing umbrella under which Itron positions next-generation
grid-edge solutions for developer partners; Starfish Studio is a related
sandbox/prototyping surface for IoT solution builders. As of May 2026 the
Starfish Studio landing page (na.itron.com/developers/starfish-studio) returns
a 404, and program details — sample apps, sandboxes, certifications — are
accessible only after partner-program acceptance.

- **Human URL:** [https://na.itron.com/developers/itron-developer-program](https://na.itron.com/developers/itron-developer-program)
- **Base URL:** `https://partner.itron.com/`

#### Tags

- GenX
- Starfish Studio
- Prototyping
- Sandbox
- Partner Program

#### Properties

- [Developer Portal](https://na.itron.com/developers/itron-developer-program)
- [Sign Up](https://partner.itron.com/flow/af4b0f91-1acd-4c07-9425-7fb4c31ac22b)
- [Postman Collection](collections/starfish-data-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/starfish-data-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://na.itron.com/)
- [Developer Portal](https://na.itron.com/developers/)
- [Documentation](https://docs.itrontotal.com/)
- [Knowledge Center](https://customer.itron.com/)
- [Sign Up](https://partner.itron.com/flow/af4b0f91-1acd-4c07-9425-7fb4c31ac22b)
- [Authentication](https://docs.itrontotal.com/IAPlatform/Cloud/AdminPortal/help/Content/DataWarehouseAPI.htm)
- [GitHub Organization](https://github.com/silverspringnetworks)
- [GitHub Repository](https://github.com/silverspringnetworks/starfish-js)
- [GitHub Repository](https://github.com/silverspringnetworks/developer_program)
- [Blog](https://na.itron.com/w)
- [Newsroom](https://na.itron.com/na/company/newsroom)
- [Partners](https://na.itron.com/partners)
- [Customers](https://na.itron.com/who-we-serve)
- [Solutions](https://na.itron.com/na/solutions)
- [LinkedIn](https://www.linkedin.com/company/itron-inc/)
- [X (Twitter)](https://twitter.com/ItronInc)
- [YouTube](https://www.youtube.com/user/itroninc)
- [Glossary](https://apps.itron.com/ItronGlossary/)
- [Investors](https://investors.itron.com/)
- [Plans](plans/itron-plans-pricing.yml)
- [Rate Limits](rate-limits/itron-rate-limits.yml)
- [Fin Ops](finops/itron-finops.yml)
- [Capabilities](capabilities/)
- [Vocabulary](vocabulary/itron-vocabulary.yml)
- [JSON-LD](json-ld/itron-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
