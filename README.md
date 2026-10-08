### Hi, I'm Alejandro More 👋

**Enterprise AI & Cloud Architect** · AI & IT Governance (ISO 42001, CGEIT, TOGAF) · FinOps · Lima, Peru

I design and run enterprise AI platforms end to end — from architecture and governance to the Terraform, pipelines and Kubernetes that put them in production. Most of that work lives in private organizations because it was built for enterprise clients; this page summarizes what's there.

#### 🧠 What I build

| Area | What it is | Stack |
|---|---|---|
| **LLM Gateway** | Multi-protocol gateway (OpenAI + Anthropic APIs) for a telecom operator: model catalog, self-hosted web search, PII redaction, admin UI for business areas, secrets from a cloud KMS via IAM agency (no keys in CI) | LiteLLM · PostgreSQL · Redis · SearXNG · Presidio · Open WebUI · Caddy · Terraform · Ansible · Jenkins |
| **AI Agents** | Agent platform and a Microsoft Teams channel for it (Microsoft 365 Agents SDK proxy → agent backend → LLM Gateway) | Microsoft Agent Framework · Bot Framework · Python |
| **MLOps** | Production path for CV models: synthetic data → EDA → training → MLflow registry (`champion` alias) → BentoML image built in-cluster with Kaniko → KServe `InferenceService` + web portal, one Jenkins job | PyTorch (ResNet18) · scikit-learn (GMM) · MLflow · BentoML · Kaniko · KServe · Kubernetes |
| **AIOps** | Observability lab: a telemetry simulator emitting correlated logs, metrics and traces over OTLP, an incident-correlation stack, and a multi-cluster cost hub | OpenTelemetry · Mimir · Grafana · Keep · OpenCost |
| **FinOps** | OpenCost hub aggregating cost allocation for several Kubernetes clusters over mTLS, plus invoice exporter | OpenCost · OTel Collector · Mimir · Grafana |
| **Data / Regulatory** | PoC validating a cloud data warehouse for regulatory CDR archiving: partition pruning, local indexes on cold storage, stored procedures, real compression ratio | GaussDB(DWS) · OBS · Terraform · Python |

#### 🌱 Open source

- **[OpenCost](https://github.com/opencost/opencost)** (CNCF) — contributor:
  - [feat(huawei): add Huawei Cloud provider support](https://github.com/opencost/opencost/pulls?q=is%3Apr+author%3Aalejandromore)
  - [fix(costmodel): price default-pricing GPU nodes from RAM in GB, not bytes](https://github.com/opencost/opencost/pulls?q=is%3Apr+author%3Aalejandromore)

#### 🛠️ Toolbox

`Terraform` `Ansible` `Jenkins` `GitHub Actions` `Kubernetes` `Helm` `Python` `Java` · Huawei Cloud · AWS · Azure · AI-assisted engineering with Claude Code, Goose and Google Antigravity

#### 📜 Certifications

AIGPC (ISO 42001) · CGEIT · TOGAF 9 · COBIT · ISO 38500 · ITIL 4 · FinOps Practitioner · CCSK · Huawei HCIP

📫 [LinkedIn](https://www.linkedin.com/in/alejandro-more-montoya/)
