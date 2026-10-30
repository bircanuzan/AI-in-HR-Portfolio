# CLM Portfolio Delivery Governance, KPIs and Change Adoption

**Illustrative portfolio design; all budgets, baselines and targets must be obtained from the employer.**

## Portfolio initiative register
| Workstream | Value hypothesis | Decision gate | Critical dependency |
|---|---|---|---|
| A. Salesforce Sales Cloud lead-to-lease | More transparent leasing pipeline | Qualified lead schema and user sign-off | CRM/PMS IDs and data quality |
| B. Salesforce Service Cloud tenant support | Faster, accountable case closure | SLA categories and escalation approval | Property operations and service routing |
| C. SAP CX rationalisation | Consistent communication and preference capture | Architect-led capability decision; may be unnecessary | Salesforce overlap, consent governance |
| D. SAP S/4HANA / PMS data linkage | More reliable billing and tenancy status | Reconciled sample financial records | Finance controls, master-data ownership |
| E. Unifier (if applicable) | Joined-up project/work-order approval visibility | Relevant module & use case validated | PMO/asset operations scope |
| F. Lifecycle insights | Retention and lifetime-value visibility | Signed KPI definitions, baseline | Authoritative and reconcilable data |
| G. Change/adoption | Repeatable day-to-day behaviour | Pilot sign-off by business owners | Training, support, SOPs, champions |

## Governance
**Portfolio sponsor:** transformation executive; **business owners:** commercial, leasing, service, property operations, finance; **technical owners:** enterprise architect, data integration, Salesforce and SAP leads; **change owner:** business transformation/enablement lead.

**Stage gates:** discover → business case → architecture/data/controls → build/configure → SIT/UAT → readiness/pilot → launch/hypercare → BAU ownership → 30/60/90-day benefits review. Each requires named approver, date, acceptance evidence and risks.

**RAID controls:** integration dependency, tenant identity duplication, delayed finance approval, data-privacy concern, case-routing backlog, licensing/cost change, vendor coordination and undertrained users. Workstreams have owners and decision escalation thresholds.

**Financial controls:** budget requested vs approved vs forecast vs actual; separate capacity savings from realised cash savings; portfolio benefits only booked after finance validation. No programme budget or ROI is claimed for this case.

## KPI dictionary (proposal)
| Metric | Illustrative definition | Data systems |
|---|---|---|
| Lead-to-lease conversion | New signed leases / qualified leads in comparable cohort | Sales Cloud + PMS |
| Time to first response | Median working-time from qualified enquiry to agent first response | Sales Cloud |
| Move-in readiness | Completed approved onboarding checklists before move-in / due move-ins | PMS + Salesforce |
| Service SLA compliance | Eligible cases resolved within category SLA / eligible cases | Service Cloud |
| First-contact resolution | Eligible customer service cases resolved in first contact / eligible cases | Service Cloud |
| Tenant retention | Eligible renewed tenancies / eligible tenancies ending in period | PMS + Service Cloud |
| Customer lifetime value | Approved contribution-based model; distinguish actuals and forecast | Finance + PMS + CRM |
| CSAT | Favourable survey responses / valid survey responses with sample counts | Survey + Service Cloud |
| Tool adoption | Active eligible users completing approved workflow / eligible users | Tool telemetry + process QA |
| Data reconciliation | Cross-system records matched with approved keys / sampled eligible records | Integration monitoring |

No actual baselines, uplift or customer outcomes are available. All calculations require data governance and metric-owner approval.

## Executive reporting (monthly)
- Portfolio heatmap: RAG status, milestones, finance, blockers, top 3 decisions required.
- Adoption: workflow use, completion quality, training/support and process friction by function.
- Benefits: signed measurement hypotheses vs observed post-launch metrics; attribute cautiously.
- Cross-vendor governance: contractual work packages, integration design authorities, escalations and UAT defects.

## UAT and readiness
Pilot users from leasing, finance, customer service, property operations and IT. Test happy path, duplicate tenant, failed synchronisation, disputed charge, withheld consent, urgent safety ticket, delayed approval and failed renewal sync. Go/no-go is a business-owner decision; the program manager organises evidence and escalation.

## Truthful scope statement
Designed as independent case-study deliverables; not a production Salesforce, SAP CX, S/4HANA or Oracle Unifier programme.