# Hi, I'm Ahmed Elgammal

**Junior DevSecOps Engineer** · AWS Certified Cloud Practitioner · Cairo, Egypt

I build and secure delivery pipelines: containerized applications, CI/CD automation with security gates, Kubernetes workloads and cloud infrastructure. Before moving into DevOps I worked as a freelance full-stack developer (since 2021), so I know what developers need from a pipeline and what production troubleshooting looks like.

- Currently: **DevOps Intern at [CodeAlpha](https://www.codealpha.tech)** (since Oct 2026)
- Focus: DevSecOps, SAST / SCA / DAST in CI/CD, container security, OWASP Top 10
- Open to Junior DevSecOps, DevOps, Cloud Support and DevSecOps Intern roles (on-site, hybrid or remote)

## Tech stack

**Cloud & IaC**
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonwebservices&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat&logo=microsoftazure&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-844FBA?style=flat&logo=terraform&logoColor=white)

**Containers & orchestration**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat&logo=helm&logoColor=white)

**CI/CD & security**
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat&logo=jenkins&logoColor=white)
![Azure Pipelines](https://img.shields.io/badge/Azure_Pipelines-2560E0?style=flat&logo=azurepipelines&logoColor=white)
![Trivy](https://img.shields.io/badge/Trivy-1904DA?style=flat&logo=aqua&logoColor=white)
![OWASP](https://img.shields.io/badge/OWASP_Top_10-000000?style=flat&logo=owasp&logoColor=white)

**Linux & tooling**
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat&logo=gnubash&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat&logo=nginx&logoColor=white)

**Development**
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat&logo=php&logoColor=white)
![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=flat&logo=laravel&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat&logo=expo&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat&logo=go&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)

## Experience

**DevOps Intern, [CodeAlpha](https://www.codealpha.tech)** · Remote · Oct 2026 - present
- Jenkins Remoting with x86_64 and ARM64 agents over JNLP4/TLS, configured as code (JCasC + Job DSL)
- Java 21 build automation with Gradle, JUnit 5, a JaCoCo coverage gate and a GitHub Actions → GHCR pipeline
- Hardened Nginx container with health checks, monitoring and 13 automated smoke tests
- Azure Pipelines CI/CD to ACR and App Service with Bicep

**Freelance Developer & DevOps Support** · Self-employed · 2021 - present
- Built and run eight production SaaS and e-commerce platforms for clients in Saudi Arabia, Kuwait and Egypt ([see below](#production-client-work))
- Deployment, hosting and production troubleshooting (Linux, DNS, HTTPS, MySQL, Docker), payment integrations (MyFatoorah, Tabby, Tamara) and app-store releases

## Featured work

**[Aegis: end-to-end DevSecOps platform](https://github.com/ahmedelgmal310/aegis-devsecops)**

Secures the full path from `git push` to a running pod. Code passes secret scanning, SAST, SCA and IaC gates; the image is built multi-arch, scanned, signed with Sigstore (keyless) and ships with a signed SBOM, a signed vulnerability report and SLSA provenance. In the cluster, Kyverno admits only images signed by this pipeline with no critical CVEs, Falco detects attacker behaviour at runtime, secrets are sealed, and Argo CD deploys from Git. When Falco catches an attack, a Go incident responder isolates the pod within milliseconds, preserves the evidence and lets Kubernetes replace it. Every release the pipeline attacks its own cluster and fails if anything gets through.

![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white)
![Sigstore](https://img.shields.io/badge/Sigstore_cosign-2B2D42?style=flat&logo=sigstore&logoColor=white)
![Kyverno](https://img.shields.io/badge/Kyverno-FF6B00?style=flat)
![Falco](https://img.shields.io/badge/Falco-00AEC7?style=flat&logo=falco&logoColor=white)
![Argo CD](https://img.shields.io/badge/Argo_CD-EF7B4D?style=flat&logo=argo&logoColor=white)
![Trivy](https://img.shields.io/badge/Trivy-1904DA?style=flat&logo=aqua&logoColor=white)
![OWASP ZAP](https://img.shields.io/badge/OWASP_ZAP-000000?style=flat&logo=owasp&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat&logo=go&logoColor=white)

**[Serverless Image Processing Pipeline](https://github.com/ahmedelgmal310/Serverless-Image-Processing-Pipeline)** · [live demo](https://d3l1cbrdqvb1hz.cloudfront.net)

Event-driven image service built only from managed AWS services: uploads land in S3, events are buffered in SQS, and a Step Functions workflow validates each image, creates three renditions in parallel with Lambda, watermarks one and records the result in DynamoDB. Images are served through CloudFront. The whole stack is one SAM/CloudFormation template that deploys with a single command.

![AWS SAM](https://img.shields.io/badge/AWS_SAM-FF9900?style=flat&logo=amazonwebservices&logoColor=white)
![Step Functions](https://img.shields.io/badge/Step_Functions-E7157B?style=flat&logo=amazonwebservices&logoColor=white)
![Lambda](https://img.shields.io/badge/Lambda-FF9900?style=flat&logo=awslambda&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)

**[codealpha_tasks](https://github.com/ahmedelgmal310/codealpha_tasks)**: DevOps internship projects

| Project | Highlights |
|---|---|
| [CI/CD with Azure](https://github.com/ahmedelgmal310/codealpha_tasks/tree/main/CodeAlpha_Azure_CICD_Pipeline) | Azure Pipelines → ACR → App Service, Bicep, managed identity, post-deploy verification |
| [Jenkins Remoting](https://github.com/ahmedelgmal310/codealpha_tasks/tree/main/CodeAlpha_Jenkins_Remoting) | Controller + amd64/arm64 inbound agents, JCasC, node isolation checks |
| [Java with Gradle](https://github.com/ahmedelgmal310/codealpha_tasks/tree/main/CodeAlpha_Java_Gradle_App) | Gradle 9, version catalog, coverage gate, GitHub Actions → GHCR |
| [Web server in Docker](https://github.com/ahmedelgmal310/codealpha_tasks/tree/main/CodeAlpha_Docker_Web_Server) | Hardened Nginx container, health checks, monitoring and smoke tests |

Other hands-on work: DevSecOps pipelines with Trivy image scanning and security gates, Kubernetes deployments on kind (probes, rolling updates, ConfigMaps/Secrets, Helm), and AWS networking (VPC, subnets, security groups, EC2, RDS, IAM).

## Production client work

Platforms I built and run for clients, live in production with real users and payments. The source code is private; the links go to the live products.

| Product | What it is | Stack |
|---|---|---|
| **[Muallim+](https://taleemzaki.com)** | AI-powered multi-tenant education SaaS for teachers and students in Kuwait, Saudi Arabia and Egypt: AI exam and lesson builders grounded in the curriculum, live quizzes, adaptive practice, per-country billing | Laravel 13, Inertia, React 19, MariaDB |
| **[Taaqod](https://contract-sa.com)** | Contract management SaaS for healthcare staffing: e-signatures, approval engine, budgets, 77-permission RBAC, SaaS and Ed25519-licensed self-hosted editions | PHP 8.3, React 19, MySQL |
| **[Takamul Plus](https://takamul-plus.com)** | Modular HR, payroll and finance suite: recruitment, attendance, payroll posted to double-entry accounting, approvals and forms engines | React 19, PHP, MySQL |
| **[Hasybat](https://hasybat.com)** | Cloud accounting: ZATCA e-invoicing, VAT, inventory at weighted average cost, automatic ledger | React 19, PHP, MySQL |
| **[Koswmat](https://koswmat.com)** | Deals and appointments marketplace with QR tickets, four role-based panels and an iOS/Android app | Expo / React Native, React, PHP |
| **[2B Store](https://2b-sa.com)** | E-commerce platform: storefront, 30-screen admin dashboard and native app on the App Store and Google Play | React, Expo, PHP, MySQL |
| **[Bazzar 3D](https://bazzar3d.com)** | Interior design and 3D visualization platform: quotes, bookings, BNPL payments, admin panel | React 19, PHP, MySQL |
| **[Saba Design](https://saba-design.com)** | Design-services storefront with cart, payments, abandoned-cart recovery and a partner API | React 19, PHP, MySQL |

## Certifications & education

- **AWS Certified Cloud Practitioner**, Amazon Web Services (Sep 2026)
- **Full-Stack Web Development using .NET**, Information Technology Institute (ITI), 120 hours
- **B.Eng. Communication and Computer Engineering**, Mansoura University (2019 - 2024), GPA 3.57 / 4.00

## Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ahmed-elgammal-ab730a1b1/)
[![Portfolio](https://img.shields.io/badge/Portfolio-elgamal.codlek.com-111111?style=flat&logo=googlechrome&logoColor=white)](https://elgamal.codlek.com)
