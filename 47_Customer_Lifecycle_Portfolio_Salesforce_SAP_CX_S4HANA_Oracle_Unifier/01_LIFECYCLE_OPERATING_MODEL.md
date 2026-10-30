# End-to-end Customer Lifecycle and Operating Model

**Illustrative real-estate/property-management enterprise | fictional inputs**

| Stage | Customer objective | Accountable function | Front-office workflow | Key control | Indicative KPI |
|---|---|---|---|---|---|
| Prospecting & acquisition | Find and assess a property | Leasing/sales | Enquiry capture → qualification → viewing → offer | Duplicate contact and consent check | Lead-to-viewing conversion |
| Contract/onboarding | Lease and move in | Leasing + finance + facilities | Signed lease → finance approval → handover → welcome | Human-approved terms and receipts | Move-in readiness rate |
| Engagement | Know property services | Customer success/tenancy | Welcome communications, facilities/service guidance | Preference & privacy rules | 30-day engagement |
| Service | Resolve issue | Customer service + operations | Ticket intake → triage → contractor → resolution → feedback | Safety escalation and SLA ownership | First-contact resolution, SLA |
| Renewal/retention | Decide whether to renew | Leasing + relationship team | Renewal eligibility → outreach → offer → response | Human-approved offer and financial terms | Renewal/retention |
| Loyalty/referral | Recommend and remain engaged | Customer experience | Surveys, referrals, feedback themes | Consent and benefit controls | NPS (survey-defined), referral |

## Current vs future state
**Current illustrative:** separate sales spreadsheet, manual service inbox, ERP invoice extracts, tenant portal with partial statuses, inconsistent customer IDs and no unified lifecycle reporting.

**Proposed:** customer/journey identifiers, lead-to-opportunity funnel, tenant onboarding checklist, case management with human routing, integration events for lease/payment/work-order statuses, role-specific dashboards and governed benefit review.

## 5 decisions required before build
1. Confirm canonical customer, property, unit, tenancy and lease identifiers; do not simply merge different persons into one “customer”.
2. Agree responsibility boundaries: Salesforce case is not the ERP ledger or legally authoritative lease.
3. Define service escalation classes: safety, privacy, disputed charges, vulnerable tenants and contractual exceptions → named humans.
4. Agree SLA clock definitions, renewal denominator, owner-approved retention metrics and telemetry before baseline reporting.
5. Obtain legal, financial, information security and operational signoff before customer messaging automation.

## Change plan
- Discovery interviews: leasing, finance, customer service, facilities, property management, integration/IT and tenant-facing employees.
- Co-design workshops: identify handoffs, duplicate approvals, service exceptions and responsibilities.
- Readiness: process owner appointed, training assets, SOP revisions, data validation, access checks and business sponsor sign-off.
- Pilot: one property/location/tenant segment; capture feedback, defects, training completions and operational outcomes.
- Scale: progressive rollout with champion network, weekly hypercare, handoff to BAU owners and 30/60/90-day reviews.

No live workshops or pilots are claimed.