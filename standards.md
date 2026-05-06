# Standards & API Reference

> Project: Transportation Management System (TMS) · Generated: 2026-05-03

## Industry Standards & Specifications

### ISO Standards

| Standard | Title | URL | Relevance |
|----------|-------|-----|-----------|
| ISO 9001:2015 | Quality Management Systems | https://www.iso.org/standard/62085.html | Governs process quality for logistics providers; TMS workflows for order management, on-time delivery, and customer communication should be designed to support ISO 9001 compliance audits. |
| ISO 14001:2015 | Environmental Management Systems | https://www.iso.org/standard/60857.html | Requires organisations to measure and reduce environmental impact; TMS carbon-footprint reporting and modal-shift recommendations directly support ISO 14001 compliance. |
| ISO 28000:2022 | Security Management Systems for the Supply Chain | https://www.iso.org/standard/79612.html | Defines risk management requirements covering theft, terrorism, and sabotage across logistics networks. TMS security frameworks for carrier vetting and data access should align with this standard. |
| ISO 45001:2018 | Occupational Health and Safety Management | https://www.iso.org/standard/63787.html | Governs driver and warehouse staff safety requirements; relevant to TMS HOS (hours-of-service) tracking and compliance modules. |
| ISO 22301:2019 | Business Continuity Management | https://www.iso.org/standard/75106.html | Covers resilience planning for logistics disruptions; informs TMS exception management and alternative-routing features. |
| ISO/IEC 27001:2022 | Information Security Management | https://www.iso.org/standard/27001 | The primary information-security standard; TMS platforms handling carrier contracts, pricing, and PII must demonstrate compliance, particularly for enterprise sales. |
| ISO 23355 | Visibility Data Exchange between Logistics Information Service Providers (draft) | https://www.iso.org/standard/75326.html | Emerging standard aiming to establish interoperable data connections between logistics information system (LISS) networks; will directly govern how TMS platforms share visibility data across ecosystems. |

### W3C & IETF Standards

| Standard | URL | Relevance |
|----------|-----|-----------|
| RFC 7231 — HTTP/1.1 Semantics | https://datatracker.ietf.org/doc/html/rfc7231 | Defines HTTP methods (GET, POST, PUT, DELETE, PATCH) and status codes used by all TMS REST APIs. |
| RFC 6749 — OAuth 2.0 | https://datatracker.ietf.org/doc/html/rfc6749 | The authorisation framework used by all major TMS platforms (Oracle OTM, SAP TM, Trimble TruckMate, project44) for API access delegation. |
| RFC 6750 — OAuth 2.0 Bearer Token Usage | https://datatracker.ietf.org/doc/html/rfc6750 | Defines how Bearer tokens are transmitted in API calls; implemented by all TMS platforms using OAuth 2.0 (e.g. TruckMate passes Bearer tokens in the Authorization header). |
| RFC 7519 — JSON Web Token (JWT) | https://datatracker.ietf.org/doc/html/rfc7519 | Defines the JWT format used in OAuth 2.0 and OpenID Connect token exchanges; directly relevant to TMS API authentication flows. |
| OpenID Connect 1.0 | https://openid.net/specs/openid-connect-core-1_0.html | Identity layer over OAuth 2.0 providing user authentication and SSO; used by enterprise TMS deployments for single-sign-on with corporate identity providers. |
| RFC 4180 — CSV Format | https://datatracker.ietf.org/doc/html/rfc4180 | Widely used flat-file format for TMS batch imports/exports of shipment data, carrier rates, and audit records. |
| W3C JSON-LD 1.1 | https://www.w3.org/TR/json-ld11/ | Linked-data format used by IATA ONE Record for air cargo data exchange; relevant to TMS air freight and multimodal modules. |

### Data Model & API Specifications

