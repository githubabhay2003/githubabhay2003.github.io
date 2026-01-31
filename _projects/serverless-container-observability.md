---

layout: default

title: "Serverless Container Observability on AWS"

category: "Personal"

order: 94

tech-stack: "Terraform, AWS ECS Fargate, Prometheus, Grafana"

github-link: "https://github.com/githubabhay2003/serverless-container-observability.git"

summary: "An end-to-end observability platform for a serverless ECS Fargate application using Prometheus, Grafana, and CloudWatch, fully provisioned with Terraform."

---



\# Serverless Container Observability on AWS



This project demonstrates an end-to-end observability setup for a containerized application running on AWS ECS Fargate. Built entirely using Infrastructure as Code (Terraform), it features a Dockerized web application, an Application Load Balancer, and a dedicated, decoupled monitoring stack running Prometheus, Grafana, and the YACE exporter to centralize metrics and logs.



\[Back to Home](/)



---



\### 1. The Goal



Building production-grade observability for serverless containers often leads to either over-engineering or reliance on opaque, expensive managed services. The goal of this project was to prove that a robust, open-source monitoring stack could be built for AWS Fargate without enterprise complexity. The objective was to architect a "glass-box" solution where critical metrics (like ALB latency and ECS resource usage) and application logs are centralized into a single dashboard, provisioned automatically alongside the infrastructure.



---



\### 2. My Role \& Contributions



As the sole engineer for this project, I was responsible for the architecture, implementation, and validation of the observability pipeline.



\* \*\*Architecture Design:\*\* I designed a decoupled architecture that separates the application layer (ECS Fargate) from the monitoring layer (EC2) to ensure that monitoring remains available even if the application cluster faces issues.

\* \*\*Infrastructure as Code:\*\* I developed the modular Terraform codebase to provision the entire stack, managing complex dependencies between the VPC networking, ECS services, and the monitoring instances.

\* \*\*Observability Pipeline Engineering:\*\* I implemented a custom metric collection pipeline using YACE (Yet Another CloudWatch Exporter) to bridge the gap between AWS CloudWatch metrics and Prometheus.

\* \*\*Visualization \& Dashboarding:\*\* I created comprehensive Grafana dashboards that unify disparate data sources—visualizing real-time ECS metrics alongside CloudWatch Logs—to facilitate rapid troubleshooting.

\* \*\*Security Implementation:\*\* I implemented least-privilege IAM roles for all components, ensuring the monitoring stack uses instance profiles to scrape metrics securely without relying on risky static access keys.



---



\### 3. Technologies Used



\* \*\*Infrastructure as Code:\*\* Terraform

\* \*\*Cloud Platform:\*\* Amazon Web Services (AWS)

\* \*\*Compute:\*\* Amazon ECS (Fargate), EC2

\* \*\*Monitoring \& Metrics:\*\* Prometheus, YACE (CloudWatch Exporter)

\* \*\*Visualization:\*\* Grafana

\* \*\*Logging:\*\* Amazon CloudWatch Logs

\* \*\*Containerization:\*\* Docker, Amazon ECR



---



\### 4. Project Links



\* \*\*<a href="https://github.com/githubabhay2003/serverless-container-observability.git" target="\_blank" rel="noopener noreferrer">View Code \& Project Details on GitHub</a>\*\*



---

