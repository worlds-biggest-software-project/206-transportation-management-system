# Transportation Management System (TMS) — Feature & Functionality Survey

> Candidate #206 · Researched: 2026-05-03

## Solutions Analysed

| Tool | Type | Licence / Model | URL |
|------|------|-----------------|-----|
| Oracle Transportation Management | Commercial SaaS / On-Premise | Proprietary; from $450/month | https://www.oracle.com/scm/logistics/transportation-management/ |
| SAP Transportation Management | Commercial SaaS | Proprietary; custom quote | https://www.sap.com/products/scm/transportation-management.html |
| Manhattan Active Transportation | Commercial SaaS | Proprietary; custom quote | https://www.manh.com/solutions/supply-chain-management-software/transportation-management |
| Uber Freight TMS | Commercial SaaS | Proprietary; custom quote | https://www.uberfreight.com/ |
| MercuryGate | Commercial SaaS | Proprietary; transaction/user-based | https://www.mercurygate.com/ |
| project44 | Commercial SaaS | Proprietary; custom quote | https://www.project44.com/ |
| e2open | Commercial SaaS | Proprietary; custom quote | https://www.e2open.com/ |
| Descartes Systems | Commercial SaaS | Proprietary; custom quote | https://www.descartes.com/solutions/transportation-management |
| 3Gtms | Commercial SaaS | Proprietary; custom quote | https://www.3gtms.com/ |
| GoFreight | Commercial SaaS | Proprietary; custom quote | https://gofreight.com/ |

## Feature Analysis by Solution

### Oracle Transportation Management (OTM)

**Core features**
- Multi-modal route optimization (road, air, ocean, rail) with cost minimization
- Cooperative routing for private fleet and third-party carrier optimization
- Load consolidation and shipment building with automatic mode/carrier selection
- Carrier rate maintenance and fleet asset allocation across time zones
- Hours of service (HOS) constraint enforcement for compliance
- Freight payment, auditing, and settlement workflows
- EDI 204/214 carrier integration for automated tender and shipment status

**Differentiating features**
- Broadest mode coverage (air, ocean, rail, road) in single platform
- Cooperative routing balances internal fleet and carrier utilization
- Deep ERP integration via Oracle ecosystem (Finance, Supply Chain)
- Global multi-currency and timezone support

**UX patterns**
- Web-based interface for planning and execution
- Real-time fleet visibility dashboard
- Shipment tracking with carrier ETA monitoring
- Rate and carrier management consoles

**Integration points**
- APIs for carrier EDI integration (X12 204, 214, 990)
- ERP integration (Oracle Finance, Supply Chain)
- Warehouse management system (WMS) connectivity
- Third-party freight payment and audit platforms

**Known gaps**
- Complex implementation requiring significant Oracle expertise
- Strong Oracle ecosystem dependency limits flexibility
- Limited real-time exception management vs pure visibility platforms
- Steep learning curve for SMB users

**Licence / IP notes**
- Proprietary SaaS; from $450/month small deployments, enterprise licenses significantly higher
- Oracle-owned; licensing includes mandatory support agreements

---

### SAP Transportation Management (SAP TM)

**Core features**
- Transportation planning integrated with SAP ERP
- Carrier tendering and bid management
- Dock scheduling and yard management
- Shipment execution and tracking
- Freight costing and settlement
- Multi-modal transportation planning

**Differentiating features**
- Tight SAP ERP integration (S/4HANA, ECC)
- Dock and yard management for inbound/outbound coordination
- Supply chain visibility across production and logistics
- Global implementation support via SAP ecosystem

**UX patterns**
- SAP Fiori UI for modern experience
- Integration into SAP Supply Chain Control Tower
- Real-time shipment and dock status
- Carrier performance dashboards

**Integration points**
- SAP ERP core integration (Purchasing, Materials, Finance)
- Warehouse management (SAP Extended Warehouse Management)
- Supply chain control tower
- Third-party carrier and freight payment systems

