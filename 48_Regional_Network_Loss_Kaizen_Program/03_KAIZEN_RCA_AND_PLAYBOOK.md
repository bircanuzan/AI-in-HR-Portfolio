# Kaizen, Root-Cause Analysis, COE and Replication Playbook
**Original fictional scenario and proposed corrective actions, not tested on site**

## Example investigation: apparent inventory write-off increase at one dark store
**Symptom:** Periodic adjustment counts increase relative to a comparable period, while daily sales remain stable. This is a hypothetical trigger, not evidence of theft or any specific cause.

### Investigation protocol
1. Confirm whether a category definition changed, a delayed adjustment posted, or source data duplicated.
2. Reconcile inventory records with approved ledger amounts and validate event timestamps.
3. Run Pareto on approved incident subtypes to identify the highest measured contributions.
4. Observe the receiving-to-shelf-to-pick process and review sampled controls.
5. Use fishbone (process / people / technology / materials / environment / measurement) and **5 Whys** as hypothesis tools, not proof.
6. Identify alternative explanations and test them with time-bound evidence before choosing a solution.
7. Assign containment, permanent corrective action, prevention control and benefit-validation owner.

### Illustrative hypotheses, not findings
- Poor scan compliance at receiving or transfers; validate matched scan and physical counts.
- Unclear status ownership during returns or concessions; validate handoff timestamps and exception codes.
- Unit conversion or timing issue in reporting; reconcile with Finance before counting an operational saving.

## Sample corrective-action register
| Action | Function | Success evidence |
|---|---|---|
| Reconcile bucket logic and Finance posting windows | Finance + Data | Signed source-to-report mapping |
| Improve exception scan checkpoints | Site operations + ICQA | Reproducible scan compliance test |
| Standardize transfer custody acknowledgement | Transport + RDC | Sample handoff trace completeness |
| Introduce daily unresolved-exception review | Site manager | Aged exception trend and action closure |
| Validate rollout training and SOP comprehension | Enablement + country operations | Observed workflow checks, not attendance only |

## COE (correction of error) template
- Customer/network impact; time window; affected regions and count; validated facts.
- Detection path and why existing control did not surface earlier.
- Root-cause evidence, alternatives considered, contributing conditions.
- Immediate containment and long-term prevention; one owner each.
- Measurable exit criteria, due dates and independent verification.
- What system/process conditions changed, not individual blame.

## Scale decision rules
Only standardize a pilot if: severity-adjusted losses trend in the intended direction on a comparable denominator; no material harm to availability/CX; Finance supports the benefits method; policy/compliance signoff is complete; local country differences are addressed. Otherwise, refine and retest.

## Change and sustain
30/60/90-day cadence: site champion orientation, SOP briefing, demonstration in daily work, spot audit, weekly countermeasure follow-up and monthly review with regional leaders. Escalations and coaching should use objective data with no punitive individual inference.

## Reusable artifacts
Project charter, RACI, RAID, loss bucket data dictionary, Pareto worksheet, 5-Whys worksheet, COE template, corrective-action tracker, WBR/MBR pack, pilot go/no-go and operating handover checklist.

**Evidence status:** Methodology design complete; source system access, site baseline, experiments, user adoption and realized operational impact not performed or measured.