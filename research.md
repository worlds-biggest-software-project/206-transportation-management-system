# Transportation Management System (TMS)

> Candidate #206 · Researched: 2026-05-02

## Existing Products and Software Packages

| Tool | Description | Type | Pricing | Strengths / Weaknesses |
|------|-------------|------|---------|------------------------|
| Oracle Transportation Management (OTM) | Enterprise TMS covering multi-modal planning, execution, freight audit, and carrier management | SaaS / On-premise | From $450/month | Strength: broadest mode coverage (air, ocean, rail, road); Weakness: complex implementation, Oracle-ecosystem dependency |
| SAP Transportation Management (SAP TM) | TMS integrated with SAP ERP for transportation planning, carrier tendering, and dock scheduling | SaaS | Custom quote | Strength: deep SAP ERP integration, strong dock/yard management; Weakness: high cost, slow to deploy |
| Manhattan Active Transportation | Cloud-native TMS with AI-driven route optimisation, carrier management, and load planning | SaaS | Custom quote | Strength: 8× Gartner Magic Quadrant Leader; Weakness: enterprise price point |
| Uber Freight TMS (formerly Transplace) | North America-focused TMS with managed transportation services and carrier network access | SaaS | Custom quote | Strength: large carrier network, competitive TCO; Weakness: primarily North American |
| MercuryGate (Infios) | Mid-market TMS covering routing, optimisation, carrier management, and freight audit | SaaS | Transaction / user-based | Strength: flexible deployment, strong freight audit; Weakness: weaker international coverage |
| project44 | Real-time multi-modal visibility platform providing ETA predictions and exception management | SaaS | Custom quote | Strength: best-in-class visibility; Weakness: not a full TMS (no rate shopping or tendering) |
| e2open | End-to-end supply chain platform with integrated TMS, trade compliance, and carrier collaboration | SaaS | Custom quote | Strength: broad supply chain coverage; Weakness: complex integration, large-enterprise focus |
| Descartes Systems | TMS and logistics management suite with routing, compliance, and carrier connectivity | SaaS | Custom quote | Strength: strong regulatory/customs; Weakness: fragmented product portfolio from acquisitions |
| 3Gtms | Mid-market cloud TMS with load planning, carrier tendering, and shipper-carrier collaboration | SaaS | Custom quote | Strength: purpose-built mid-market; Weakness: smaller carrier network |
| GoFreight | Freight forwarding TMS for customs brokers and NVOCCs with shipment, document, and billing management | SaaS | Custom quote | Strength: freight-forwarding specialist; Weakness: limited for shippers |

## Relevant Industry Standards or Protocols

- **EDI 204 / 214 / 990** — ANSI X12 electronic data interchange standards for motor carrier load tender, shipment status, and tender response; foundational for carrier integration in TMS
- **ELD (Electronic Logging Device) Mandate** — US FMCSA regulation requiring HOS logging via certified ELDs; TMS platforms must ingest ELD data for accurate capacity and ETA planning
- **NMFC (National Motor Freight Classification)** — Commodity classification system governing LTL freight rating in North America
- **Incoterms 2020** — ICC-defined international trade terms governing freight responsibility and risk transfer; embedded in TMS shipment configuration
- **AMS / ISF (Importer Security Filing)** — US Customs pre-filing requirements for ocean imports; relevant to TMS international modules
- **GS1 EPCIS** — Event-based visibility data standard enabling interoperable track-and-trace across supply chain participants

## Available Research Materials

1. Grand View Research (2025). *Transportation Management System Market Report, 2033*. Grand View Research. https://www.grandviewresearch.com/industry-analysis/transportation-management-systems-market
2. Mordor Intelligence (2025). *Transportation Management System Market Size, Trends, Share Analysis 2031*. Mordor Intelligence. https://www.mordorintelligence.com/industry-reports/transportation-management-system-market
3. Precedence Research (2025). *Transportation Management Systems Market Size to Hit USD 47.97 Bn by 2035*. Precedence Research. https://www.precedenceresearch.com/transportation-management-systems-market
4. Ubico (2026). *The 6 Best TMS Software for Logistics Companies in 2026*. Ubico Blog. https://www.ubico.io/post/the-6-best-tms-software-for-logistics-companies-in-2026
5. SelectHub (2026). *Oracle Transportation Management Reviews 2026: Pricing, Features & More*. SelectHub. https://www.selecthub.com/p/tms-software/oracle-transportation-management/
6. Gartner (2026). *Best Transportation Management Systems Reviews 2026*. Gartner Peer Insights. https://www.gartner.com/reviews/market/transportation-management-systems
7. GoFreight (2026). *TMS Software Compared: 10 Platforms by Use Case (2026)*. GoFreight Blog. https://gofreight.com/blog/best-tms-software

## Market Research

**Market Size:** The global TMS market is estimated at USD 21.75 billion in 2026, projected to grow to USD 82.43 billion by 2034 at a 17.72% CAGR. North America holds the largest regional share at ~43%, driven by e-commerce growth and fragmented carrier networks.

**Funding:** Oracle (ORCL) and SAP dominate enterprise TMS. Manhattan Associates (MANH) is publicly traded and a perennial Gartner Leader. Uber Freight has invested heavily post-Transplace acquisition. Project44 raised $420M in Series E funding (2021).

**Pricing Landscape:** Oracle OTM starts at ~$450/month at the low end; enterprise deployments run into seven figures annually. MercuryGate uses transaction-based or user-based SaaS pricing. Mid-market platforms are typically custom-quoted. Visibility overlays like project44 are subscription-based per lane or shipment volume.

**Key Buyer Personas:** Logistics directors at shippers managing carrier networks and freight spend; 3PLs and freight brokers orchestrating carrier tendering; operations managers seeking real-time shipment visibility; finance teams running freight audit and payment processes; international trade compliance officers.

**Notable Trends:** AI is generating dynamic ETA predictions from real-time traffic, weather, and carrier history. Route optimisation now incorporates carbon emissions as an optimisation variable alongside cost and time. Freight audit automation is eliminating manual invoice reconciliation. Carrier capacity volatility post-pandemic has accelerated shipper investment in multi-carrier tendering and spot-market connectivity.

## AI-Native Opportunity

- Dynamic route optimisation that continuously re-optimises loads in response to live traffic, weather, carrier ELD data, and dock appointment availability — beyond static batch planning
- AI-powered freight audit that automatically matches carrier invoices to shipment records, flags discrepancies, and learns from dispute outcomes to improve accuracy over time
- Predictive carrier capacity and spot-rate forecasting using historical lane data, market indices, and demand signals to guide carrier selection and contract negotiation
- Carbon-aware load building that minimises emissions per unit shipped by optimising mode choice, consolidation, and carrier selection alongside cost
- Natural-language shipment visibility assistant allowing operations staff to query shipment status, exceptions, and carrier performance in plain language without logging into multiple carrier portals
