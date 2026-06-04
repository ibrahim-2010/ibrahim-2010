# Ibrahim Jinadu – DevOps & Cloud Infrastructure Engineer

**7+ years** building and operating production AWS infrastructure. I specialise in EKS platform engineering, DevSecOps pipelines, and GitOps delivery. Currently open to **DevOps Engineer · SRE · Platform Engineer · Cloud Infrastructure Engineer** roles – remote or hybrid.

📍 &nbsp;[linkedin.com/in/ibrahim-jinadu-2388b73b8](https://www.linkedin.com/in/ibrahim-jinadu-2388b73b8/) &nbsp;|&nbsp; 🏅 &nbsp;AWS Certified Solutions Architect · AWS Cloud Practitioner

---

## 🔧 Core Stack

| Domain | Technologies |
|---|---|
| **Cloud & IaC** | AWS (EKS, RDS, ElastiCache, ECR, ALB, Route 53, Secrets Manager) · Terraform |
| **Kubernetes** | EKS · ArgoCD App-of-Apps · Kyverno · External Secrets Operator · Karpenter |
| **CI/CD** | Jenkins (JCasC) · GitHub Actions · SonarQube · Trivy · Docker · ECR |
| **Observability** | Prometheus · Grafana · Loki · Tempo · Promtail · AlertManager |
| **Security** | IRSA · Kyverno admission control · Falco · GuardDuty · Cosign/Sigstore |
| **Messaging** | Strimzi Kafka (KRaft) · Redis · RabbitMQ |
| **Languages** | Python · Bash · HCL · YAML |

---

## 🚀 Featured Projects

### [NimbusRetail Platform](https://github.com/ibrahim-2010/nimbus-retail-platform)
Production-grade cloud-native e-commerce platform on AWS EKS. Five microservices (Node.js + Python FastAPI) communicating over HTTP and Kafka. Full GitOps delivery via ArgoCD App-of-Apps. Zero hardcoded credentials – ESO syncs secrets from AWS Secrets Manager via IRSA at pod startup. Kyverno enforces resource limits and blocks privileged containers. Full observability: Prometheus metrics, Loki logs, Tempo traces, five PrometheusRule alerts.

`Terraform` `EKS` `ArgoCD` `Strimzi Kafka` `Kyverno` `ESO + IRSA` `Prometheus` `Loki` `Tempo` `Jenkins JCasC`

> 19 real production issues documented with root cause and fix – not a tutorial.

---

### [Operator Copilot](https://github.com/ibrahim-2010/operator-copilot-starter)
AI-powered SRE first-responder agent built on the Anthropic API and Model Context Protocol. Connects to a live EKS cluster, diagnoses Kafka consumer lag, CrashLoopBackOff, and TLS expiry, then proposes remediations blocked behind a human approval gate. The gate is enforced in the MCP server code – the LLM cannot self-approve. Every tool call is written to an append-only audit log (JSONL). Rate-limited at 20 calls/tool/60s.

`Python` `Anthropic API` `MCP` `Kubernetes Python client` `Prometheus AlertManager` `cert-manager`

> 12 tools (8 read-only, 4 mutating). Approval gate enforced in server, not prompt.

---

### [Cloud-Native DevSecOps EKS](https://github.com/ibrahim-2010/cloud-native-eks)
Three-tier app (React + Node.js + PostgreSQL + Redis) on AWS EKS with a fully automated lifecycle. Jenkins JCasC auto-configures 102 plugins, credentials, and pipeline jobs – zero UI clicking. ExternalDNS creates Route 53 records automatically from Ingress annotations. Nine-stage DevSecOps pipeline: SonarQube quality gate → Trivy CVE scan → ECR push → ArgoCD GitOps rollout.

`Terraform` `EKS` `Jenkins JCasC` `ArgoCD` `SonarQube` `Trivy` `ExternalDNS` `Prometheus` `Grafana`

> 17 production issues documented across 4 deployment cycles.

---

### [DevSecOps Three-Tier EKS](https://github.com/ibrahim-2010/DevSecOps-Three-Tier-EKS)
End-to-end DevSecOps pipeline deploying a React + Node.js + MongoDB three-tier application to AWS EKS. Built and validated with 2026 tooling: Jenkins GPG key, Java 21, EBS CSI driver for EKS 1.34, CVSS v4 parser workaround.

`Terraform` `EKS 1.34` `Jenkins` `ArgoCD` `SonarQube` `Trivy` `Prometheus` `Grafana`

> 16 real issues documented – including the upstream OWASP CVSS v4 parser bug.

---

### [AWS Cost Optimization](https://github.com/ibrahim-2010/aws-cost-optimization)
Four-phase FinOps framework deployed against a real AWS environment. Automated audit surfaced an EC2 instance at 0.18% average CPU, unattached EBS volumes, and an orphaned Elastic IP – none visible in the monthly bill. Terraform modules for budget alerts (80/100/120% thresholds + anomaly detection), tag enforcement via AWS Config, and scheduled Lambda shutdown/startup.

`Terraform` `Python (boto3)` `AWS Budgets` `Cost Explorer` `Lambda` `EventBridge` `AWS Config`

---

### [Jenkins CI/CD to EKS](https://github.com/ibrahim-2010/cicd_jenkins)
Six-stage Jenkins pipeline: Maven unit tests → Docker build → DockerHub push → EKS deployment → Prometheus/Grafana monitoring. Full pipeline completes in ~25 seconds. Custom PrometheusRule alerts for PodDown, HighCPU, and CrashLooping – validated live.

`Jenkins` `Maven` `Docker` `EKS` `Prometheus` `Grafana`

---

## 📊 Experience Snapshot

| Role | Company | Period |
|---|---|---|
| Senior SRE Consultant | Technology Excellence Services | Mar 2024 – Present |
| Site Reliability Engineer | Körber Supply Chain | Dec 2022 – Feb 2024 |
| DevOps Engineer | Technology Excellence Services | Mar 2019 – Dec 2022 |
| Linux Systems Administrator | Platinum Group | Jun 2016 – Jan 2019 |

---

*Open to remote and hybrid opportunities. Connect on [LinkedIn](https://www.linkedin.com/in/ibrahim-jinadu-2388b73b8/) or reach out directly.*
