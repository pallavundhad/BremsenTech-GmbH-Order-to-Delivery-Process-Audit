**Tier-2 Automotive Supplier · Bavaria, Germany · SAP S/4HANA Migration Case Study**

> I mapped every step. I quantified every failure. Then I designed the fix.
> **EUR 683,200 in annual losses identified · 17 manual handoffs eliminated · 7 process gaps solved with SAP S/4HANA**

## Why I Built This

Most people learning SAP study modules in isolation, they know what SD does, they know what PP does, but they have never seen how a broken process looks *before* SAP, what it actually costs the business, and how each module addresses a specific, named failure.
I wanted to build the thing that makes that connection real.
So I created BremsenTech GmbH, a fictional Tier-2 automotive brake component manufacturer in Bavaria which gave it a real business crisis, and audited it the same way a management consultant would on day one of a paid engagement. Real industry benchmarks. Real SAP module logic. Real financial quantification. The only thing fictional is the company name.

The result is a full Order-to-Delivery process audit: AS-IS mapped in BPMN 2.0, seven gaps quantified in EUR, a TO-BE redesign with every SAP module named and justified, and an 18-month phased implementation roadmap.

## The Business Problem

BremsenTech sits at a crossroads that is common across German Tier-2 automotive suppliers. Continental AG and ZF Friedrichshafen, together 75% of their revenue are demanding EDI integration and real-time delivery visibility as a **non-negotiable condition of contract renewal.** On top of that, BMW and Mercedes-Daimler have signalled they will only consider direct Tier-1 suppliers who can integrate into their digital supply chain infrastructure. BremsenTech cannot do either of those things on SAP Business One 9.3.

The gap between where the company is and where its customers need it to be is not a technology gap. It is a process gap that technology will solve but only if you first understand exactly what is broken and what it is costing.

That is what this audit does.

## What I Actually Did
**Benchmarked the business against the industry.**
I pulled eight data points from McKinsey, Oliver Wyman, AIAG, Odette International, APQC, and Ardent Partners, the same sources a consulting firm would cite and built a side-by-side comparison showing where BremsenTech sat against Tier-2 best practice on every key supply chain metric. The red cells tell the story on their own.

**Mapped the full AS-IS process in BPMN 2.0.**
Nineteen steps. Six swim lanes. Every manual handoff, every paper form, every phone call drawn out and annotated with its real cost. I used proper BPMN notation with start events, end events, XOR gateways with YES/NO paths, sequence flows across lane boundaries — because that is the standard language of SAP project teams and process consultants.

**Turned observations into financial arguments.**
Each of the seven gaps I identified has an annual EUR cost attached to it. Not an estimate pulled from thin air, a calculation with named inputs, a logic trail, and an assumptions tab in Excel you can open and stress-test. When I write "EUR 180,000/year in SLA penalties to Continental AG," that number has a formula behind it.

**Designed the TO-BE process with SAP module precision.**
The TO-BE map is not a vague "after SAP" state. Every automated step is labelled with the exact module that handles it [SAP SD] for order confirmation, [SAP PP] for MRP scheduling, [SAP QM] for inline inspection, [SAP TM] for carrier booking. The diagram shows the before and after side by side so the improvement is immediate and visual.

**Built a phased implementation roadmap.**
Three phases, 18 months, SAP Activate methodology. Phase 1 delivers the core ERP foundation and cuts OtD from 14.2 to 11 days. Phase 2 activates manufacturing and quality modules. Phase 3 turns on full EDI connectivity with Continental and ZF. Each phase has specific, measurable outcomes, not just "go live."

## The Numbers

| Metric | AS-IS | Industry Target | Gap |
|---|---|---|---|
| Order-to-Delivery Cycle | 14.2 days | 7–10 days | +79% above benchmark |
| On-Time Delivery Rate | 87% | 95–98% | −9 percentage points |
| Invoice Processing Lag | 8.5 days | 3 days (automated) | +5.5 days |
| Inventory Turnover | 9x / year | 12–18x / year | −6 cycles |
| EDI Integration | 0% | 78% of EU peers | Full gap |
| Defect Detection Speed | 6-hour batch lag | Real-time inline | 6-hour blind spot |
| Manual Process Handoffs | 17 | 4 (industry avg) | +13 unnecessary steps |

**Annual cost of these gaps: EUR 683,200 which is not counting a EUR 4M+ BMW opportunity currently out of reach.**

## The SAP Fix

Nine modules. Each one mapped to a specific gap. Each one chosen because it is the right tool for the job not because it sounds impressive.

| Module | What It Fixes | The Business Impact |
|---|---|---|
| **SAP SD** | Zero EDI, manual order entry | PO auto-creates Sales Order · ORDERS/ORDRSP/DESADV/INVOIC live |
| **SAP MM** | Fragmented inventory data | Real-time stock · MRP material requirements automated |
| **SAP PP** | Excel scheduling (2.1-day delay) | MRP planning run replaces spreadsheet · same-day scheduling |
| **SAP QM** | 6-hour end-of-line batch inspection | Inline inspection at each production stage · defects caught immediately |
| **SAP FI/CO** | 8.5-day invoice lag | Auto EDI INVOIC on goods issue · same-day invoicing live |
| **SAP EWM** | Manual stock updates, bin chaos | Real-time bin tracking · inventory turns: 9x → 14x |
| **SAP TM** | Phone-based transport booking | Automated carrier selection · real-time shipment tracking |
| **Integration Suite (BTP)** | No EDI with any customer | Full B2B EDI with Continental, ZF, Bosch — ORDERS, DESADV, INVOIC |
| **SAP Analytics Cloud** | No visibility into any KPI | Live OtD dashboard · quality metrics · exec reporting |

## What Changes After Implementation
Before → After

OtD Cycle:          14.2 days  →  8.1 days
Manual Handoffs:    17         →  4
Invoice Lag:        8.5 days   →  Same day
Inventory Turns:    9x/year    →  14x/year
On-Time Delivery:   87%        →  96%+
Annual Loss:        €683,200   →  €83,200 (residual)

Annual savings:     EUR 600,000+
OEM opportunity:    EUR 4,000,000+ unlocked

## Repository Contents

| File | What It Is |
|---|---|
| `BremsenTech_Process_Audit.pptx` | 10-slide consultant deck, the full story from benchmark to roadmap |
| `AS-IS_Process_Map.png` | BPMN 2.0 current state diagram, every pain point annotated in red |
| `TO-BE_Process_Map.png` | BPMN 2.0 future state diagram, SAP module labels on every automated step |
| `gap_analysis.xlsx` | 7-gap structured table, root cause, EUR impact, priority, SAP fix |
| `roi_model.xlsx` | ROI model with live Excel formulas and a full assumptions tab |
| `benchmark_data_sources.md` | Every data source cited with named, linked, with context |

## Tools & Methodology

`draw.io` for BPMN 2.0 · `PowerPoint` for the consultant deck · `Excel + Python (openpyxl)` for the ROI model · `SAP Help Portal` for module documentation · `SAP Learning` for S/4HANA module overviews · Benchmarks from McKinsey · Oliver Wyman · AIAG · Odette International · APQC · Ardent Partners · IATF 16949

## A Note on the Fictional Company

BremsenTech GmbH does not exist. The methodology, the benchmarks, the SAP module logic, and the process gaps do.

Using a fictional company was a deliberate choice. It meant I could go as deep as the work required — without access constraints, NDAs, or simplified scope. The output is what a real engagement would produce. The company just happens to exist only in this repository.

*Portfolio Project 02 · SAP + PM Track · OTH Amberg-Weiden · May 2026*
*[Pallav Undhad]
