---

layout: default

title: "EKS Observability Platform with Prometheus, Grafana, and FastAPI"

category: "Personal"

order: 93

tech-stack: "Terraform, AWS EKS, Helm, Prometheus, Grafana"

github-link: "https://github.com/githubabhay2003/eks-observability-fastapi.git"

summary: "A fully automated, rebuild-safe Kubernetes observability platform on AWS EKS using Terraform and Helm, featuring a FastAPI application instrumented with Prometheus metrics."

---



\# EKS Observability Platform with Prometheus, Grafana, and FastAPI



This project demonstrates a production-style, fully reproducible Kubernetes observability platform on AWS EKS. Built using Terraform and Helm as the single sources of truth, it provisions a secure EKS cluster, deploys an instrumented FastAPI application, and installs a complete monitoring stack without manual intervention.



\[Back to Home](/)



---



\### 1. The Goal



In complex Kubernetes environments, setting up observability often involves fragile, manual steps that are hard to replicate. The goal of this project was to achieve \*\*end-to-end automation\*\* and \*\*rebuild-safety\*\*. The objective was to create a platform where running `terraform destroy` followed by `terraform apply` would restore the entire environment—infrastructure, application, and monitoring dashboards—to a fully functional state with zero manual configuration.







---



\### 2. My Role \& Contributions



I designed and engineered this platform to demonstrate the intersection of Infrastructure as Code and Site Reliability Engineering (SRE) practices.



\* \*\*Infrastructure Provisioning:\*\* I architected a custom AWS VPC and deployed an EKS cluster with managed node groups and a secure Bastion host using Terraform.

\* \*\*Kubernetes Automation:\*\* I managed Kubernetes resources declaratively, utilizing the Helm provider for Terraform to deploy the `kube-prometheus-stack` and the application components.

\* \*\*Application Instrumentation:\*\* I developed a Python FastAPI application and instrumented it with the Prometheus client library to expose custom metrics (Golden Signals like latency and error rates).

\* \*\*Observability Stack:\*\* I configured the Prometheus Operator to automatically discover targets via `ServiceMonitor` CRDs and provisioned Grafana dashboards as code using JSON definitions.

\* \*\*Reliability Engineering:\*\* I implemented and validated custom Prometheus Alert Rules to detect high latency and pod failures, ensuring the alerting pipeline (from Prometheus to Alertmanager) was functional.



---



\### 3. Technologies Used



\* \*\*Infrastructure as Code:\*\* Terraform

\* \*\*Cloud Provider:\*\* AWS (EKS, VPC, EC2, ECR)

\* \*\*Package Management:\*\* Helm

\* \*\*Observability:\*\* Prometheus, Grafana, Alertmanager

\* \*\*Application:\*\* Python (FastAPI), Docker

\* \*\*Orchestration:\*\* Kubernetes



---



\### 4. Project Links



\* \*\*<a href="https://github.com/githubabhay2003/eks-observability-fastapi.git" target="\_blank" rel="noopener noreferrer">View Code \& Project Details on GitHub</a>\*\*



---

