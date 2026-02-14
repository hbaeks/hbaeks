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
  <a href="https://aws.amazon.com/" target="_blank">
    <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white" />
  </a>
  <a href="https://azure.microsoft.com/" target="_blank">
    <img src="https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" />
  </a>
  <a href="https://cloud.google.com/" target="_blank">
    <img src="https://img.shields.io/badge/GCP-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white" />
  </a>
  <a href="https://www.ncloud.com/" target="_blank">
    <img src="https://img.shields.io/badge/Naver%20Cloud-03C75A?style=for-the-badge&logo=naver&logoColor=white" />
  </a>
  <a href="https://www.alibabacloud.com/" target="_blank">
    <img src="https://img.shields.io/badge/Alibaba%20Cloud-FF6A00?style=for-the-badge&logo=alibabacloud&logoColor=white" />
  </a>
</p>

### 📊 Observability & Monitoring
<p>
  <a href="https://prometheus.io/" target="_blank">
    <img src="https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white" />
  </a>
  <a href="https://grafana.com/" target="_blank">
    <img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white" />
  </a>
  <a href="https://newrelic.com/" target="_blank">
    <img src="https://img.shields.io/badge/New%20Relic-1CE783?style=for-the-badge&logo=newrelic&logoColor=white" />
  </a>
  <a href="https://www.datadoghq.com/" target="_blank">
    <img src="https://img.shields.io/badge/Datadog-632CA6?style=for-the-badge&logo=datadog&logoColor=white" />
  </a>
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
