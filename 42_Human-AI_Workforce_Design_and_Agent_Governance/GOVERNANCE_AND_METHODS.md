# Governance framework, methodology and tools

## Six-stage implementation methodology
1. **Discover and map work.** Interviews, SIPOC, HR service catalogue, AS-IS/TO-BE, exception inventory, employee impact assessment and data classification.
2. **Design the mixed workforce.** Task-allocation matrix (human / deterministic automation / LLM agent), agent job description, delegated authority, competencies, RACI, service levels.
3. **Assess and select the agent.** Synthetic benchmark, scenario-based competency rubric, approved policy grounding, prompt-injection and PII tests, quality/safety thresholds, reviewer calibration.
4. **Onboard and control.** Named owner, least-privilege identity, approved tools, versioned knowledge sources, audit logging, escalation routes, change control and rollback.
5. **Probation and supervision.** Offline TEVV; shadow mode; limited human-reviewed pilot; weekly quality review; incidents and corrective actions; go/no-go committee.
6. **Manage and improve.** Monthly scorecard, drift/policy change tests, cost per resolved case, human workload, employee satisfaction, re-training/reconfiguration and retirement criteria.

## Control design aligned to NIST AI RMF functions (conceptual)
| AI RMF function | Operational evidence planned |
|---|---|
| Govern | AI use-case owner, risk appetite, policy, sign-offs, incident response |
| Map | Task boundaries, process map, stakeholders, affected users and data flows |
| Measure | Test-set accuracy, mandatory escalation recall, log completeness, unauthorised action count and bias/privacy tests |
| Manage | Limited release gates, remediation backlog, monitoring, rollback, periodic reviews |

NIST AI RMF is a reference framework here, **not** evidence of official conformity, formal validation or third-party assurance.

## RACI
| Activity | HR Ops Owner | AI Product/Engineering | InfoSec & Privacy | Legal/Compliance | HR Case Specialist |
|---|---|---|---|---|---|
| Set HR policy and service scope | A | C | C | C | R |
| Configure agent and integrations | C | A/R | C | C | I |
| Define test scenarios and assess HR correctness | A | R | C | C | R |
| Approve access and security controls | C | R | A | C | I |
| Approve pilot/go-live | A | R | C | C | C |
| Handle employment/visa/payroll decisions | A | I | I | C | R |
| Review monthly agent performance | A | R | C | C | R |

R = responsible; A = accountable; C = consulted; I = informed. One accountable owner per row.

## Practical tool architecture (design only)
- **Microsoft Copilot Studio / Azure AI Foundry Agent Service:** prospective agent development/orchestration platform; no environment was provisioned.
- **SharePoint:** proposed approved policy repository with document owner, effective date and retention controls.
- **Power Automate / Teams Approvals:** proposed deterministic human approval and case escalation.
- **Entra ID:** proposed identity, permissions and conditional access.
- **Power BI:** proposed operational scorecard.
- **Python 3 + CSV:** actual portfolio artefacts for offline, deterministic calculation against fictional test observations.
- **ChatGPT:** used to assist preparation and structure of this fictional governance case; **not** evidence of a deployed agent.

## Risk and escalation register
| Risk | Trigger | Preventive / detective control | Human decision maker |
|---|---|---|---|
| Fabricated HR policy | Missing/expired source or unsupported response | Refuse or escalate; verify source version; review samples | HR Policy Lead |
| Sensitive data disclosure | Request for salary, ID, medical or immigration data | No sensitive data in prompts; deny/exclude permissions; incident logging | InfoSec / HR |
| Unauthorised HR transaction | Agent attempts changes to HRIS or payroll | Read-only role and no write connector; blocked tool audit | HRIS Owner |
| Prompt injection / adversarial content | User instructions conflict with system scope | Deny unsafe instructions; test cases; monitoring | AI Product Lead |
| Human overreliance | Users treat draft as final HR decision | Clear AI label, human approval and training | HR Ops |
| Bias / employee impact | Unequal handling or inconsistent escalation | Test stratified cases and review complaints | HR + Compliance |
| Knowledge change / drift | Policy or agent version update | Versioned evaluation and regression gate | HR Policy + Product |

## Stage gates (proposed, not met by any production agent)
1. **Safety:** 0 unauthorised actions in the test set.
2. **High-risk escalation:** 100% of cases requiring a human are escalated.
3. **Response correctness:** at least 95% correct in the defined benchmark.
4. **Audit completeness:** 100% required fields recorded.
5. **Release:** Independent HR, engineering and security approval after live-environment testing. Sample pass/fail numbers are *not* a go-live authorisation.

## Sources
- NIST AI RMF: https://www.nist.gov/itl/ai-risk-management-framework
- Microsoft Copilot Studio: https://learn.microsoft.com/en-us/microsoft-copilot-studio/
- Microsoft Power Automate: https://learn.microsoft.com/en-us/power-automate/
