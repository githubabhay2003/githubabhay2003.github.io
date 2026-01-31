---

layout: default

title: "End-to-End Multi-Tier WordPress Deployment on AWS"

category: "Personal"

order: 98

tech-stack: "Terraform, AWS (EC2, RDS, VPC), Shell Scripting"

github-link: "https://github.com/githubabhay2003/aws-wordpress-terraform-project.git"

summary: "A production-grade Infrastructure as Code solution that automates the deployment of a secure, three-tier WordPress architecture on AWS using Terraform."

---



\# End-to-End Multi-Tier WordPress Deployment on AWS with Terraform



This project demonstrates a fully automated, production-grade Infrastructure as Code (IaC) solution for deploying a secure and scalable WordPress application. It replaces manual configuration with a robust Terraform codebase that provisions a complete three-tier architecture on AWS in minutes.



\[Back to Home](/)



---



\### 1. The Goal



Manually deploying and configuring multi-tier web applications is often a slow, error-prone process that is difficult to replicate consistently. The goal of this project was to solve these challenges by creating a "one-click" deployment pipeline. The objective was to ensure that the entire stack—from the network layer to the application installation—could be provisioned, updated, or destroyed programmatically, ensuring reliability and drastically reducing deployment time.



---



\### 2. My Role \& Contributions



I was responsible for the end-to-end architecture and implementation of this IaC solution.



\* \*\*Network Architecture:\*\* I designed a custom VPC with a strict segmentation strategy, placing web servers in public subnets and the database in private subnets to prevent direct internet access to sensitive data.

\* \*\*Modular Terraform Development:\*\* I structured the codebase into reusable modules (`compute`, `database`, `network`) to ensure maintainability and scalability, rather than using a monolithic configuration file.

\* \*\*Automated Provisioning:\*\* I wrote the `user\_data` shell scripts to automatically install Apache, PHP, and WordPress upon instance boot, removing the need for manual SSH configuration.

\* \*\*Database Management:\*\* I implemented a Multi-AZ Amazon RDS (MySQL) instance to ensure high availability and offloaded database management tasks.

\* \*\*Security Engineering:\*\* I utilized AWS Security Groups as stateful firewalls, strictly allowing only HTTP/SSH traffic to the web tier and restricting database access solely to the web server instances.



---



\### 3. Technologies Used



\* \*\*Infrastructure as Code:\*\* Terraform

\* \*\*Cloud Provider:\*\* Amazon Web Services (AWS)

\* \*\*Compute \& Config:\*\* EC2, Shell Scripting (Bash)

\* \*\*Database:\*\* Amazon RDS (MySQL)

\* \*\*Networking:\*\* VPC, Subnets, Internet \& NAT Gateways

\* \*\*Security:\*\* Security Groups, IAM



---



\### 4. Project Links



\* \*\*<a href="https://github.com/githubabhay2003/aws-wordpress-terraform-project.git" target="\_blank" rel="noopener noreferrer">View Code \& Project Details on GitHub</a>\*\*



---

