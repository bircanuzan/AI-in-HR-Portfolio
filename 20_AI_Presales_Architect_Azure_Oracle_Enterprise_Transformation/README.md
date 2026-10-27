# Project 20 — AI Pre-Sales Architect | Azure, Oracle & Enterprise Transformation

**Kaidon.ai role-aligned original solution-design simulation.** This is not a real delivery, client engagement, or Azure/TOGAF certification.

## Fictional customer
GulfConnect Group operates Oracle HCM/ERP SaaS, a separate CRM, legacy .NET/Java portal and disconnected spreadsheets. Its CIO wants governed integration, modern applications, Azure analytics and carefully approved AI use cases.

## Presales deliverables
1. [Executive discovery and workshop](01_Discovery_and_Executive_Workshop.md): decision-makers, questions, capability mapping, business and non-functional requirements.
2. [Reference solution architecture](02_Azure_Oracle_Integration_Architecture.md): Azure PaaS, serverless, event-driven integrations, APIs, modernization, security and data architecture.
3. [Modernization and migration decisions](03_Modernization_Migration_Roadmap.md): six Rs, Kubernetes trade-offs and phased delivery.
4. [RFP response and Statement of Work](04_RFP_SOW_and_Estimate.md): scope, acceptance, assumptions, estimates and executive value narrative.
5. [Enterprise architecture controls](05_Data_AI_MLOps_Governance.md): data lake, MLOps, analytics, responsible AI and TOGAF-informed governance.
6. [Example API contract](api/employee_metrics.openapi.yaml) and [Python proposal estimate](src/estimate.py), with [unit tests](tests/test_estimate.py).

### Reference architecture — decision-first, not a diagram alone
Oracle HCM/ERP and CRM remain systems of record. A governed API layer using Azure API Management plus Functions / Logic Apps validates requests. Durable workflow messages use Service Bus; pub/sub updates may use Event Grid. Curated inputs land through Data Factory into ADLS Gen2, are transformed in a fit-for-purpose service such as Databricks, and power Power BI. Sensitive AI use cases require retrieval permissions, evaluation and human approval.

**Azure App Service / Container Apps vs. AKS:** prefer managed PaaS unless workload constraints justify the complexity and operational ownership of Kubernetes. **MLOps:** only if real model retraining and operational evaluation are warranted; a retrieval prototype does not automatically require ML model training.

### Run
Python 3.10+: `python src/estimate.py` and `python -m unittest discover -s tests -v`. Example estimates are *assumptions*, not a vendor price quote.

### Covers job-description keywords
Client discovery, executive workshops, solution shaping, enterprise architecture, TOGAF concepts, Oracle SaaS/ERP/CRM, Azure PaaS/serverless, API/microservices, Kubernetes and containers, event-driven design, data lakes/MLOps, security, RFP, SOW, budget assumptions, roadmap and delivery gates.

**What it does not prove:** Azure production deployment, successful bid awards, Kubernetes operations or TOGAF/Azure certifications.

JD: https://ae.linkedin.com/jobs/view/ai-pre-sales-architect-at-kaidon-ai-4476581295
