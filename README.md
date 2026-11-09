# 👋 Hi, I'm Deen Ojo - AI Systems Engineer

<div align="center">
  
[![Portfolio](https://img.shields.io/badge/Portfolio-SRE%20Projects-blue?style=for-the-badge&logo=github)](https://github.com/deenojo/SRE-Portfolio)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/deenojo)
[![Email](https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:olaitan.ojo@outlook.com)

</div>

## 🚀 AI Systems Engineer · Reliability & Security · MS AI Systems Management @ CMU

I build **AI systems that are reliable and secure in production**: from SRE/DevOps and **infrastructure automation** to **AI agents**, **LLM guardrails** and **DevSecOps**. Background in Azure DevOps for banking infrastructure; currently pursuing an **MS in AI Systems Management at Carnegie Mellon**.

### 🔧 What I Do
- 🏗️ **Infrastructure as Code** - Terraform, Kubernetes, AWS/GCP/Azure
- 📊 **Observability** - Prometheus, Grafana, ELK Stack, Distributed Tracing  
- 🚨 **Incident Response** - Chaos Engineering, Automated Runbooks, SLO Management
- 🚀 **CI/CD & Deployment** - Blue-Green, Canary, GitOps, Advanced Deployment Strategies
- 📈 **Capacity Planning** - ML-powered forecasting, Cost optimization, Resource management
- 🛡️ **DevSecOps & AI Security** - Vulnerability remediation, supply-chain security, LLM guardrails and red-teaming

---

## 🛡️ Featured: AI Security & DevSecOps

### 🩹 [Patchwarden: Self-Healing Vulnerability Remediation Agent](https://github.com/deenojo/Vulnerability-Remediation-Agent)
An AI agent that finds vulnerabilities, triages them by real reachability, opens the **smallest safe fix PRs**, and patches containers in place, while a deterministic policy gate decides what ships.
- 1,596 raw findings → 1,392 unique (Trivy + OSV-Scanner); **Claude triage agrees with hand labels 71% vs 43%** for rules alone
- Smallest-safe-upgrade fixes: **4 of 4 PRs pass CI** (vs 5 of 6 failing with newest-version bumps)
- Container self-heal: **287 OS CVEs → 0**, verified, signed with Sigstore, rolled out to Kubernetes
- Red-teamed: even a fully compromised model can't make it ship anything dangerous

[▶ 3-min demo](https://youtu.be/qShgD-97AX4) · [📊 Live dashboard](https://deenojo.github.io/Vulnerability-Remediation-Agent/) · [Threat model](https://github.com/deenojo/Vulnerability-Remediation-Agent/blob/main/THREAT_MODEL.md)

### 🧱 [PromptWall: LLM Runtime Security Gateway](https://github.com/deenojo/PromptWall)
A gateway in front of production LLM features: blocks prompt injection, quarantines poisoned documents, stops PII/secret leaks, and enforces tool-call policy.
- Against real Claude, 5 trials per attack: **4 of 80 attacks landed alone → 0 of 80 with PromptWall**
- Stopped zero-click exfiltration through a poisoned document that fooled the model 4 of 5 times
- **0 of 60** benign requests over-blocked · under 0.1 ms overhead · mapped to the OWASP Top 10 for LLM apps
- Red-teamed with NVIDIA garak (370 attacks): found and fixed 3 output-handling bugs; XSS/exfiltration **27/41 → 0/41** in the worst case

### 🏰 [TenantGuard: Secure Baseline for Customer-Cloud Deployments](https://github.com/deenojo/TenantGuard)
A hardened Terraform module for deploying a product into a customer's Azure subscription: nothing public, managed identities only, HSM-backed keys, every resource logged, and Azure Policy guardrails against drift.
- Checkov **54 passed, 0 failed** · **9/9** security tests on a mock provider (no Azure account needed)
- **6 custom deny policies** + the CIS Azure Foundations initiative · **10 alerts** on security-relevant changes

### 🔎 [Pen Test → Remediation Playbook](https://github.com/deenojo/Vulnerable-App-Pen-Test)
Takes common web-app pen-test findings and closes them for good: every OWASP Top 10 issue gets a fix, a regression test, and a static-analysis rule that fails CI if it returns.
- **6 findings remediated** (1 Critical, 4 High, 1 Medium) across 5 OWASP Top 10 categories
- **18 regression tests** + **5 self-tested Semgrep rules** · CI runs pytest · Semgrep · Bandit · pip-audit, all green

---

## 🏆 Featured SRE Portfolio Projects

### 🏗️ Portfolio Architecture Overview
```mermaid
graph TB
    subgraph "SRE Core Competencies"
        A1[Observability & Monitoring]
        A2[Infrastructure Automation]
        A3[Incident Response]
        A4[Deployment Engineering]
        A5[Capacity Planning]
    end
    
    subgraph "Portfolio Projects"
        B1[Prometheus Monitoring Stack]
        B2[Infrastructure as Code]
        B3[Incident Response Toolkit]
        B4[CI/CD Pipeline Platform]
        B5[Capacity Planning System]
        B6[Log Aggregation System]
    end
    
    subgraph "Technology Ecosystem"
        C1[Cloud Platforms]
        C2[Container Orchestration]
        C3[Monitoring Tools]
        C4[Automation Frameworks]
        C5[ML/AI Integration]
    end
    
    A1 --> B1
    A1 --> B6
    A2 --> B2
    A3 --> B3
    A4 --> B4
    A5 --> B5
    
    B1 --> C3
    B2 --> C1
    B3 --> C4
    B4 --> C2
    B5 --> C5
    B6 --> C3
```

<div align="center">

### 📊 [Production Monitoring Stack](https://github.com/deenojo/prometheus-monitoring-stack)
**Prometheus + Grafana + AlertManager**  
*Enterprise-grade monitoring with SLI/SLO tracking and intelligent alerting*

### 🚨 [Incident Response Toolkit](https://github.com/deenojo/incident-response-toolkit)  
**Chaos Engineering + Incident Management**  
*Complete incident response platform with automated chaos experiments*

### 📝 [Log Aggregation System](https://github.com/deenojo/log-aggregation-system)
**ELK Stack + Real-time Analysis**  
*Centralized logging with ML-powered anomaly detection*

### 📈 [Capacity Planning Platform](https://github.com/deenojo/capacity-planning-system)
**ML Forecasting + Cost Optimization**  
*AI-powered resource planning with 40% cost reduction*

### 🏗️ [Infrastructure as Code](https://github.com/deenojo/infrastructure-as-code)
**Terraform + Kubernetes + Multi-Cloud**  
*Production-ready IaC with advanced EKS modules and governance*

### 🚀 [CI/CD Pipeline Platform](https://github.com/deenojo/ci-cd-pipeline)
**Blue-Green + Canary + GitHub Actions**  
*Enterprise CI/CD with advanced deployment strategies*

</div>

---

## 📊 GitHub Metrics

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=deenojo&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=deenojo&layout=compact&theme=tokyonight&hide_border=true&langs_count=8)

</div>

<div align="center">

![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=deenojo&theme=tokyonight&hide_border=true)

</div>

---

## 🛠️ Tech Stack & Tools

<div align="center">

### ☁️ Cloud & Infrastructure
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)
![GCP](https://img.shields.io/badge/GCP-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoft-azure&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-623CE4?style=for-the-badge&logo=terraform&logoColor=white)

### 📊 Monitoring & Observability  
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)
![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?style=for-the-badge&logo=elasticsearch&logoColor=white)
![Kibana](https://img.shields.io/badge/Kibana-005571?style=for-the-badge&logo=kibana&logoColor=white)
![Jaeger](https://img.shields.io/badge/Jaeger-66CFE3?style=for-the-badge&logo=jaeger&logoColor=white)

### 🚀 CI/CD & Automation
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![GitLab CI](https://img.shields.io/badge/GitLab_CI-FCA326?style=for-the-badge&logo=gitlab&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white)
![ArgoCD](https://img.shields.io/badge/ArgoCD-EF7B4D?style=for-the-badge&logo=argo&logoColor=white)

### 💻 Languages & Frameworks
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white)

### 🗄️ Databases & Storage
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![InfluxDB](https://img.shields.io/badge/InfluxDB-22ADF6?style=for-the-badge&logo=influxdb&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)

</div>

---

## 🎯 SRE Expertise & Achievements

<div align="center">

| 🎯 **Area** | 📊 **Achievement** | 🏆 **Impact** |
|------------|-------------------|---------------|
| **Reliability** | 99.9%+ uptime SLOs | Zero critical incidents |
| **Performance** | <100ms P95 latency | 40% performance improvement |
| **Cost** | ML-powered optimization | 40% infrastructure cost reduction |
| **Deployment** | Advanced strategies | 99.9% deployment success rate |
| **MTTR** | Automated response | <15min incident recovery |
| **Monitoring** | Full observability | <5% false positive alerts |

</div>

---

## 🏅 DORA Metrics Performance

<div align="center">

| 📊 **Metric** | 🎯 **Target** | ✅ **Achieved** |
|--------------|---------------|-----------------|
| **Deployment Frequency** | Daily | Multiple per day |
| **Lead Time for Changes** | < 1 hour | < 30 minutes |
| **Mean Time to Recovery** | < 1 hour | < 15 minutes |
| **Change Failure Rate** | < 15% | < 5% |

</div>

---

## 📝 Recent Activity

<!--START_SECTION:activity-->
1. 🎉 Merged PR [#11](https://github.com/deenojo/Vulnerability-Remediation-Agent/pull/11) in [deenojo/Vulnerability-Remediation-Agent](https://github.com/deenojo/Vulnerability-Remediation-Agent)
2. 💪 Opened PR [#11](https://github.com/deenojo/Vulnerability-Remediation-Agent/pull/11) in [deenojo/Vulnerability-Remediation-Agent](https://github.com/deenojo/Vulnerability-Remediation-Agent)
<!--END_SECTION:activity-->

---

## 📈 Current Focus & Learning

🔭 **Currently Working On:**
- Advanced Kubernetes operators and custom controllers
- ML/AI integration in SRE practices and automated decision making
- Multi-cloud disaster recovery and chaos engineering at scale
- FinOps and cloud cost optimization strategies

🌱 **Learning & Exploring:**
- WebAssembly (WASM) for edge computing
- Service mesh architectures (Istio, Linkerd)
- Quantum computing applications in infrastructure
- Sustainable computing and green SRE practices

---

## 🏆 Certifications & Achievements

<div align="center">

![AWS](https://img.shields.io/badge/AWS_Certified-Solutions_Architect-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Kubernetes](https://img.shields.io/badge/CKA-Certified_Kubernetes_Administrator-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Terraform](https://img.shields.io/badge/HashiCorp-Terraform_Associate-623CE4?style=for-the-badge&logo=terraform&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-Certified_Associate-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)

</div>

---

## 📫 Let's Connect!

<div align="center">

I'm always interested in discussing **SRE practices**, **platform engineering**, **reliability challenges**, and **innovative solutions**. Let's connect and share knowledge!

[![Portfolio](https://img.shields.io/badge/📁_Portfolio-SRE_Projects-4285F4?style=for-the-badge)](https://github.com/deenojo/SRE-Portfolio)
[![LinkedIn](https://img.shields.io/badge/💼_LinkedIn-Connect-0077B5?style=for-the-badge)](https://www.linkedin.com/in/deenojo)
[![Email](https://img.shields.io/badge/📧_Email-Contact-EA4335?style=for-the-badge)](mailto:olaitan.ojo@outlook.com)

</div>

---

<div align="center">

### 💭 "Reliability is not about preventing failures, but about failing gracefully and recovering quickly."

![Profile Views](https://komarev.com/ghpvc/?username=deenojo&color=blueviolet&style=for-the-badge&label=Profile+Views)

⭐ **Star my repositories if you find them helpful!**  
🤝 **Always open to collaboration and learning opportunities**

</div>

---

<details>
<summary>📊 <b>Detailed GitHub Analytics</b></summary>

![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=deenojo&theme=tokyo-night&hide_border=true)

![GitHub Trophies](https://github-profile-trophy.vercel.app/?username=deenojo&theme=tokyonight&no-frame=true&no-bg=true&row=1&column=6)

</details>
