# Loss KPIs, WBR / MBR and Executive Reporting
**Illustrative metric architecture only. No production data or achieved results.**

## Proposed source contracts
- Finance-approved network-loss actuals by *employer-defined* WHL, WHD, Concessions buckets.
- Throughput denominator as formally approved by Finance (e.g., units, value or transactions; not interchangeable).
- Site operations data, inventory accuracy indicators, incident evidence and delivery exceptions only where legally permitted and reliably matched.
- Data-freshness, missing-value, site-mapping, duplicate-event and timing controls.

## Draft scorecard (definitions must be signed off)
| KPI | Example analytical question | Validation |
|---|---|---|
| Loss actual versus target | Which regions, sites and buckets are above approved target? | Finance-signed bookings and time period |
| Loss rate | Are losses changing after controlling for comparable volume? | Same denominator definition across sites |
| High-severity exception backlog | How many open incidents lack verified containment? | ICQA/operations evidence |
| Root-cause confidence | How many incidents have source evidence, not inferred causes? | RCA/COE review |
| Corrective action on-time rate | Are action owners closing issues to validated criteria? | Audit follow-up |
| Customer experience guardrail | Did availability, substitutions, returns or delivery experience worsen? | CX owner approval |
| Adoption rate | Are sites using the new standard control steps? | Sampling/training evidence |

**Do not combine reporting currencies across UAE, Saudi Arabia and Egypt without a Finance-approved FX translation and accounting treatment.** Report local-currency actuals separately if the consolidated basis is not established.

## Weekly Business Review (WBR)
1. One-page trend: week-to-date, previous week, four-week trend, target gap, largest category/site drivers.
2. Data integrity: freshness, pending adjustments and known reconciliations.
3. Top exceptions: incident facts, documented scope, confidence, temporary containment.
4. Actions: owner, due date, barrier, next evidence checkpoint.
5. Executive asks: decision, trade-off, responsible approver and required date.

## Monthly Business Review (MBR)
- Country/site/category normalized trend and monthly target variance.
- Documented Finance bridge from last month to current month (volume/mix/timing/true process changes).
- Kaizen pilot outcomes, control-group/comparability caveats and customer-impact checks.
- Net benefit *only after Finance sign-off*: verified actual impact less implementation/ongoing costs.
- Portfolio RAG, approvals required, next-month capacity and priorities.

## Flash report trigger
An illustrative rule might alert on material loss spikes, category reclassification or stale reconciliation; numerical thresholds must be created from actual network variability, approved materiality and false-alert performance. This project makes no claim about Amazon thresholds.

## Data/BI approach
Conceptual pipeline: governed WMS/site records + approved Finance ledger → quality controls → reconciled loss category dataset → analyst review → Power BI/Excel scorecard → WBR/MBR. No live source connection or dashboard deployment is claimed.
