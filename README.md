<h1 align="center">hbaeks</h1>
<p align="center">
  <b>Infrastructure Specialist · SRE · DevSecOps · Platform Engineering</b><br/>
  Reliability · Multi-Cloud · Kubernetes · Observability · FinOps · Team Leadership
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/paekheon/">LinkedIn</a> ·
  <a href="mailto:paekheon@gmail.com">paekheon@gmail.com</a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=hbaeks&style=flat"/>
  <img src="https://img.shields.io/github/followers/hbaeks?style=flat"/>
</p>

---

## 🧭 Professional Focus

- Infrastructure Architecture & Multi-Cloud Strategy  
- Service Reliability Engineering & Incident Leadership  
- Kubernetes Platform Engineering (EKS)  
- DevSecOps & CI/CD Automation  
- FinOps & Cost Optimization  
- Technical Team Leadership  

---

## 🧰 Core Technology Stack

### ☁️ Cloud Platforms
<p>
  <a href="https://aws.amazon.com/">
    <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white"/>
  </a>
  <a href="https://azure.microsoft.com/">
    <img src="https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white"/>
  </a>
  <a href="https://cloud.google.com/">
    <img src="https://img.shields.io/badge/GCP-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white"/>
  </a>
  <a href="https://www.ncloud.com/">
    <img src="https://img.shields.io/badge/Naver%20Cloud-03C75A?style=for-the-badge&logo=naver&logoColor=white"/>
  </a>
  <a href="https://www.alibabacloud.com/">
    <img src="https://img.shields.io/badge/Alibaba%20Cloud-FF6A00?style=for-the-badge&logo=alibabacloud&logoColor=white"/>
  </a>
</p>

---

### 🏗 Infrastructure as Code (IaC)
<p>
  <a href="https://www.terraform.io/">
    <img src="https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white"/>
  </a>
  <a href="https://aws.amazon.com/cloudformation/">
    <img src="https://img.shields.io/badge/AWS%20CloudFormation-FF4F00?style=for-the-badge&logo=amazonaws&logoColor=white"/>
  </a>
  <a href="https://www.ansible.com/">
    <img src="https://img.shields.io/badge/Ansible-EE0000?style=for-the-badge&logo=ansible&logoColor=white"/>
  </a>
  <a href="https://helm.sh/">
    <img src="https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white"/>
  </a>
</p>

---

### 🔄 CI / CD & Automation
<p>
  <a href="https://github.com/features/actions">
    <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white"/>
  </a>
  <a href="https://www.jenkins.io/">
    <img src="https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white"/>
  </a>
  <a href="https://argo-cd.readthedocs.io/">
    <img src="https://img.shields.io/badge/ArgoCD-EF7B4D?style=for-the-badge&logo=argo&logoColor=white"/>
  </a>
</p>

---

### 📊 Observability & Monitoring
<p>
  <a href="https://prometheus.io/">
    <img src="https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white"/>
  </a>
  <a href="https://grafana.com/">
    <img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white"/>
  </a>
  <a href="https://newrelic.com/">
    <img src="https://img.shields.io/badge/New%20Relic-1CE783?style=for-the-badge&logo=newrelic&logoColor=white"/>
  </a>
  <a href="https://www.datadoghq.com/">
    <img src="https://img.shields.io/badge/Datadog-632CA6?style=for-the-badge&logo=datadog&logoColor=white"/>
  </a>
</p>

---

## 📊 GitHub Analytics

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=hbaeks&show_icons=true"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=hbaeks&layout=compact"/>
</p>

---

## 🗺️ Platform Architecture

```mermaid
flowchart LR
  U[Users] --> CDN[CDN / WAF]
  CDN --> LB[Load Balancer / Ingress]
  LB --> K8S[Kubernetes Platform]
  K8S --> SVC[Services]
  SVC --> DB[(Database)]
  SVC --> CACHE[(Cache)]
  SVC --> MQ[(Message Queue)]
  SVC --> EXT[External APIs]

flowchart TB
  APP[Apps / Pods] -->|metrics| PROM[Prometheus]
  PROM --> GRAF[Grafana]
  APP -->|logs| LOGS[Log Pipeline]
  APP -->|APM| APM[APM Agents]
  APM --> NR[New Relic]
  APM --> DD[Datadog]
  GRAF --> ALERT[Alerting]

sequenceDiagram
  participant Dev as Developer
  participant GH as GitHub
  participant GA as GitHub Actions
  participant REG as Container Registry
  participant ARGO as Argo CD
  participant K8S as Kubernetes (EKS)

  Dev->>GH: Push / Merge
  GH->>GA: Trigger CI
  GA->>GA: Test & Build
  GA->>REG: Push Image
  GA->>GH: Update Manifest
  GH->>ARGO: Sync
  ARGO->>K8S: Deploy
  K8S-->>ARGO: Health Check
