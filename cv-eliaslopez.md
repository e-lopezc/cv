# Elias Lopez

**Cloud & Platform Engineer | AWS Infrastructure | Terraform | Kubernetes**

https://www.linkedin.com/in/eliaslopez25  
GitHub: https://github.com/e-lopezc

---

## Professional Summary

Cloud & Platform Engineer with 2+ years of hands-on experience building and improving AWS infrastructure, Kubernetes platforms, and automation for production systems, backed by 7+ years of progressive technical experience overall. Delivered ~$6,960/year in confirmed AWS cost savings for dev account, executed zero-downtime PostgreSQL 13→17 migration, and led infrastructure initiatives across Terraform, GitOps, CI/CD, and platform reliability.

**Core Competencies:** AWS Infrastructure • FinOps/Cost Engineering • Terraform/IaC • PostgreSQL/RDS/Aurora • Kubernetes/EKS • GitOps/FluxCD • Python Automation • DataDog Monitoring • CI/CD • Security & Compliance

---

## Key Achievements

- **FinOps — ~$6,960/year confirmed AWS savings**: Designed first-ever cross-account ECR lifecycle policies; cut dev account cost $22.63 → $4.13/day (-82%), verified via AWS Cost Explorer
- **Zero-downtime PostgreSQL 13→17 production migration** using native logical replication — native logical replication lab dry-run, zero data loss across staging and live
- **Flux/Helm scalability**: Cut helm-controller CPU 91% (596m→56m); EKS spot pools 15→48 across 3 AZs + aws-node-termination-handler graceful drain
- **2026 AZ DR Failover Exercise**: Full staging + live exercise using deployment-affinity AZ exclusion — audit-ready evidence for enterprise contracts
- **Cloud Cost Sentinel** _(side project)_: Containerised AWS cost scanner (ECS Fargate + EventBridge + Terraform) detecting idle EC2, EBS, RDS, S3 resources with scheduled HTML reports and SNS alerts
- **Serverless Product Catalog API** _(side project)_: API Gateway + Lambda (Python) + DynamoDB with event-driven IAM security patterns

---

## Professional Experience

### DevOps Engineer

**Brightflag** | Dublin, Ireland | Jul 2026 - Present

- Design, build, and maintain the infrastructure and systems necessary for the development, testing, and deployment of Brightflag software applications
- Collaborate with cross-functional teams, including developers, QA engineers, and product managers, to define infrastructure requirements, implement solutions, and
  ensure smooth operations
- Develop and maintain CI/CD pipelines, automated deployment scripts, and configuration management systems to streamline software releases and updates
- Implement and maintain observability solutions to proactively identify and resolve system issues, bottlenecks, and performance optimizations
- Continuously improve the scalability, reliability, and security of our infrastructure by leveraging best practices and implementing appropriate tools and technologies
- Collaborate with the security team to ensure compliance with security standards and best practices, including vulnerability management and incident response
- Document system configurations, processes, and troubleshooting procedures to facilitate knowledge sharing and maintain a robust knowledge base

### **SRE Engineer**

**RapidRatings** | Dublin, Ireland | Sept 2023 - Jun 2026

- Delivered ~$6,960/year confirmed AWS savings via first-ever cross-account ECR lifecycle policies (dev / live / staging); dev account daily cost $22.63 → $4.13 (-82%), verified via AWS Cost Explorer
- Consolidated AWS ECR from 2 accounts to 1 across 15+ application repos in a 6-phase rollout; eliminated cross-account replication lag and narrowed OIDC trust to per-repo roles
- Reduced Datadog log ingest costs by shipping cluster-wide Agent filtering rules across all services in live and staging environments
- Executed zero-downtime PostgreSQL 13.22 → 17.6 production migration using native logical replication; built native logical replication lab for dry-run rehearsals, validated post-cutover with zero data loss across staging and live
- Implemented database permission hierarchies across 20+ production databases; patched silent `ALTER DEFAULT PRIVILEGES` gap across 6 databases preventing analyst-facing privilege drift
- Upgraded GitHub self-hosted runner infrastructure (terraform-aws-github-runner v6.10.1 → v7.4.0) via blue-green per-tier rollout with zero CI maintenance window; managed Terraform IaC for ECR consolidation groundwork and multi-environment infrastructure provisioning
- Cut Flux helm-controller CPU by 91% (596m → 56m) by pruning Flux objects for powered-off environments; scaled platform to support 2-3x concurrent demo environments
- Expanded EKS spot instance-type diversity from 5 → 16 (15 → 48 capacity pools across 3 AZs); deployed aws-node-termination-handler for graceful 2-minute drain replacing hard kills
- Stabilised rrtasker Celery fleet (16-ticket campaign): queue-depth monitoring, file-based heartbeat liveness probes, gevent → solo pool migration, soft time limits
- Eliminated recurring 502 errors on primary internal API (rrio) via uWSGI buffer-size, liveness probe, and `reload-mercy` alignment with Kubernetes `terminationGracePeriodSeconds`
- Audited live EKS cluster hygiene: 25+ deployments without CPU requests, zero LimitRanges/PDBs/HPAs; authored 3-tier remediation plan
- Implemented DataDog monitoring: APM across 5 microservices, synthetic monitoring, RDS enhanced metrics, custom alerting
- Designed and implemented API rate limiting for OAuth endpoints
- Coordinated security compliance and vulnerability scanning for enterprise client integrations
- Designed and executed 2026 AZ DR Failover Exercise across staging and live — produced audit-ready DR evidence for enterprise contracts
- Adopted AI-assisted development workflows (Claude Code, GitHub Copilot) to accelerate IaC authoring, automation scripting, and incident investigation — reducing time-to-solution on infrastructure tasks

