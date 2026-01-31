---

layout: default

title: "AWS CI/CD Infrastructure Observability Project"

category: "Personal"

order: 95

tech-stack: "Terraform, Ansible, Jenkins, Prometheus, Grafana"

github-link: "https://github.com/githubabhay2003/aws-ci-cd-infra-observability.git"

summary: "Automated end-to-end DevOps pipeline provisioned with Terraform and Ansible, running Jenkins CI/CD with full observability through Prometheus, Grafana, and Alertmanager."

---



\# AWS CI/CD Infrastructure Observability Project



This project showcases a fully automated DevOps environment capable of provisioning cloud infrastructure, configuring CI/CD tooling, deploying applications, and monitoring both application and pipeline health. It achieves "zero-touch" automation: destroying and recreating the entire stack works without any manual reconfiguration.



\[Back to Home](/)



---



\### 1. The Goal



In many DevOps setups, the "management" layer (Jenkins servers, monitoring dashboards) is often manually configured and fragile. If the server dies, restoring it is a manual, time-consuming process. The goal of this project was to prove automation maturity by treating the \*entire\* DevOps stack as code. The objective was to ensure that a single command could provision the infrastructure, install Jenkins, configure pipelines, and set up monitoring dashboards without a human ever logging into a console.



---



\### 2. My Role \& Contributions



I engineered the complete automation lifecycle, focusing on "gluing" disparate tools into a seamless workflow.



\* \*\*Infrastructure as Code:\*\* I utilized Terraform with a remote backend to provision secure AWS EC2 infrastructure, ensuring state locking and consistency.

\* \*\*Configuration Management:\*\* I wrote extensive Ansible roles to install and configure Jenkins, Docker, Prometheus, and Grafana. Crucially, I automated the \*logic\* (e.g., adding the Jenkins user to the Docker group) to prevent runtime permission errors.

\* \*\*Dynamic Inventory Automation:\*\* I solved the challenge of changing IP addresses by writing a `bootstrap-dev.sh` script that dynamically fetches Terraform outputs and updates the Ansible inventory, enabling seamless destroy/rebuild cycles.

\* \*\*Observability as Code:\*\* Instead of manually creating dashboards, I implemented Grafana provisioning via Ansible. This ensured that dashboards and datasources were persistent and version-controlled, reappearing automatically after every deployment.

\* \*\*End-to-End Validation:\*\* I implemented a "Destroy \& Rebuild" validation strategy to verify that the system was truly resilient and required no manual "hot-fixes" to recover.



---



\### 3. Technologies Used



\* \*\*Infrastructure:\*\* AWS, Terraform (Remote Backend)

\* \*\*Configuration:\*\* Ansible (Roles \& Playbooks)

\* \*\*CI/CD:\*\* Jenkins (Scripted Pipeline), Docker

\* \*\*Observability:\*\* Prometheus (Metrics), Grafana (Visualization), Alertmanager

\* \*\*Scripting:\*\* Bash, Python



---



\### 4. Project Links



\* \*\*<a href="https://github.com/githubabhay2003/aws-ci-cd-infra-observability.git" target="\_blank" rel="noopener noreferrer">View Code \& Project Details on GitHub</a>\*\*



---