| Specification | URL | Relevance |
|---------------|-----|-----------|
| OpenAPI Specification 3.1 | https://spec.openapis.org/oas/v3.1.0.html | The industry standard for documenting REST APIs; all major TMS vendors (Oracle, SAP, Trimble, project44) publish OpenAPI-compliant API specifications. |
| ANSI X12 EDI Standards | https://x12.org/products/transaction-sets | The dominant North American EDI standard for carrier integration. Key transaction sets: 204 (Motor Carrier Load Tender), 210 (Freight Invoice), 214 (Shipment Status), 990 (Response to Load Tender), 856 (Advance Ship Notice), 997 (Functional Acknowledgment). |
| UN/EDIFACT | https://unece.org/trade/uncefact/introducing-unedifact | UN-defined EDI standard dominant in Europe and international trade; covers equivalent freight and customs message types. TMS platforms targeting global markets must support both X12 and EDIFACT. |
| GS1 EPCIS 2.0 | https://www.gs1.org/standards/epcis | Event-based visibility standard capturing "what, when, where, why" of shipment events using GTINs and SSCCs. EPCIS 2.0 adds REST/JSON-LD support alongside legacy SOAP/XML. Enables interoperable track-and-trace across TMS, WMS, and carrier systems. |
| GS1 Core Business Vocabulary (CBV) | https://www.gs1.org/standards/epcis | Companion to EPCIS defining standardised business step and disposition codes (e.g. "in_transit", "arrived", "departed"); ensures consistent event semantics across trading partners. |
| Open Trip Model 5 (OTM5) | https://opentripmodel.org/ | Open-source REST/JSON data model for real-time logistics trip data exchange. Mandates JSON (no XML), REST architecture, and follows OpenAPI specification. Gaining adoption in European logistics. |
| IATA ONE Record | https://www.iata.org/en/programs/cargo/e/one-record/ | Air cargo data-sharing standard replacing legacy Cargo IMP and XML systems; became the preferred standard for air cargo data sharing from January 2026. Uses JSON-LD and REST APIs with a federated trust network for authentication. |
| NMFC (National Motor Freight Classification) | https://www.nmfta.org/ | Governs LTL freight commodity classification and rating in North America; TMS LTL rating engines must reference NMFC codes for accurate rate shopping. |
| Incoterms 2020 | https://iccwbo.org/business-solutions/incoterms-rules/incoterms-2020/ | ICC-defined international trade terms (EXW, FOB, CIF, DAP, etc.) governing risk transfer and freight responsibility; embedded in TMS shipment configuration for cross-border shipments. |

### Security & Authentication Standards

| Standard | URL | Relevance |
|----------|-----|-----------|
| OAuth 2.0 (RFC 6749/6750) | https://datatracker.ietf.org/doc/html/rfc6749 | Primary authorisation protocol for TMS API access; Client Credentials flow for machine-to-machine integration, Authorization Code flow for user-delegated access. |
| OpenID Connect 1.0 | https://openid.net/developers/how-connect-works/ | Authentication layer for enterprise SSO; required for TMS deployments integrated with corporate identity providers (Azure AD, Okta, Google Workspace). |
| OWASP API Security Top 10 | https://owasp.org/www-project-api-security/ | Reference for API security best practices; TMS APIs handling carrier contracts and rate data are high-value targets — broken object-level authorisation (BOLA) is the most common vulnerability class. |
| TLS 1.3 (RFC 8446) | https://datatracker.ietf.org/doc/html/rfc8446 | Mandatory transport encryption for all TMS API communications; older versions (TLS 1.0, 1.1) must be disabled. |
| NIST SP 800-53 | https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final | US federal security control framework; relevant for TMS platforms serving government shippers or defence logistics. |
| GDPR (EU 2016/679) | https://gdpr-info.eu/ | EU data regulation; TMS platforms handling European shipment data (driver PII, consignee addresses) must implement data minimisation, right-to-erasure, and cross-border transfer controls. |

### MCP Server Specifications

The Model Context Protocol (MCP) is not yet standardised within the TMS industry. However, AI-native TMS platforms could expose MCP-compatible servers to allow LLM agents to query shipment status, trigger routing re-optimisation, and retrieve carrier capacity in real time. Key reference:

- **MCP Specification**: https://modelcontextprotocol.io/specification — Defines the protocol for tool/resource exposure to LLM agents; a TMS MCP server could provide tools such as `get_shipment_status`, `reroute_shipment`, `get_carrier_rates`, and `query_eld_position`.