**Key Technologies:** AWS (RDS, Aurora, EC2, Lambda, S3, ECR, VPC, IAM, CloudWatch, EventBridge, API Gateway, DynamoDB), Terraform, Python, Kubernetes/EKS, FluxCD/Helm, Docker, DataDog, PostgreSQL, GitHub Actions

---

### **Software Engineer**

**RapidRatings** | Dublin, Ireland | Sept 2020 - Sept 2023

- Delivered tier 2/3 technical support for enterprise SaaS platform; independently resolved bugs or escalated based on severity and impact — reducing recurring issues by 25% through incident pattern analysis
- Developed Python automation scripts reducing repetitive manual tasks by 40+ hours monthly
- Supported enterprise client integrations via SSO (SAML 2.0) and REST APIs; performed SQL data extractions from PostgreSQL for customer reporting
- Mentored 5+ new team members on product architecture and troubleshooting methodologies

**Key Technologies:** Python, PostgreSQL, REST APIs, SSO/SAML, OAuth 2.0, SQL, Linux, Git

---

### **Technical Support Engineer**

**RapidRatings** | Dublin, Ireland | Mar 2019 - Sept 2020

- Provided tier 2 technical support for enterprise client-facing teams; delivered technical implementation support for SSO and API integrations
- Created internal knowledge base documenting support processes and SLAs; mentored new team members on product architecture and troubleshooting

---

### **Technical Support Engineer II**

**Rapid7** | Dublin, Ireland | Jul 2017 - Mar 2019

- Resolved escalated security platform issues (Nexpose/InsightVM) on Linux/Windows for enterprise customers; partnered with engineering on root cause analysis and platform defect resolution

---

## Technical Skills

**AWS:** EC2, RDS/Aurora, S3, Lambda, ECR, VPC, IAM, CloudWatch, EventBridge, API Gateway, DynamoDB  
**IaC & Automation:** Terraform, Python (boto3), Bash, GitHub Actions, GitOps/FluxCD  
**Containers & Orchestration:** Kubernetes/EKS, Helm, Docker  
**Databases:** PostgreSQL, Aurora Serverless v2, logical replication, ElasticSearch  
**Observability:** DataDog (APM, synthetics, metrics, alerting), CloudWatch  
**Security:** IAM, SSO/SAML 2.0, OAuth 2.0, ECR scanning, vulnerability management  
**FinOps:** AWS Cost Explorer, ECR lifecycle policies, resource rightsizing, cost allocation  
**OS & Networking:** Linux (RHEL/Ubuntu/Alpine), TCP/IP, DNS, TLS/SSL, VPC design

---

## Education

### **Master of Science in Computer Science**

**University "Centroccidental Lisandro Alvarado"** | Venezuela  
**Thesis:** Cloud Computing Model for E-learning Platform Infrastructure Management  
Focus: Cloud infrastructure design, virtualization, resource optimization

### **Bachelor of Science in Computer Science**

**University "Centroccidental Lisandro Alvarado"** | Venezuela

---

## Certifications & Professional Development

- **AWS Certified Security - Specialty** (2023)
- **Developing on AWS** (2021)

---

## Languages

- **Spanish:** Native
- **English:** Full professional proficiency

---

## Additional Information

**Work Authorization:** Irish Citizen
**Location:** Dublin, Ireland | Open to remote opportunities within EU/UK
**Availability:** 1 month notice period

---

_Last Updated: June 2026_
