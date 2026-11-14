### Hi, I'm Alejandro More 👋

**Enterprise AI & Cloud Architect** · AI & IT Governance (ISO 42001, CGEIT, TOGAF) · FinOps · Lima, Peru

I design and build enterprise AI platforms end to end, from architecture and governance to the Terraform, pipelines and Kubernetes that run them. Most of that work lives in private organizations because it was built for enterprise clients; this page summarizes what's there.

#### 🧠 What I build

| Area | What it is | Stack |
|---|---|---|
| **LLM Gateway** | Multi-protocol gateway (OpenAI + Anthropic APIs) for a telecom operator: model catalog, self-hosted web search, PII redaction, admin UI for business areas, secrets from a cloud KMS via IAM agency (no keys in CI) | LiteLLM · PostgreSQL · Redis · SearXNG · Presidio · Open WebUI · Caddy · Terraform · Ansible · Jenkins |
| **AI Agents** | Agent platform and a Microsoft Teams channel for it (Microsoft 365 Agents SDK proxy → agent backend → LLM Gateway) | Microsoft Agent Framework · Bot Framework · Python |
| **MLOps** | End-to-end pipeline for CV models: synthetic data → EDA → training → MLflow registry (`champion` alias) → BentoML image built in-cluster with Kaniko → KServe `InferenceService` + web portal, one Jenkins job | PyTorch (ResNet18) · scikit-learn (GMM) · MLflow · BentoML · Kaniko · KServe · Kubernetes |
| **AIOps** | Observability lab: a telemetry simulator emitting correlated logs, metrics and traces over OTLP, an incident-correlation stack, and a multi-cluster cost hub | OpenTelemetry · Mimir · Grafana · Keep · OpenCost |
| **FinOps** | OpenCost hub aggregating cost allocation for several Kubernetes clusters over mTLS, plus invoice exporter | OpenCost · OTel Collector · Mimir · Grafana |
| **Data / Regulatory** | PoC validating a cloud data warehouse for regulatory CDR archiving: partition pruning, local indexes on cold storage, stored procedures, real compression ratio | GaussDB(DWS) · OBS · Terraform · Python |

#### 🚀 Recent projects

| Project | What it is | Stack |
|---|---|---|
| **[alejandro-jobsearch-agent](https://github.com/alejandro-jobsearch/alejandro-jobsearch-agent)** | Agentic job-search pipeline: sources openings from job boards and ATS APIs, filters and scores them (deterministic ATS keyword coverage + LLM rubric) and tracks them as GitHub Issues on a Project board. A human approves every application. Built spec-first with coding agents. | LangGraph · Python · GitHub Actions · OpenAI-compatible LLM (GLM on Huawei Cloud MaaS) |
| **RPA control plane** (private) | Demo of an external control plane for an RPA operation: detects robot failures, classifies them, recovers by levels (retry, app reset, host restart with human approval) and escalates with an LLM diagnosis through the LLM Gateway. Passed 39 of 39 failure scenarios. | Kestra · Robot Framework · Blue Prism · Terraform · Ansible · GitHub Actions (OIDC) |
| **[devbox](https://github.com/alejandromore/devbox)** | Browser-accessible Linux desktop on Huawei Cloud, fully provisioned by code | Terraform · Ansible · Jenkins · KasmVNC · Caddy |
| **Self-hosted platforms** (private) | Hardened Nextcloud for sensitive company files, and an AI assistant gateway on Huawei Cloud, both deployed by pipeline | Terraform · Ansible · GitHub Actions · Docker |

#### 🌱 Open source

- **[OpenCost](https://github.com/opencost/opencost)** (CNCF) contributor (Huawei Cloud provider and a GPU pricing fix):
  - [feat(huawei): add Huawei Cloud provider support](https://github.com/opencost/opencost/pulls?q=is%3Apr+author%3Aalejandromore)
  - [fix(costmodel): price default-pricing GPU nodes from RAM in GB, not bytes](https://github.com/opencost/opencost/pulls?q=is%3Apr+author%3Aalejandromore)

#### 🛠️ Toolbox

`Python` `LangGraph` `LiteLLM` `Terraform` `Ansible` `Jenkins` `GitHub Actions` `Kubernetes` `Helm` `Java` · Huawei Cloud · AWS · Azure · AI-assisted engineering with Claude Code, Goose and Google Antigravity

#### 📜 Certifications

AIGPC (ISO 42001) · CGEIT · TOGAF 9 · COBIT · ISO 38500 · ITIL Foundation · FinOps Practitioner · CCSK · AWS Certified AI Practitioner · Azure Fundamentals · Huawei HCIA/HCIP Cloud

📫 [LinkedIn](https://www.linkedin.com/in/alejandro-more-montoya/)
