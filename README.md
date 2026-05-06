# Transportation Management System (TMS)

> Part of the [worlds-biggest-software-project](https://github.com/worlds-biggest-software-project) initiative.
>
> An AI-native, open-source TMS for route optimisation, carrier management, and freight audit across multi-modal logistics.

The Transportation Management System (TMS) project is a candidate open-source platform for shippers, 3PLs, and freight brokers who need to plan, execute, and audit transportation across road, ocean, air, and rail. It targets the gap between heavyweight enterprise suites (Oracle OTM, SAP TM, Manhattan Active) and narrow visibility overlays (project44), bringing AI-driven optimisation, freight audit, and shipment visibility into a single, deployable system.

---

## Why Transportation Management System (TMS)?

- Incumbent enterprise platforms (Oracle OTM, SAP TM, e2open) carry high implementation cost, long deployment timelines (12-24 months for SAP TM), and deep ecosystem dependencies that lock buyers in.
- Manhattan Active Transportation leads on optimisation but sits at an enterprise price point that is inaccessible to mid-market shippers and 3PLs.
- Visibility platforms such as project44 deliver excellent ETA prediction but are not full TMS solutions - they lack rate shopping, tendering, load building, and freight payment.
- Mid-market platforms (MercuryGate, 3Gtms) trade away international coverage, optimisation sophistication, and AI features for accessibility.
- Freight audit, carrier bid evaluation, and exception management remain heavily manual or rule-based across the market, leaving clear room for an AI-native open-source alternative.

---

## Key Features

### Load Planning and Optimisation

- Automatic shipment consolidation and carrier selection
- Multi-modal route building across road, LTL, ocean, air, and rail
- Continuous re-optimisation as new orders arrive and conditions change
- Backhaul and multi-stop route planning
- Carbon-aware load building that weights emissions alongside cost and time

### Carrier Management and Tendering

- Rate card management and contract administration
- Carrier tendering and bid/ask workflows with automated awarding
- Carrier performance analytics and automated scorecarding
- EDI X12 (204/214/990) and REST API connectivity for tender and shipment status
- Shipper-carrier collaboration portal with real-time visibility

### Shipment Visibility and Exception Management

- Real-time multi-modal shipment tracking with status and ETA
- AI-powered ETA prediction from traffic, weather, and historical carrier data
- Exception management with AI-recommended resolutions
- Carrier performance dashboards and KPI reporting
- Mobile-first interfaces for drivers and operations staff

### Freight Audit and Settlement

- Automated invoice-to-shipment matching with discrepancy flagging
- ML-based detection of rating errors, duplicate invoices, and service failures
- Payment reconciliation and settlement workflows
- Carrier dispute learning loop that improves audit accuracy over time

### Compliance and Trade

- Hours of Service (HOS) compliance via ELD integration for US motor carriers
- NMFC commodity classification for North American LTL rating
- International trade compliance hooks (ISF, AMS, Incoterms 2020)
- GS1 EPCIS event-based visibility data for interoperable track-and-trace

---

## AI-Native Advantage

AI capabilities are designed in from the start rather than bolted on. Continuous load re-optimisation responds to live traffic, weather, ELD data, and dock availability instead of running as static batch plans. ETA prediction and exception triage learn from historical lane and carrier behaviour. A natural-language visibility assistant lets operations staff query shipment status, exceptions, and carrier performance in plain language, and freight audit improves itself by learning from dispute outcomes. Carrier bid evaluation, spot-rate forecasting, and lane-level demand forecasting move carrier selection and capacity procurement from manual judgement to ML-supported decisions.

---

## Tech Stack & Deployment

The platform is intended to support cloud-native and self-hosted deployment, mirroring the cloud-native architectures of leading incumbents while remaining accessible to operators that require on-premise control. Carrier integration is built around EDI X12 (204/214/990) plus modern REST APIs, with GS1 EPCIS for cross-party visibility events. ELD integration is required for US HOS compliance. Integration surfaces include WMS, ERP, order management, and third-party freight payment platforms.

---

## Market Context

The global TMS market is estimated at USD 21.75 billion in 2026 and projected to grow to USD 82.43 billion by 2034 at a 17.72% CAGR, with North America accounting for roughly 43% of regional share (Grand View Research; Precedence Research; Mordor Intelligence). Incumbent pricing ranges from around USD 450/month for entry-level Oracle OTM up to seven-figure annual enterprise deployments; most mid-market and enterprise vendors quote custom pricing. Primary buyers are logistics directors at shippers, 3PLs and freight brokers, operations managers responsible for shipment visibility, finance teams running freight audit, and international trade compliance officers.

---

## Project Status

> This project is in the **research and specification phase**.  
> Contributions, feedback, and domain expertise are welcome.

---

## Contributing

We welcome contributions from developers, domain experts, and potential users.
See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

**Important:** All contributions must be your own original work or clearly attributed
open-source material with a compatible licence. Copyright infringement and licence
violations will not be tolerated and will result in immediate removal of the offending
contribution. If you are unsure whether a piece of code, text, or other material is
safe to contribute, open an issue and ask before submitting.

---

## Licence

Licence to be determined. See [discussion](#) for context.