---

## Similar Products — Developer Documentation & APIs

### Oracle Transportation Management (OTM)

- **Description:** Enterprise TMS covering multi-modal planning, freight audit, carrier management, and global trade compliance. Part of Oracle Logistics Cloud.
- **API Documentation:** https://docs.oracle.com/en/cloud/saas/transportation/26b/otmol/index.html
- **REST API Reference:** https://docs.oracle.com/en/cloud/saas/transportation/24c/otmra/Quick_Start.html
- **Developer Guide:** https://docs.oracle.com/cd/E65625_01/nav/otm.htm (on-premise); https://docs.oracle.com/en/cloud/saas/transportation/26b/index.html (cloud)
- **Standards:** REST/JSON, OpenAPI; supports EDI X12, EDIFACT, and GS1 EPCIS integrations
- **Authentication:** OAuth 2.0 (Client Credentials and Authorization Code flows)

### SAP Transportation Management (SAP TM / SAP Cloud Transport Management)

- **Description:** TMS integrated with SAP S/4HANA for transportation planning, carrier tendering, dock scheduling, and freight-cost settlement.
- **API Documentation:** https://api.sap.com/package/TmsForCloudPub/rest
- **SAP Business Accelerator Hub:** https://api.sap.com/api/TMS_v2/resource
- **Developer Guide:** https://help.sap.com/docs/SAP_S4HANA_CLOUD/61e246f4b34c4e1790d8b7651c0b40a8/6486beeb38114fdc94261ef2829d5b03.html
- **Standards:** REST/JSON, OpenAPI 3.0; deep SAP BTP integration; supports EDI X12 and EDIFACT
- **Authentication:** OAuth 2.0 (Client Credentials); token obtained via SAP BTP service binding

### Trimble TruckMate

- **Description:** Carrier-focused TMS for truckload and LTL operations including dispatch, operations, and accounting. Three REST APIs: TruckMate API (business data), Master Data API (configuration), Finance API (invoicing).
- **API Documentation:** https://developer.trimble.com/docs/truckmate/
- **API Reference (OpenAPI):** https://developer.trimble.com/docs/truckmate/reference/openapi/truckmate/
- **SDKs/Libraries:** Client libraries for Java and C# available through the developer portal
- **Developer Guide:** https://developer.trimble.com/docs/truckmate/guides/access/
- **Standards:** REST/JSON, OpenAPI; hundreds of endpoints covering orders, trips, reports, driver profiles, invoices
- **Authentication:** OAuth 2.0 Bearer Token (passed as Authorization header)

### project44

- **Description:** Multi-modal real-time supply chain visibility platform providing ETA predictions, exception management, and carrier connectivity across truckload, LTL, ocean, air, and rail.
- **API Documentation:** https://developers.project44.com/api-reference
- **Developer Portal:** https://developers.project44.com/
- **SDKs/Libraries:** Java and C# client libraries provided
- **Developer Guide:** https://developers.project44.com/guides/shippers/visibility/ftl
- **Standards:** REST/JSON (API v4, not backward compatible with v3); OpenAPI-documented
- **Authentication:** OAuth 2.0 (Bearer Token); dedicated per-environment credentials

### Descartes MacroPoint

- **Description:** Real-time freight visibility and predictive ETA platform for shippers, brokers, and 3PLs. Integrates with TMS via REST API or SFTP flat-file.
- **Customer Integration Docs:** https://docs.macropoint.com/
- **Carrier Integration Docs:** https://carrierdocs.macropoint.com/
- **Capacity Integration Docs:** https://capacitydocs.macropoint.com/
- **Standards:** REST/XML (legacy); Base URL: `https://macropoint-lite.com/api/1.0/`; also supports SFTP/FTPS flat-file uploads
- **Authentication:** Basic Authentication

### FourKites

