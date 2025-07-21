# Project: Contact Identification API with CI/CD on AWS

This project features a Node.js REST API that is fully containerized, deployed to a Kubernetes cluster on AWS, and managed by an automated CI/CD pipeline using GitHub Actions.

[Back to Home](./index.md)

---

### 1. The Goal
The goal of this technical challenge was to build and deploy a simple Node.js REST API for identifying and consolidating user contacts. The key requirement was not just the application itself, but demonstrating a complete, end-to-end DevOps workflow for its deployment and management on the cloud.

---

### 2. My Role & Contributions
As the DevOps engineer for this project, I handled the entire infrastructure, containerization, and automation pipeline.

* **Application Containerization:** I wrote a multi-stage `Dockerfile` to create a lightweight, optimized, and secure container image for the Node.js application.
* **Kubernetes Orchestration:** I authored the `k8s_deployment_v1.yaml` manifest to define the Kubernetes Deployment and Service, ensuring the application could be deployed reliably and exposed correctly within an EKS cluster.
* **CI/CD Pipeline Automation:** I built the complete CI/CD pipeline from scratch using GitHub Actions. The workflow automatically triggers on code pushes, builds the Docker image, pushes it to Amazon ECR (Elastic Container Registry), and then securely deploys the new version to the Amazon EKS (Elastic Kubernetes Service) cluster.
* **Cloud Integration:** I configured the necessary connections and permissions between GitHub Actions and AWS, using secure secrets management for AWS credentials.

---

### 3. Technologies Used
* **Application:** Node.js, Express.js
* **Containerization:** Docker
* **Orchestration:** Kubernetes
* **CI/CD:** GitHub Actions
* **Cloud Platform:** AWS (Amazon ECR, Amazon EKS)

---

### 4. Project Links
* [**View Code & CI/CD Workflow on GitHub**](https://github.com/githubabhay2003/Cloud-backend-Assignment)
