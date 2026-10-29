# Pilot, adoption and value — proposed 30/60/90-day plan

All actions are plans, not completed deployment milestones.

## Days 1–30: scope and evidence
- Interview HR operations, HRIS, IT, security, legal and employee representatives.
- Build SIPOC and BPMN-level AS-IS / TO-BE; classify tasks into human, rules-based automation or agent.
- Establish baseline: volume, complexity, first-contact resolution, handling time, rework, escalation, satisfaction and policy breaches.
- Approve policy corpus and test scenario catalogue. Run offline simulations; resolve all failed mandatory safety gates.

## Days 31–60: controlled configuration
- Engineering configures a least-privilege proof of concept in a **sandbox** (subject to procurement and tenant licensing).
- Configure separate deterministic approval workflow, read-only retrieval, role mapping, audit logs, access tests and safe refusal routes.
- Conduct UAT, red-team scenarios, human calibration and shadow-mode monitoring with approved test data.
- Train HR reviewers in agent limitations, overrides and incident escalation.

## Days 61–90: pilot decision and supervision
- If and only if gates pass and governance owners sign off, conduct a small human-supervised pilot.
- Weekly quality samples, incident review and policy freshness checks; daily exception queue.
- Monthly agent-performance review and business-case update; expand, hold, narrow or retire scope.

## KPI dictionary and sample targets (illustrative)
| Measure | Definition | Target before expansion |
|---|---|---|
| Correct answer rate | Gold-standard correct / evaluated responses | >=95% |
| Mandatory escalation recall | Cases escalated / cases that required human | 100% |
| Unauthorised HR actions | Actions outside approved role or permissions | 0 |
| Audit completeness | Traces with minimum required fields / assessed traces | 100% |
| Approval SLA | Time from draft submission to accountable human decision | Baseline then target |
| Human review workload | Reviewer minutes per 100 resolved requests | Measure, no fabricated savings |
| Employee experience | Verified satisfaction and complaint themes | Measure by employee cohort |
| Cost-to-serve | Fully loaded licence, inference, build, security, support and human review cost per resolved case | Compare with baseline |

## Value modelling (not claimed savings)
Monthly net value = (validated minutes avoided per eligible request × eligible monthly requests × loaded labour cost per minute) – incremental monthly AI/platform licence, inference, integration, compliance, security, maintenance and human-review costs.

Measure **quality and downstream rework**, not only cases deflected. A successful agent might improve service without eliminating any jobs; employee redeployment or headcount reduction is not assumed.

## Vendor / architecture due diligence checklist
Model hosting and retention; geographic data processing; UAE/sector-specific privacy requirements; connectors and licensing; auditability; prompt-injection controls; approval separation; cost caps; versioning; human appeal; accessibility; reporting; vendor lock-in and exit plan.

## Learning ladder
1. Power Automate: deterministic HR approvals, exception routing and monitoring.
2. Copilot Studio: agent instructions, approved knowledge and tool permissions in a sandbox.
3. Python: build richer evaluation harnesses and API integrations.
4. Azure AI Foundry / LLMOps: tracing, model choice, red-teaming and operational deployment with technical partners.

**No certification, tenant access, live agent, measured ROI, or client deliverables are claimed in this project.**
