# Human-AI Workforce Design and Agent Governance

**Bircan Uzan | HumanEvoX | Project 42**

> **Portfolio demonstration, October 2026.** Original, fictional enterprise HR case with synthetic assessment records. This is a **designed governance framework and executable offline evaluation script**, not a deployed AI agent, live Microsoft tenant implementation, client engagement, production security review or proven business outcome.

## Executive case: HR Operations AI Agent — digital-worker onboarding and probation

**Scenario:** A fictional UAE professional-services business with 800 employees wants to introduce an AI service agent to handle low-risk HR policy FAQs and draft standard employment letters. Leaders are concerned about inaccurate answers, personal data exposure, unauthorised employment decisions, hidden operational costs and employee adoption.

**Business question:** How do we define an AI agent's job, assess its competence before deployment, give it restricted access, supervise it during probation and conduct evidence-based performance reviews while keeping humans accountable?

**Proposed solution:** A human–AI workforce operating model that applies HR competency design, assessment-centre thinking, onboarding, probation, performance management, governance and continuous improvement to a software agent.

## Project artefacts

| Artefact | Deliverable |
|---|---|
| [Case study and workflow](CASE_STUDY.md) | Business problem, operating model, AS-IS/TO-BE workflow and use-case boundaries |
| [Governance, methodology and tools](GOVERNANCE_AND_METHODS.md) | Six-stage methodology, human accountability, NIST AI RMF alignment, tools, RACI, controls and agent job description |
| [Agent assessment matrix](data/agent_assessment_cases.csv) | 12 synthetic test scenarios including edge cases and human-escalation tests |
| [Offline scorecard calculator](scripts/evaluate_agent.py) | Python 3 standard-library evaluator; reads the recorded scenario outcomes; prints pass/fail gates |
| [30/60/90-day rollout plan](ROLLOUT_AND_VALUE.md) | Proposed pilot, UAT, training, monitoring, KPI and benefits methodology |
| [Agent performance review template](AGENT_PERFORMANCE_REVIEW.md) | AI probation review with competency evidence, safety gates and sign-off |

## Skills demonstrated
Human–AI work design • competency and responsibility mapping • assessment design • agent governance • human-in-the-loop controls • service operations • change management • policy-to-workflow mapping • TEVV planning • responsible AI • agent performance review • KPI dashboards • business stakeholder governance.

## Tools and AI used — exact distinction

- **Used for this portfolio:** GitHub/Markdown for structured case artefacts; AI-assisted content development using ChatGPT; a Python 3 standard-library script for an **offline** assessment scorecard; synthetic CSV test data. The CSV is an invented assessment sample, **not outputs from an actual AI agent**.
- **Proposed deployment stack (not connected, built or tested):** Microsoft Copilot Studio or Azure AI Foundry Agent Service for agent configuration; Microsoft Power Automate for rule-based routing and approvals; Microsoft Teams for human escalation; SharePoint for versioned policy retrieval; Microsoft Entra ID for least-privilege identity; Power BI for dashboarding.
- **Methodological references (not certification or external audit):** SIPOC, RACI, BPMN-style process mapping, risk-tiering, NIST AI Risk Management Framework (Govern / Map / Measure / Manage), test–evaluate–verify–validate (TEVV), gated pilot, 30/60/90-day adoption and KPI review.

## Proposed outcomes, not achieved metrics
- Automate **only** low-risk responses where source policy and requester identity have been verified.
- Require human approval before letters are issued and for all employment, payroll, benefits, visa and hiring decisions.
- Maintain a searchable audit trail, named accountable owner, exception queue and rollback/kill-switch plan.
- Apply threshold gates to a test suite before a future pilot; no claim of production efficiency, headcount reduction or ROI.

**Positioning:** This project is about **governing digital work** rather than engineering an autonomous agent from scratch. Engineering and security partners would be required for a live deployment.

© 2026 Bircan Uzan — All Rights Reserved.
