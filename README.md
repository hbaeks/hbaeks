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

## 🧰 Core Technology Stackqqq
<div align="center"><h2>🧰 STACKS</h2></div>

<div align="center">

  <!-- Cloud -->
  <h3>☁️ Cloud</h3>
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=FF9900">
  <img src="https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white">
  <img src="https://img.shields.io/badge/GCP-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white">
  <img src="https://img.shields.io/badge/Naver%20Cloud-03C75A?style=for-the-badge&logo=naver&logoColor=white">
  <img src="https://img.shields.io/badge/Alibaba%20Cloud-FF6A00?style=for-the-badge&logo=alibabacloud&logoColor=white">
  <br><br>

  <!-- Kubernetes / Platform -->
  <h3>🧱 Kubernetes & Platform</h3>
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white">
  <img src="https://img.shields.io/badge/Amazon%20EKS-232F3E?style=for-the-badge&logo=amazoneks&logoColor=FF9900">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white">
  <img src="https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white">
   <br><br>

  <!-- IaC -->
  <h3>🏗 IaC</h3>
  <img src="https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white">
  <img src="https://img.shields.io/badge/CloudFormation-232F3E?style=for-the-badge&logo=amazonaws&logoColor=FF9900">
  <img src="https://img.shields.io/badge/Ansible-EE0000?style=for-the-badge&logo=ansible&logoColor=white">
  <br><br>

  <!-- CI/CD -->
  <h3>🔄 CI/CD</h3>
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white">
  <img src="https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white">
  <img src="https://img.shields.io/badge/Argo%20CD-EF7B4D?style=for-the-badge&logo=argo&logoColor=white">
  <br><br>

  <!-- Observability -->
  <h3>📊 Observability</h3>
  <img src="https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white">
  <img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white">
  <img src="https://img.shields.io/badge/New%20Relic-1CE783?style=for-the-badge&logo=newrelic&logoColor=white">
  <img src="https://img.shields.io/badge/Datadog-632CA6?style=for-the-badge&logo=datadog&logoColor=white">
  <br><br>

  <!-- Ops -->
  <h3>🧑‍💻 Ops</h3>
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black">
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white">
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white">

</div>

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
  ```

```mermaid
flowchart TB
  APP[Apps / Pods] -->|metrics| PROM[Prometheus]
  PROM --> GRAF[Grafana]
  APP -->|logs| LOGS[Log Pipeline]
  APP -->|APM| APM[APM Agents]
  APM --> NR[New Relic]
  APM --> DD[Datadog]
  GRAF --> ALERT[Alerting]
  ```


```mermaid
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
```
