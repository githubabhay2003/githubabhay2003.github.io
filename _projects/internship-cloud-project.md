---
layout: default
title: "Cloud Technology Intern (Nullclass Edtech Pvt. Ltd.)"
category: "Internship"
order: 1
tech-stack: "AWS, Terraform, Ansible, Jenkins, Docker"
github-link: "https://github.com/githubabhay2003/internship-cloud-project"
summary: "A fully automated CI/CD pipeline built with Jenkins, Terraform, and Ansible to deploy a containerized web application on AWS infrastructure."
---

# Project: Automated Web Application Deployment on AWS (NullClass Internship Project)

The primary objective of this project was to design, build, and deploy a fully automated Continuous Integration and Continuous Deployment (CI/CD) pipeline. The goal was to take a static web application from a source code repository to a live, publicly accessible server on AWS, with the entire process being automated and triggered by a `git push`.

[Back to Home](../index.md)

---

### 1. The Goal

The goal was to implement modern DevOps principles such as Infrastructure as Code, Configuration Management, and Pipeline as Code to create a fully automated CI/CD pipeline. The final system needed to automatically build, test, and deploy a web application to AWS infrastructure in response to code changes, eliminating manual intervention and accelerating the delivery lifecycle.

---

### 2. My Role & Contributions

During my internship at NullClass Edtech, I was responsible for building this entire CI/CD pipeline from scratch, covering all aspects from infrastructure to deployment.

* **Infrastructure as Code (Terraform):** I wrote Terraform scripts to provision all the necessary AWS infrastructure, including the EC2 instance and a security group with the required ingress rules for SSH and HTTP traffic.
* **Configuration Management (Ansible):** I developed an idempotent Ansible playbook to perform the initial server setup, which included installing Docker, its prerequisites, and the Docker Compose plugin.
* **Containerization (Docker):** I containerized the static web application by authoring a `Dockerfile` and managed its service definition with a `docker-compose.yml` file to ensure a consistent runtime environment.
* **Pipeline as Code (Jenkins):** I authored a declarative `Jenkinsfile` that defined the entire multi-stage CI/CD workflow, including checking out code, building the Docker image, pushing it to Docker Hub, and deploying it to the EC2 server.
* **CI/CD Integration:** I integrated the Jenkins pipeline with the GitHub repository using webhooks, enabling the entire process to be triggered automatically on every `git push`.
* **Problem Solving:** I systematically diagnosed and resolved a wide range of real-world integration issues, including SSH key permissions, package dependencies, Terraform state management, and Jenkins user permissions for the Docker socket.

---

### 3. Technologies Used

* **Cloud Provider:** Amazon Web Services (AWS)
* **Infrastructure as Code:** Terraform
* **Configuration Management:** Ansible
* **Containerization:** Docker & Docker Compose
* **CI/CD Automation:** Jenkins
* **Version Control:** Git & GitHub

---

### 4. Project Links

* **<a href="https://github.com/githubabhay2003/internship-cloud-project" target="_blank" rel="noopener noreferrer">View Code & Project Details on GitHub</a>**
* **<a href="https://drive.google.com/file/d/1boezQtv-9o_LGoYgfXfqK7JumYTg2vOi/view?usp=sharing" target="_blank" rel="noopener noreferrer">Watch the End-to-End Demo Video</a>**
---