**Known gaps**
- High implementation cost and timeline (12-24 months typical)
- SAP ecosystem dependency limits alternative integrations
- Weaker carrier network connectivity vs standalone TMS
- Less mature AI-driven optimization compared to Manhattan

**Licence / IP notes**
- Proprietary SaaS; custom quote pricing
- SAP-owned; bundled licensing with other SAP modules typical

---

### Manhattan Active Transportation

**Core features**
- Cloud-native multi-modal optimization (18 million considerations/second)
- Load optimization with automatic capacity and route calculation
- Carrier management and bid/rate administration
- Real-time shipment tracking and exception management
- Backhaul and multi-stop route planning
- Continuous optimization engine re-solving shipments in real time

**Differentiating features**
- 5-year consecutive Gartner Magic Quadrant Leader (8× winner)
- Fastest optimization engine in industry (10x faster solves)
- Continuous re-optimization based on live data (traffic, weather, ELDs)
- Cloud-native architecture enabling rapid deployment
- Carbon emissions as optimization variable

**UX patterns**
- Intuitive dashboard with real-time load visualization
- Drag-and-drop shipment and carrier management
- Exception alerts with action recommendations
- Mobile-first carrier and operations interface

**Integration points**
- APIs for carrier, WMS, and ERP connectivity
- Real-time traffic and weather data integration
- ELD (Electronic Logging Device) integration for HOS compliance
- Third-party freight payment and audit platforms
- Customer order integration

**Known gaps**
- Enterprise pricing point; less accessible to SMBs
- Smaller carrier network than Uber Freight or project44
- Limited international coverage vs Oracle/SAP

**Licence / IP notes**
- Proprietary SaaS; custom quote pricing
- Publicly traded (MANH); investment-grade stability
- Strong IP portfolio around optimization algorithms

---

### Uber Freight TMS

**Core features**
- North America-focused TMS with integrated carrier network
- Real-time spot-rate visibility and negotiation
- Load tendering across Uber's carrier network
- Route and load optimization
- Managed transportation services with Uber's own capacity
- Real-time shipment tracking and ETA

**Differentiating features**
- Access to Uber's large North American carrier network
- Integrated managed transportation services (vs platform-only)
- Competitive cost structure through technology and volume
- Real-time spot-rate pricing vs fixed tariffs
- Mobile-first operations experience

**UX patterns**
- Consumer app-like interface for easy adoption
- Real-time tracking with ETA and carrier info
- One-click shipment submission to Uber network
- Spot-rate marketplace for dynamic pricing

**Integration points**
- APIs for WMS, ERP, and TMS integration
- Real-time rate APIs for competitive pricing
- Shipment status webhooks
- Customer portal integrations

**Known gaps**
- Primarily North America; limited international
- Dependent on Uber's carrier network (limited choice)
- Less flexible for shippers with complex multi-carrier strategies
- Newer platform with smaller customer base than Manhattan/Oracle

**Licence / IP notes**
- Proprietary SaaS; custom quote pricing
- Uber-owned; post-Transplace acquisition
- Technology built on Transplace platform heritage

---

### MercuryGate

**Core features**
- Routing and route optimization with carrier tendering
- Freight audit and payment automation
- Carrier management with scorecarding
- Load building and consolidation
- Shipment visibility and tracking
- Multi-modal transportation planning
- Network design and planning tools

**Differentiating features**
- Strong freight audit automation reducing manual reconciliation
- Flexible transaction-based or user-based pricing models
- Mid-market focus with easier deployment than enterprise platforms
- Integration with freight payment and audit providers
- Good dock/facility scheduling

**UX patterns**
- Web-based interface with modern UX
- Carrier bid management with automated awarding
- Freight audit dashboard with exception highlighting
- Real-time shipment tracking

**Integration points**
- APIs for carrier EDI, WMS, and ERP integration
- Freight audit and payment platform connections
- Order management integration
- Carrier rate file upload and maintenance

