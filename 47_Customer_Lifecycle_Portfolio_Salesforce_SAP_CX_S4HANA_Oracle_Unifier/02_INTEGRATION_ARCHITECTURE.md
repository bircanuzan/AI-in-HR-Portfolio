# Salesforce — SAP — Oracle Unifier Integration and Data Governance Blueprint

**Conceptual solution, not validated against any specific customer's SAP/Salesforce releases, licensed modules or existing enterprise architecture.**

## System roles (proposed, require discovery)
| Platform | Possible responsibility | Business data | Proposed owner |
|---|---|---|---|
| Salesforce Sales Cloud | Leads, account/contact, opportunities, leasing pipeline | lead IDs, contact permissions, sales activities | Commercial/leasing |
| Salesforce Service Cloud | Tenant service cases, queues, SLA milestones, feedback | case IDs, interactions, escalation | Customer service |
| SAP CX (where licensed) | Customer engagement, consent, marketing and/or service capability; decide whether complementary to or overlapping with Salesforce | profiles, preferences, campaigns | CX / marketing |
| SAP S/4HANA | Financials, invoice/payment status and master-data integration as configured | customer/business partner references, AR status | Finance |
| Property management system | Property, unit, tenancy, contract details and operational requests | property/unit/lease IDs and effective dates | Property operations |
| Oracle Unifier (if present) | Capital/project, facility or contract workflow and approvals depending on deployed modules | project/workflow references | Projects / capital delivery |
| Power BI | Role-based CLM and program metrics fed from approved data products | curated, masked snapshots | Data / transformation PMO |

**Architecture note:** SAP CX is a portfolio of capabilities, not a synonym for SAP S/4HANA. Salesforce Sales Cloud/Service Cloud functionality may overlap with SAP CX; implementing both without an approved application rationalisation decision creates duplication. Oracle Unifier integration is conditional, not assumed to exist in the enterprise.

## Integration principles
- **Customer identity:** create a master crosswalk mapping Salesforce account/contact, SAP business partner and PMS tenant/lease IDs; keep relationship/effective-date history.
- **Events:** examples of business events are lead qualified, lease approved, move-in completed, payment-status updated, service case opened/closed and renewal decision.
- **API / middleware:** design asynchronous events or governed APIs after confirming platform APIs, authentication, reliability, rate limits and integration platform standards. No direct database writes.
- **Privacy:** field minimisation, tenant consent, access by role, audit trails and data retention policy. Segment data that should not travel to the sales CRM.
- **Financial authority:** posted payment and receivable statuses originate in the designated ERP/finance system, not manual sales notes.
- **Exceptions:** idempotent event keys, retries with dead-letter review, reconciliation, owner notifications and a manual safe fallback.
- **Quality:** duplicate rate, missing key percentages, event delivery lag, reconciliation errors and stale tenancy statuses measured in a controlled dashboard.

## Example event contract — non-executable illustration
```json
{
  "event_type": "tenancy.onboarding_ready",
  "event_id": "DEMO-10071",
  "tenant_ref": "TEN-00071",
  "lease_ref": "LEASE-00071",
  "property_ref": "PROP-002",
  "approval_status": "APPROVED_BY_HUMAN",
  "effective_at": "2026-10-01T12:00:00+04:00",
  "source_system": "PROPERTY_MANAGEMENT_SAMPLE",
  "schema_version": "1.0"
}
```

The event contains no names or payment information. Schema should be reviewed against real systems, legal requirements, and IT architecture standards before use.

## Proposed delivery dependencies
1. Enterprise architecture review and customer-data ownership approval.
2. SAP, Salesforce and PMS existing-license/integration inventory.
3. Canonical identity and consent design.
4. Source-to-target mappings, interface contracts, access policies, and reconciliation testing.
5. UAT and disaster/rollback plan signed off by leasing, finance, service and IT.
6. Rollout communications, training, adoption observation, reporting and BAU handover.

No production tenant, customer records or platform integrations were accessed or tested.