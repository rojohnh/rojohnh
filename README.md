<div align="center">
  <h1>👨‍💻 Rojohn A. Hernia</h1>
  <h3>Lead Infrastructure Architect | AI Platform Ops Expert | DevSecOps Engr | Fractional CTO</h3>
  <p>📍 Davao City, Philippines | 🌐 APAC / EMEA / US & Canada (Remote)</p>

  [![DITE Consortium](https://img.shields.io/badge/DITE_Profile-0f172a?style=for-the-badge&logo=googlecloud&logoColor=10b981)](https://roj.davaoitengineers.com)
  [![CloudVCard](https://img.shields.io/badge/CloudVCard-Digital_Identity-10b981?style=for-the-badge&logo=vcard)](https://roj.cloudvcard.net)
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/rojohn-hernia/)
  [![Email](https://img.shields.io/badge/Email-rhernia@davaoitengineers.com-ea4335?style=for-the-badge&logo=gmail)](mailto:rhernia@davaoitengineers.com)
</div>
<br/>

## 💼 Professional Summary

Senior Infrastructure Architect and AI Developer with **18+ years of battle-tested experience** in Platform Operations, API integrations, and high-concurrency cloud ecosystems. Specialized in **automating real-world business processes**: agentic workflows (n8n, LangChain, **Model Context Protocol**), secure **Retrieval-Augmented Generation (RAG)** systems, and production integrations of leading LLMs (**Anthropic Claude, OpenAI GPT, Google Gemini, Meta Llama**) into enterprise CRM and DevOps pipelines. Proven track record migrating legacy monoliths to zero-latency Edge networks, engineering self-healing Kubernetes environments, and delivering compliance-ready, zero-downtime architectures across AWS, GCP, Azure, and bare metal — while driving infrastructure costs toward $0 idle.

---

## 🤖 AI & LLM Engineering

![Anthropic Claude](https://img.shields.io/badge/Anthropic_Claude-191919?style=flat-square&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI_GPT-412991?style=flat-square&logo=openai&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Google_Gemini-4285F4?style=flat-square&logo=googlegemini&logoColor=white)
![Meta Llama](https://img.shields.io/badge/Meta_Llama-0467DF?style=flat-square&logo=meta&logoColor=white)
![MCP](https://img.shields.io/badge/Model_Context_Protocol-0f172a?style=flat-square&logo=anthropic&logoColor=10b981)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white)
![Zapier](https://img.shields.io/badge/Zapier-FF4F00?style=flat-square&logo=zapier&logoColor=white)
![Make](https://img.shields.io/badge/Make.com-6D00CC?style=flat-square&logo=make&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?style=flat-square&logo=elasticsearch&logoColor=white)
![Cloudflare Vectorize](https://img.shields.io/badge/Cloudflare_Vectorize-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![Cloudflare D1](https://img.shields.io/badge/Cloudflare_D1-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![Cloudflare AI Gateway](https://img.shields.io/badge/Cloudflare_AI_Gateway-F38020?style=flat-square&logo=cloudflare&logoColor=white)

* 🧠 **LLM APIs in production:** Anthropic Claude (Messages API, tool use with `strict` schemas, structured outputs, prompt caching), OpenAI GPT, Google Gemini, Meta Llama — wired into developer tooling, CRM/workflow automation, and business-process AI. **Claude Code, Claude Projects, connected knowledge, and the Agent SDK** are daily drivers, not demos; Cursor and Replit where they fit.
* 🎛️ **Controlled AI agents with human approval points:** Tool registries where risk classification lives in **code, not the system prompt** — so a prompt injection buried in customer text can make an agent *attempt* an action but never complete it. Durable run state in Postgres lets an agent park on a sensitive call, wait for a signed expiring approval link, and resume hours later in a different process. Rejections feed back as tool results so the agent adapts instead of blindly retrying.
* 🔁 **Production n8n workflows:** Not happy-path demos — error branches that are actually wired, retries with full jitter, idempotency keys enforced by unique constraints, business thresholds in Code nodes where they can be diffed, and grouped alerting with an explicit `UNKNOWN` state for when the monitor itself goes blind. Make and Zapier where they suit the job — and I'll tell a client when the honest answer is *buy the product, build nothing*.
* 📄 **Document extraction & intelligent workflows:** Native PDF reading with Claude (no OCR-then-regex, which loses exactly the table structure that matters) — then line items **re-summed in code**, because a language model is the wrong tool for addition and an invoice that doesn't balance is the last one you want auto-posted.
* 📚 **RAG, knowledge assistants & vector search:** **PostgreSQL 16 + pgvector**, Cloudflare Vectorize, Elasticsearch. Every `[n]` citation verified against the chunks actually retrieved — a fabricated citation is caught and logged, never shipped, because a wrong answer that *looks* sourced is the one people believe.
* 🛡️ **Serverless Enterprise RAG (Zero Trust AI Databank):** Architected a serverless RAG command center on Cloudflare Workers + **Vectorize** (semantic search) + **D1** (structured memory), powered by BAAI embeddings and Meta Llama instruction models; **Cloudflare AI Gateway** caching drives token burn on repeat queries to zero.
* 🔌 **Agentic Workflows & MCP:** Design and operate **Model Context Protocol (MCP)** connectors bridging AI agents to Jira/Confluence, Bitbucket, Datadog, and AWS — enabling agents to triage incidents, run observability queries, draft runbooks, and enforce deployment pre-flight checks autonomously.
* 🗂️ **CRM & business-process automation:** Agentic n8n + LangChain pipelines replacing manual data entry with zero-error LLM integrations into enterprise CRM and field-service systems (Xero / ServiceM8-shaped bill posting, quote intake, job scheduling); REST/webhook/OAuth2 integrations glued with TypeScript, Python, and Bash.
* 🔐 **Secure credentials & permissions:** Secrets in Worker/secret stores rather than config, OAuth2 refresh handled by the platform, HMAC-signed single-purpose expiring approval tokens with timing-safe verification, tenant isolation via Postgres RLS **plus** explicit query scoping, and log redaction applied on ingest — because redacting at the sink is already too late.
* 🧪 **Testing, logging, monitoring & failure handling:** Vitest suites running against in-memory ports (no network, sub-second, so they actually get run), one-JSON-object-per-line structured logs, mechanical CI validation of workflow exports, Datadog Bits AI and LLM Observability for AI workloads, and documented blast radius per failure mode.
* 📊 **AIOps:** Kubernetes clusters tuned specifically for AI application deployments; self-healing remediation pipelines that mitigate risk before end-users notice.

### 🔍 Proof — code you can actually read

| Capability | Where to look |
| :--- | :--- |
| Production n8n workflows with real error handling | [**ai-automation-blueprints**](https://github.com/rojohnh/ai-automation-blueprints/tree/main/workflows) — 4 importable workflows, 55 nodes, CI-validated |
| Controlled agent + durable human approval gate | [**approval-gateway**](https://github.com/rojohnh/ai-automation-blueprints/tree/main/services/approval-gateway) — TypeScript on Workers, 62 tests, typecheck clean |
| Document extraction gated on arithmetic | [02-document-extraction-to-accounting.json](https://github.com/rojohnh/ai-automation-blueprints/blob/main/workflows/02-document-extraction-to-accounting.json) |
| RAG with verified citations | [03-knowledge-assistant-rag.json](https://github.com/rojohnh/ai-automation-blueprints/blob/main/workflows/03-knowledge-assistant-rag.json) |
| Postgres/pgvector schema, RLS, expiry sweep | [db/schema.sql](https://github.com/rojohnh/ai-automation-blueprints/blob/main/db/schema.sql) |
| Live AI vision extraction + injection-resistant prompts | [**cloudvcard.net**](https://cloudvcard.net) — Workers AI vision with model fallback chains, structured JSON output, and PII-refusal prompts, running in production *(source private — happy to walk through it)* |
| Failure modes, runbook, security trade-offs | [docs/](https://github.com/rojohnh/ai-automation-blueprints/tree/main/docs) |
| When **not** to build custom | [choosing-the-tool.md](https://github.com/rojohnh/ai-automation-blueprints/blob/main/docs/choosing-the-tool.md) |

---

## 🧠 Engineering & Operational Standards

> *"We don't just write code. We engineer legacies. No fluff. Just battle-tested infrastructure and intelligent automation."*

* 🛡️ **Proactive Remediation:** Systems are architected to self-heal. I automate repetitive tasks and build intelligent workflows to mitigate risks before they impact end-users, requiring *zero manual follow-ups*.
* 🎯 **Outcome-Oriented Execution:** Technical architecture is strictly aligned with business metrics. The priority is always maximizing system uptime, protecting revenue during massive traffic spikes, and driving infrastructure costs to absolute zero ($0 idle cost).
* ⚡ **Continuous Learning & Adaptability:** Agile, cloud-native environments require speed and flexibility. I leverage AI heavily, foster open communication and deep empathy for the end user, and rapidly transition legacy setups to modern, decoupled AI ecosystems that scale instantly.

---

## ⚙️ Technical Arsenal

### ☁️ Cloud & Edge Platforms
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white)
![GCP](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat-square&logo=google-cloud&logoColor=white)
![Azure](https://img.shields.io/badge/Microsoft_Azure-0089D6?style=flat-square&logo=microsoft-azure&logoColor=white)
![DigitalOcean](https://img.shields.io/badge/DigitalOcean-0080FF?style=flat-square&logo=digitalocean&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare_Workers%2FPages-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

### 🚢 Container Orchestration & IaC
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![OpenShift](https://img.shields.io/badge/Red_Hat_OpenShift-EE0000?style=flat-square&logo=redhat&logoColor=white)
![AWS ECS/Fargate](https://img.shields.io/badge/AWS_ECS%2FFargate-FF9900?style=flat-square&logo=amazonecs&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![OpenTofu](https://img.shields.io/badge/OpenTofu-FFDA18?style=flat-square&logo=opentofu&logoColor=black)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white)
![NixOS](https://img.shields.io/badge/NixOS-5277C3?style=flat-square&logo=nixos&logoColor=white)

### 🔄 CI/CD, Observability & Data Streaming
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)
![Bitbucket Pipelines](https://img.shields.io/badge/Bitbucket_Pipelines-0052CC?style=flat-square&logo=bitbucket&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
![GitLab CI](https://img.shields.io/badge/GitLab_CI-FC6D26?style=flat-square&logo=gitlab&logoColor=white)
![Datadog](https://img.shields.io/badge/Datadog-632CA6?style=flat-square&logo=datadog&logoColor=white)
![Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?style=flat-square&logo=elasticsearch&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)

### 🐧 Languages, OS & Data
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white)
![RHEL 9](https://img.shields.io/badge/RHEL_9-CC0000?style=flat-square&logo=redhat&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=flat-square&logo=ubuntu&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![AWS Glue/Athena](https://img.shields.io/badge/AWS_Glue%2FAthena-FF9900?style=flat-square&logo=amazon-aws&logoColor=white)

<br/>

> **Specialized Operations:** RAG & MCP Integrations, CRM Automation, Cloudflare AI Gateway, PII/Legal data governance (AWS Lake Formation, IAM Least Privilege), High-Concurrency Mobile Proxy Routing (30k+ ports), SOC2/HIPAA Readiness, Zero Trust, WORM Storage, Anti-Bot Bypass, GeoIP Filtering, SELinux.

---

## 💼 Executive & Architecture Experience

### ⚖️ Senior DevOps Engineer | LegalMatch (US Legal Tech)
*2026 – Present*
* **Legal-Tech Platform Ops:** Ensure high availability and strict PII/legal-data security for a US platform matching clients with attorneys — AWS ECS/Fargate, ALB, RDS PostgreSQL 16 (**pgvector**), ECR, S3, EFS, all provisioned via Terraform with enforced cost-allocation tagging.
* **Zero-Downtime CI/CD:** Own Jenkins + Bitbucket Pipelines for multi-repo, cross-team releases (Kafka eventing framework); built automated pre-flight checks and rollback strategies that safeguard deployments and eliminate weekend firefighting.
* **AI-Accelerated DevOps:** Heavy production use of **Claude + MCP connectors** (Jira/Confluence, Datadog) and **Datadog Bits AI** to automate ticket workflows, observability queries, incident triage, and runbook generation.
* **FinOps / Cost Optimization:** Co-own the AWS cost-optimization epic — Datadog Cloud Cost Management waste dashboards, AWS Cost Explorer & Anomaly Detection, and retroactive + Terraform-enforced tagging governance.
* **Data & PII Governance:** Operate an S3 medallion data lake (Raw/Refined/Curated) with AWS Glue, Athena, and **Lake Formation tag-based RBAC** masking PII for legal data compliance.

### 🦅 Lead Systems Architect & AI Developer | DITE Consortium
*2018 – Present*
* **Enterprise Infrastructure:** Lead Architect for an elite engineering consortium specializing in cloud-agnostic enterprise deployments.
* **AI Product Engineering:** Architected and deployed the **Zero Trust AI Databank**, a serverless enterprise RAG command center utilizing Cloudflare Workers, Vectorize, and Meta Llama models.
* **CRM Automation:** Built intelligent agentic workflows and automated pipelines via n8n and LangChain, permanently replacing manual data entry with zero-error LLM integrations.
* **Cloud Migration & IaC:** Automated multi-cloud provisioning via Terraform and OpenTofu across AWS, GCP, and Azure, eliminating massive upfront hardware CapEx for enterprise clients.
* **Disaster Recovery:** Architected immutable, Write-Once-Read-Many (WORM) disaster recovery vaults to mathematically neutralize ransomware attacks and ensure continuous data protection.
* **High Availability:** Deployed and managed highly available container orchestration using Kubernetes and Red Hat OpenShift (OCP) for mission-critical applications.

### ⚡ Founder & Lead Platform Engineer | CloudVCard.net
*2024 – Present*
* **Edge SaaS Architecture:** Architected and launched a premium enterprise digital identity SaaS platform serving high-performing professionals and real estate brokers.
* **Zero-Idle Cost Infrastructure:** Engineered a serverless, decoupled architecture utilizing Cloudflare Pages for a zero-latency global frontend with $0 idle server costs.
* **Automated Deployments:** Built fully automated GitOps CI/CD pipelines via GitHub Actions for seamless, zero-downtime edge deployments.
* **Backend Concurrency:** Integrated Supabase and PostgreSQL to handle highly scalable, global backend concurrency and dynamic SVG QR code generation.

### 🌐 Senior DevOps Consultant & Infrastructure Architect | Freelance / Remote Contracts
*August 2025 – Present*
* **Hybrid Cloud Orchestration:** Architected and managed containerized workloads across GKE (Google), EKS (AWS), and AKS (Azure), ensuring 99.99% uptime for hybrid environments.
* **AIOps & AI Assistants:** Developed internal **RAG chatbots** using self-hosted **n8n** workflows and Elasticsearch to automate log analysis and proactive issue remediation; integrated **OpenAI, Claude, and Gemini APIs** into client automation pipelines.
* **Security Hardening:** Enforced strict RBAC, Network Policies, and Azure Policy for high-compliance enterprise clients, adhering to "Security by Design" principles.
* **Immutable Infrastructure:** Deployed NixOS QCOW images to DigitalOcean via Terraform/OpenTofu, establishing fully reproducible and rollback-capable server environments.

---

## 🛠️ Core Systems Engineering Experience

### 🚀 Senior DevOps Engineer | BlueDrive IT Services
*November 2024 – April 2026*
* Managed AWS and multi-cloud infrastructure, ensuring high availability for massive client hosting requirements.
* Orchestrated Kubernetes clusters specifically tuned for AI application deployments and scalable development environments.
* Architected a robust Zabbix and Elasticsearch cluster for centralized logging, reducing incident response times drastically.

### 🚀 Sr. Linux Engineer | Alorica Systems & Services Technologies, Inc.
*November 2023 – February 2025*
* Managed **10,000+ global Linux servers** (RHEL, CentOS) across VMware and Azure hybrid environments.
* Directed day-2 OpenShift cluster operations, including worker node scaling, CrashLoopBackOff resolution, and Security Context Constraints (SCC).
* Achieved **100% internal audit compliance** by strictly hardening servers via SELinux policies, Fail2ban, and Trivy vulnerability scanning.

### 🚀 IT Technical Manager / Security Administrator | Real Estate IQ
*April 2019 – September 2023*
* Deployed Falco and KubeArmor for real-time threat detection across production Linux-based web servers.
* Led the seamless migration of legacy AWS Linux instances into secure, modern architectures using Terraform/OpenTofu and Ansible.

### 🚀 Tier 3 Systems Administrator | SilverNetworks
*February 2017 – April 2019*
* Maintained 40+ production RHEL/CentOS servers, performing deep kernel-level performance tuning (sysctl, systemd).
* Scripted and fully automated WHMCS and Discourse deployments utilizing custom Bash and Python automation.

*(Note: Additional earlier history from 2007–2017 available upon request, including IT Dept. Head at Callbox and Web Server Admin at HP Outsourcing).*

---

## 📂 Featured Enterprise Projects

### AI, Agents & Automation
* 🤖 **Zero Trust AI Databank (Enterprise RAG Protocol):** Serverless AI command center designed to replace bloated enterprise CRMs — Cloudflare Vectorize for semantic search, D1 for structured text memory, and AI Gateway query caching driving token burn to absolute zero; MCP wiring connects internal data sources to public LLMs (BAAI embeddings + Llama instruction models) without data leakage or hallucination.
* 🤖 **MCP-Driven AIOps Pipeline:** Wired LLM agents (Claude + Model Context Protocol) into Jira, Confluence, Bitbucket, and Datadog — automating incident triage, deployment pre-flight validation, worklog/ticket hygiene, and runbook generation for an enterprise legal-tech platform.
* 🤖 **Internal RAG Chatbot Platform:** Self-hosted n8n + Elasticsearch retrieval pipelines that let engineers query logs and infrastructure state in natural language, cutting log-analysis toil and enabling proactive remediation.
* 🤖 **Vector-Search Ready Data Platform:** PostgreSQL 16 + pgvector on RDS backing semantic search and RAG workloads, fed by an S3 medallion data lake (Glue/Athena) with Lake Formation PII masking.

### High-Concurrency & Decoupled Architecture
* 🔗 **Global Enterprise Web Architecture:** Multi-region, high-availability platform engineered to sustain millions of concurrent user sessions — Edge caching, global load balancing, and auto-scaling Kubernetes guaranteeing 99.999% uptime during massive traffic spikes.
* 🔗 **Enterprise Proxy Engine:** Custom proxy gateway on bare-metal OVH Linux routing high-volume traffic through 30,000 upstream mobile proxy ports to bypass strict enterprise anti-bot systems (Datadome, PerimeterX).
* 🔗 **Decoupled AWS S3 Architecture (Cypress Genesis):** Headless AWS S3 + CloudFront CDN architecture serving 600GB of biological data with 99.999% durability and zero server CPU overload.

### Edge Computing & IAM
* 🔗 **Serverless Edge Auth Gateway:** Zero-latency OAuth2 proxy on Cloudflare Workers enabling secure authentication for Headless/Git-based CMSs without a monolithic backend.

### Legacy Enterprise Builds
* 🔗 **Osiris Browser Infrastructure (Decenternet):** Secure Linux backend for 10M+ users using RHEL and Docker.
* 🔗 **Coineru Cryptocurrency Platform:** Highly available Kubernetes clusters on Ubuntu for high-frequency trading.

---

## 🎓 Education & Fundamentals

**BS Information Technology** | *AMA Computer College (March 2007)*
*Focus: Unix/Linux System Administration, Network Security, Scripting*

<br/>
<div align="center">
  <i>Currently accepting select enterprise contracts, AI platform engineering, and Fractional CTO roles.</i><br/><br/>
  <a href="https://github.com/rojohnh">
    <img src="https://github-readme-stats.vercel.app/api?username=rojohnh&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0f172a" alt="Rojohn's GitHub Stats" />
  </a>
</div>
