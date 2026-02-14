<h1 align="center">hbaeks</h1>
<p align="center">
  <b>Infrastructure Specialist · SRE · DevSecOps · Platform Engineering</b><br/>
  Reliability · Kubernetes · EKS · Observability · FinOps · Team Leadership
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

- **Infrastructure Architecture** — 확장성과 안정성을 고려한 클라우드 아키텍처 설계
- **Service Reliability Engineering** — MTTR 단축, 인시던트 대응 체계 수립
- **Kubernetes Platform Operations** — EKS 기반 무중단 배포 및 운영 표준화
- **DevSecOps Strategy** — CI/CD 자동화, 보안 정책 및 접근 통제 설계
- **FinOps Leadership** — 비용 가시화, 리소스 최적화, 예산 효율화
- **Technical Team Leadership** — 인프라 조직 리딩 및 운영 전략 수립

---

## 🧰 Core Technology Stack

### ☁️ Cloud Platforms
<p>
  <img src="https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonaws&logoColor=white"/>
  <img src="https://img.shields.io/badge/Microsoft_Azure-0078D4?style=flat&logo=microsoftazure&logoColor=white"/>
  <img src="https://img.shields.io/badge/Google_Cloud-4285F4?style=flat&logo=googlecloud&logoColor=white"/>
  <img src="https://img.shields.io/badge/Naver_Cloud-03C75A?style=flat&logo=naver&logoColor=white"/>
  <img src="https://img.shields.io/badge/Alibaba_Cloud-FF6A00?style=flat&logo=alibabacloud&logoColor=white"/>
</p>

---

### 🐳 Container & Orchestration
<p>
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/Helm-0F1689?style=flat&logo=helm&logoColor=white"/>
  <img src="https://img.shields.io/badge/ArgoCD-EF7B4D?style=flat&logo=argo&logoColor=white"/>
</p>

---

### 🏗 Infrastructure as Code
<p>
  <img src="https://img.shields.io/badge/Terraform-7B42BC?style=flat&logo=terraform&logoColor=white"/>
  <img src="https://img.shields.io/badge/Ansible-EE0000?style=flat&logo=ansible&logoColor=white"/>
</p>

---

### 🔄 CI/CD & Automation
<p>
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white"/>
  <img src="https://img.shields.io/badge/Jenkins-D24939?style=flat&logo=jenkins&logoColor=white"/>
</p>

---

### 📊 Observability & Monitoring
<p>
  <img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat&logo=prometheus&logoColor=white"/>
  <img src="https://img.shields.io/badge/Grafana-F46800?style=flat&logo=grafana&logoColor=white"/>
  <img src="https://img.shields.io/badge/New_Relic-1CE783?style=flat&logo=newrelic&logoColor=white"/>
  <img src="https://img.shields.io/badge/Datadog-632CA6?style=flat&logo=datadog&logoColor=white"/>
</p>

---

## 📊 GitHub Analytics

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=hbaeks&show_icons=true"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=hbaeks&layout=compact"/>
</p>

---

## 🗺️ Reference Platform Architecture

```mermaid
flowchart LR
    User --> CDN
    CDN --> ALB
    ALB --> Ingress
    Ingress --> Service
    Service --> Pods
    Pods --> DB[(RDS)]
    Pods --> Cache[(Redis)]
    Pods --> MQ[(Message Queue)]
    Pods --> Metrics[Prometheus]
    Metrics --> Grafana
    Grafana --> Alerting