- **Description:** AI-powered predictive supply chain visibility platform for Fortune 500 shippers and 3PLs. Provides real-time shipment tracking across modes with predictive ETAs.
- **Developer Portal:** https://developer.fourkites.com/
- **GitHub (examples):** https://github.com/FourKites/Tracking-Information-Assignment-API
- **Developer Guide:** https://fourkites.my.site.com/publicKB/s/tms-locations-api-integration
- **Standards:** REST/JSON; webhook-based event delivery for shipment status updates
- **Authentication:** Basic / Digest authentication; API key management via portal

### Flexport

- **Description:** Digital freight forwarder and supply chain platform covering ocean, air, truck, and customs. REST API enables TMS integration for purchase orders, shipments, and freight invoices.
- **Developer Portal:** https://developers.flexport.com/
- **API Reference:** https://apidocs.flexport.com/
- **Developer Guides:** https://developers.flexport.com/tutorials/purchase-order-api-tutorial/
- **Standards:** REST/JSON; supports EDI X12 and EDIFACT for TMS integrations
- **Authentication:** OAuth 2.0 (API credentials via developer portal)

### MercuryGate (Infios) TMS

- **Description:** Mid-market SaaS TMS covering routing, carrier management, freight audit, and load optimisation. Offers a Booking API accepting rate requests and returning rate lists.
- **API Documentation:** https://qa-api-docs.mercurygate.net/documentation/
- **Standard Data Codes:** https://qa-api-docs.mercurygate.net/documentation/standard-data.html
- **Standards:** REST; OAuth Authorization Code flow for partner integrations
- **Authentication:** OAuth 2.0 (Authorization Code flow)

### Transporeon

- **Description:** Trimble-owned transport management and procurement platform connecting shippers and carriers; specialises in freight sourcing, time-slot management, and transport execution.
- **Developer Portal:** https://transporeon-hcskb.atlassian.net/wiki/spaces/ADPD
- **API Documentation:** https://transporeon-hcskb.atlassian.net/wiki/spaces/ADPD/pages/27231708/Documentation
- **Carrier Slot Booking API:** https://transporeon-hcskb.atlassian.net/wiki/spaces/ADPD/pages/27230328
- **Standards:** REST; JSON; APIs for carriers, freight procurement, rate management, and transport operations
- **Authentication:** OAuth 2.0

### FMCSA QCMobile API (US DOT)

- **Description:** Free US government REST API providing carrier safety data including BASIC scores, out-of-service rates, crash records, inspection history, and operating authority status.
- **Developer Portal:** https://mobile.fmcsa.dot.gov/
- **API Access Guide:** https://mobile.fmcsa.dot.gov/QCDevsite/docs/apiAccess
- **Standards:** REST; API key (WebKey) appended as query parameter
- **Authentication:** API Key (requires Login.gov account registration)
- **Notes:** TMS carrier vetting and compliance modules should integrate FMCSA data to automate carrier qualification workflows.

---

## Notes

### Emerging and Evolving Areas

1. **ELD API Standardisation Gap**: While FMCSA mandates ELD usage, there is no single standardised API specification for ELD data exchange. Each provider (Geotab, Verizon Connect, BigRoad, Samsara) exposes its own REST API. TruckerCloud and similar aggregation platforms provide a normalised layer, but an open ELD API standard does not yet exist.

2. **IATA ONE Record Adoption Ramp**: ONE Record became the preferred standard for air cargo data sharing from January 1, 2026. As of early 2026, adoption is accelerating with major carriers (Cathay, Lufthansa) in production. TMS platforms with air freight modules should prioritise ONE Record integration over legacy Cargo IMP/XML.

3. **Open Trip Model (OTM5) in Europe**: OTM5 is gaining traction in Dutch and broader European logistics as a standardised REST/JSON data model for trip data exchange. It is not yet widely adopted outside Europe but represents the direction for open TMS data interoperability.

4. **AI and MCP Integration**: The emergence of the Model Context Protocol (MCP) creates an opportunity for TMS platforms to expose structured tool interfaces to LLM agents. No TMS vendor currently publishes an MCP server, representing a first-mover opportunity for an AI-native TMS.

5. **ISO 23355 (LISS Interoperability)**: This forthcoming ISO standard for logistics information system interoperability will directly affect how TMS platforms share visibility data. Monitoring this standard's development is advisable for architecture decisions around data federation.