**Known gaps**
- Weaker international coverage vs Oracle/SAP
- Smaller real-time optimization capabilities vs Manhattan
- Limited carrier network (relies on shipper's own carriers)
- Less sophisticated AI features vs newer platforms

**Licence / IP notes**
- Proprietary SaaS; transaction-based or user-based pricing
- Owned by Infios Group; stable privately-held vendor

---

### project44

**Core features**
- Real-time multi-modal shipment visibility (air, ocean, road, rail)
- ETA prediction and dynamic delay forecasting
- Exception management with automated alerts
- Carrier performance analytics and scorecarding
- Standard-based data exchange (GS1 EPCIS, APIs)
- Supply chain event visibility

**Differentiating features**
- Best-in-class visibility platform; 500+ carrier integrations
- AI-powered ETA predictions from traffic, weather, and historical data
- Passive tracking via carrier network participation (less data silos)
- Compliance reporting for supply chain regulations
- Real-time exception management with low false-positive rates

**UX patterns**
- Dashboard-centric interface with global shipment view
- Customisable alerts and escalation workflows
- Carrier and customer portal access
- Mobile tracking for supply chain users

**Integration points**
- 500+ carrier API integrations
- GS1 EPCIS data exchange
- ERP and order management system APIs
- Third-party provider integrations

**Known gaps**
- Not a full TMS; lacks rate shopping, tendering, and load building
- Does not manage freight payment or settlement
- Primarily a visibility overlay vs end-to-end planning
- Requires integration with separate TMS or carrier management tool

**Licence / IP notes**
- Proprietary SaaS; custom quote pricing per lane/shipment volume
- Well-funded (Series E $420M); strong IP in ETA prediction algorithms

---

### e2open

**Core features**
- Integrated TMS with supply chain planning and execution
- Supplier collaboration and order management
- Trade compliance (tariff, duty, restricted party screening)
- Carrier management and freight payment
- Global supply chain visibility
- Demand planning and forecasting

**Differentiating features**
- End-to-end supply chain platform (procure-to-pay + order-to-delivery)
- Deep trade compliance module for international
- Supplier collaboration network with embedded logistics
- Unified order and shipment management

**UX patterns**
- Enterprise dashboard with supply chain control tower view
- Supplier portal for collaboration and order visibility
- Compliance and regulatory reporting dashboards
- Mobile access for field and transportation operations

**Integration points**
- APIs across procurement, orders, shipping, and compliance
- Supplier portal integrations
- ERP system connectivity
- Third-party carrier and service provider integrations

**Known gaps**
- Complex integration and high implementation cost
- Large-enterprise focus; less accessible to SMBs
- Significant learning curve for full platform mastery
- Fragmented product portfolio can slow innovation

**Licence / IP notes**
- Proprietary SaaS; custom quote pricing
- Public company (EZOP); strong market position
- Numerous acquisitions have created complex IP portfolio

---

### Descartes Systems

**Core features**
- TMS with routing, optimisation, and carrier connectivity
- Customs and regulatory compliance management (ISF, AMS)
- Logistics optimization and planning
- Carrier tendering and management
- Freight payment integration
- International trade documentation

**Differentiating features**
- Strong regulatory and customs compliance (ISF, AMS, NMFC)
- Good for shippers with complex international requirements
- Carrier connectivity and EDI management
- Logistics management suite combining multiple modules

**UX patterns**
- Traditional web-based interface
- Compliance and regulatory workflow dashboards
- Carrier rate and tender management
- Shipment tracking and visibility

**Integration points**
- EDI and API connectivity to carriers
- ERP and order management integration
- Customs and trade compliance APIs
- Freight payment platform integrations

**Known gaps**
- Fragmented product portfolio from acquisitions (Logimax, ShipManager)
- Less cohesive user experience vs pure-play TMS
- Weaker optimization vs Manhattan
- Less modern cloud architecture vs newer platforms

**Licence / IP notes**
- Proprietary SaaS; custom quote pricing
- Public company (DSGX); portfolio includes multiple acquired solutions

---

### 3Gtms

**Core features**
- Cloud-based TMS for load planning and carrier tendering
- Shipper-carrier collaboration portal
- Route optimization and carrier selection
- Shipment tracking and visibility
- Freight audit integration
- Mid-market focus with straightforward deployment

**Differentiating features**
- Purpose-built for mid-market shippers
- Easier implementation than enterprise platforms
- Flexible deployment and quick ROI
- Carrier collaboration features for smaller networks

**UX patterns**
- Modern cloud interface
- Intuitive load planning and tendering
- Carrier self-service portal
- Real-time shipment visibility

**Integration points**
- APIs for order management, WMS, and freight payment
- Carrier portal and EDI connectivity
- Basic ERP integration

**Known gaps**
- Smaller carrier network vs Uber Freight, project44
- Limited optimization sophistication vs Manhattan
- Less international capability
- Smaller feature set overall

**Licence / IP notes**
- Proprietary SaaS; custom quote pricing
- Privately held; mid-market focus

---

### GoFreight

**Core features**
- Freight forwarding and customs management
- Shipment documentation and compliance
- Billing and invoicing for freight services
- Carrier and warehouse network management
- Multimodal shipment execution
- Trade compliance and customs filing

**Differentiating features**
- Purpose-built for freight forwarders and NVOCCs
- Strong in documentation and customs workflows
- Good for international ocean/air logistics
- Simplified interface for forwarding-specific operations

**UX patterns**
- Forwarding-focused dashboard
- Documentation and compliance checklists
- Shipment status and milestone tracking
- Customer invoice and billing management

**Integration points**
- Carrier and warehouse APIs
- Customs filing system integration
- Third-party logistics provider connections
- Customer portal access

**Known gaps**
- Not suitable for shippers managing own freight; forwarding-specific
- Limited domestic or intra-modal capabilities
- Smaller platform overall
- Limited optimization and planning features

**Licence / IP notes**
- Proprietary SaaS; custom quote pricing
- Smaller specialist player

---

## Cross-Cutting Feature Themes

### Table-Stakes Features

Any TMS targeting logistics operations must include:

- **Load planning and optimization** — automatic shipment consolidation, carrier selection, and route building
- **Carrier management** — rate cards, tendering, bid/ask workflows, contract administration
- **Shipment tracking and visibility** — real-time status, ETA, and exception alerts
- **Multi-modal support** — at minimum road and LTL; ideally ocean, air, rail
- **EDI/API carrier integration** — X12 204/214 or modern APIs for tender and status exchange
- **Freight audit and payment** — invoice reconciliation, discrepancy flagging, payment settlement
- **Reporting and analytics** — KPIs (cost, time, exceptions), carrier scorecards, performance trends
- **Hours of Service (HOS) compliance** — ELD integration for US motor carrier regulation

### Differentiating Features

Capabilities present in leading solutions that provide competitive advantage:

- **Real-time continuous optimization** — re-solving loads as new orders arrive and conditions change (Manhattan)
- **AI-powered ETA prediction** — dynamic delay forecasting from traffic, weather, and historical data (project44)
- **Spot-rate and carrier network access** — real-time pricing and shipper-carrier matching (Uber Freight)
- **End-to-end supply chain integration** — unified order, procurement, and logistics planning (e2open)
- **Trade compliance automation** — ISF filing, tariff calculation, restricted-party screening for international
- **Carbon emissions optimization** — route and mode selection considering environmental impact
- **Dynamic dock scheduling** — yard management and appointment optimization
- **Mobile-first operations experience** — field-friendly interfaces for drivers, technicians, operations staff

### Underserved Areas / Opportunities

Gaps identified across the solution space that represent genuine opportunities:

- **AI-driven carrier selection** — most platforms require manual bidding; ML could score carrier proposals by cost, time, reliability, and capacity
- **Predictive freight demand forecasting** — current platforms react to orders; AI could forecast demand by lane and recommend capacity procurement
- **Autonomous exception resolution** — platforms alert on delays/exceptions; AI could autonomously reroute shipments or negotiate with carriers
- **Intelligent shipper-carrier collaboration** — most platforms separate shipper TMS from carrier systems; AI could enable real-time collaborative replanning
- **Emissions and sustainability optimisation** — few platforms weight carbon alongside cost; AI could balance environmental and financial objectives
- **White-glove last-mile optimization** — parcel and LTL last-mile remains manual; AI could dynamically optimize routes with real-time delivery window negotiation
- **Yard and dock automation** — most platforms manage scheduling but not physical automation; integration with yard robotics and dock systems
- **Automated freight invoice auditing** — current manual review; ML could detect rating errors, duplicate invoices, and service failures with high confidence

### AI-Augmentation Candidates

Manual or rule-based features where AI could meaningfully improve outcomes:

- **Carrier bid evaluation and selection** — currently manual; ML could score proposals by total cost, reliability, and capacity
- **Load building optimisation** — currently rule-based; ML could identify high-value consolidation opportunities missed by heuristic engines
- **Dynamic ETA prediction** — most tools use static carrier estimates; ML models could learn from actual traffic, weather, and carrier performance
- **Exception management and escalation** — currently rule-based alerts; AI could predict which exceptions will impact delivery and recommend proactive solutions
- **Freight rate prediction and negotiation** — current spot rates static; ML could forecast rate trends and recommend optimal timing for capacity procurement
- **Demand forecasting by lane** — current platforms reactive; AI could forecast demand by origin-destination lane to guide network planning
- **Carbon footprint calculation** — currently manual estimates; AI could optimize for emissions alongside cost and service levels
- **Shipper-carrier contract compliance monitoring** — manual review of terms; AI could track contract performance and flag renewal opportunities

## Legal & IP Summary

No copyright or licensing conflicts identified among solutions analysed. All are proprietary SaaS with clear licensing models. Relevant standards (EDI X12, ELD, NMFC, Incoterms, GS1 EPCIS) are publicly defined specifications and not proprietary. However, note that (1) Route optimisation algorithms are patent-encumbered across industry; freedom-to-operate analysis is essential before implementing optimisation features; (2) Real-time ETA prediction models (project44, Manhattan) likely have patent protection; similar to above, FTO review required. Regulatory compliance with ELD mandate and FMCSA HOS rules is mandatory for US deployments. Trade compliance features must adhere to US Customs (ISF), international Incoterms, and export control regulations.

## Recommended Feature Scope

Based on the analysis above, a prioritised feature scope for an AI-native TMS:

**Must-have (MVP)**
- Load planning with automatic shipment consolidation and carrier selection
- Carrier rate card management and bid/ask tendering workflows
- Real-time shipment tracking with status and ETA
- EDI X12 (204/214) and/or REST API carrier integration
- Freight audit and payment reconciliation
- Basic KPI reporting (cost, time, exceptions)
- HOS compliance and ELD integration for US drivers

**Should-have (v1.1)**
- AI-powered continuous load re-optimisation as orders arrive
- Dynamic ETA prediction using traffic, weather, and carrier history
- Carrier performance analytics and automated scorecarding
- Multi-modal support (air, ocean, rail alongside road/LTL)
- Carbon emissions calculation and eco-routing
- Shipper-carrier collaboration portal with real-time visibility
- Exception management with AI-recommended resolutions
- Dock and yard scheduling automation

**Nice-to-have (backlog)**
- AI-powered carrier bid evaluation and automated selection
- Demand forecasting by lane with capacity procurement recommendations
- Autonomous exception resolution with carrier communication
- Spot-rate forecasting and negotiation assistance
- International trade compliance (ISF, tariff, restricted party screening)
- Freight rate trend analysis and contract renewal alerts
- Multi-tenant marketplace for shipper-carrier matching
- Integration with warehouse automation and robotics systems
