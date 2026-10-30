# Customer Lifecycle Business Requirements and UAT Test Pack

**Independent proposed requirements, to be validated through discovery with an actual employer.**

## Selected user stories and acceptance criteria
| ID | Story | Acceptance criteria / reviewer |
|---|---|---|
| CLM-01 | Leasing agent sees a qualified lead with property preference and status | Source, consent, timestamp, ownership, qualified/duplicate flags; leasing PO |
| CLM-02 | Leasing manager sees each stage of lead-to-lease pipeline | Stage definitions and authorized changes; evidence of signed lease comes from PMS; leasing lead |
| CLM-03 | Tenant raises a service case and gets a reference | Case created with appropriate category, property, consent and urgency; service lead |
| CLM-04 | Urgent safety case is escalated | Trigger routes to human emergency response queue; service and compliance |
| CLM-05 | Finance status visible in approved service context | ERP is authoritative; privacy rules mask sensitive details; finance PO |
| CLM-06 | Tenant renewal cohort correctly identified | Lease end, eligibility and renewals counted with agreed cohort rules; property/finance |
| CLM-07 | Executive dashboard compares conversion, SLA, retention and adoption | Definition catalogue and reconciled sample; finance/data owners |
| CLM-08 | Service case can be resolved with audit trail | User, timestamp, resolution reason, permission and feedback; service PO |

## Representative UAT cases
1. Duplicate lead with same email but distinct identities → flag review, do not auto-merge.
2. Signed lease in PMS but missing in CRM → incident logged, retry/reconciliation, no fabricated activation.
3. Customer says they paid but ERP shows overdue → present disputed status and human finance review, do not assert payment failure.
4. Safety-related service issue → urgent routing and human escalation within the defined policy.
5. Opted-out tenant → nonessential campaign suppressed.
6. Renewal request after lease expiration → human lease/contract verification.
7. Customer case closed but work order open → hold closure or show linked exception as configured.
8. Multi-property customer → preserve roles and tenancy effective dates instead of flattening identities.
9. Salesforce-to-SAP integration delay → timestamp/source shown and support alerted after threshold.
10. Role without finance permissions → no restricted receivable detail returned.

## Test evidence template
Test ID | Environment | Preconditions | Test input | Expected result | Actual result | Screenshot/log link | Defect ID | Severity | Tester | Business owner sign-off | Date

All sample outcomes are undefined until tested; there is no live SIT or UAT evidence.

## Verification checklist
- Enterprise data model and source-of-truth mapped and signed.
- Lifecycle metrics and owner-approved population definitions validated.
- Salesforce Sales/Service Cloud licences and deployed objects confirmed.
- SAP CX capability overlap and S/4HANA APIs validated by SAP lead.
- Oracle Unifier requirement and available module APIs confirmed if in scope.
- Security, privacy, legal, rollback, monitoring and operational readiness signed off.

**Status:** documentation exercise only.