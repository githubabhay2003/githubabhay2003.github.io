---

layout: default

title: "Fully Automated AWS WordPress Monitoring Stack"

category: "Personal"

order: 96

tech-stack: "Terraform, AWS, Prometheus, Grafana"

github-link: "https://github.com/githubabhay2003/wordpress-rds-monitoring"

summary: "A complete Infrastructure as Code solution that deploys a secure WordPress application along with a fully integrated monitoring stack (Prometheus \& Grafana) on AWS."

---



\# Fully Automated AWS WordPress Monitoring Stack



This project automates the deployment of a secure, production-ready WordPress application with a fully integrated monitoring stack on AWS. Using Terraform, it provisions not just the application infrastructure (EC2, RDS), but also a dedicated observability layer powered by Prometheus and Grafana.



\[Back to Home](/)



---



\### 1. The Goal



Deploying a web application is only half the battle; ensuring it remains healthy and performant is equally critical. Often, monitoring is treated as an afterthought, requiring manual installation of agents and dashboards after infrastructure is provisioned. The goal of this project was to shift observability "left," making it a fundamental part of the infrastructure code. The objective was to deliver a "zero-touch" deployment where a fully instrumented application and a pre-configured monitoring dashboard are ready the moment the provisioning completes.



---



\### 2. My Role \& Contributions



I architected this solution to seamlessly integrate application hosting with infrastructure monitoring.



\* \*\*Full-Stack IaC:\*\* I wrote modular Terraform code to provision the entire stack: VPC networking, private RDS database, WordPress EC2 instances, and the monitoring server.

\* \*\*Automated Observability:\*\* I configured the EC2 instances to automatically install and run Node Exporter upon boot using User Data scripts.

\* \*\*Prometheus \& Grafana Integration:\*\* I engineered a dedicated monitoring instance that automatically discovers targets and pre-loads Grafana with dashboards for CPU, memory, and database metrics.

\* \*\*Security Architecture:\*\* I designed the network to ensure the database remains private, while allowing the monitoring server to securely scrape metrics from the application tier within the VPC.

\* \*\*Database Reliability:\*\* I provisioned an Amazon RDS (MySQL) instance in a private subnet to ensure data persistence and security, decoupled from the web layer.



---



\### 3. Technologies Used



\* \*\*Infrastructure as Code:\*\* Terraform

\* \*\*Cloud Provider:\*\* AWS (EC2, RDS, VPC, ALB)

\* \*\*Monitoring \& Alerting:\*\* Prometheus, Node Exporter

\* \*\*Visualization:\*\* Grafana

\* \*\*Application:\*\* WordPress (Apache/PHP)



---



\### 4. Project Links



\* \*\*<a href="https://github.com/githubabhay2003/wordpress-rds-monitoring" target="\_blank" rel="noopener noreferrer">View Code \& Project Details on GitHub</a>\*\*



---

