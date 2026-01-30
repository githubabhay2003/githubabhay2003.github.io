---
layout: default
title: "CI/CD Pipeline for Python on AWS EKS"
category: "Personal"
order: 160
tech-stack: "AWS EKS, CodePipeline, ECR, Python, Docker"
github-link: "https://github.com/githubabhay2003/cicd-app-repo"
summary: "An end-to-end automated pipeline using AWS services, including CodePipeline and a managed Kubernetes cluster (EKS), to deploy a Python application."
---

# Project: End-to-End CI/CD Pipeline for a Python Application on AWS EKS
This project demonstrates a complete, end-to-end CI/CD pipeline that automates the entire lifecycle of a Python (FastAPI) web application. The workflow covers the entire process from a `git push` on GitHub to a live deployment on a managed Kubernetes cluster (AWS EKS).

[Back to Home](../index.md)

---

### 1. The Goal

The goal was to build a complete, end-to-end CI/CD pipeline to fully automate the software delivery lifecycle for a Python (FastAPI) application. The system automatically triggers on a `git push`, builds a containerized version of the application, pushes it to a private registry, and orchestrates its deployment onto a managed Kubernetes cluster (Amazon EKS) on AWS.

### 2. My Role & Contributions

As the architect and developer of this pipeline, I was responsible for designing and integrating the full set of cloud services required for a modern, automated deployment workflow.

* **Architecture Design:** I designed the GitOps-style CI/CD workflow, mapping out the flow from a developer's code commit on GitHub to a live deployment on Amazon EKS.
* **CI/CD Pipeline Implementation:** I configured the core automation engine using **AWS CodePipeline** to monitor the source repository and **AWS CodeBuild** to execute the build, test, and containerization stages defined in the `buildspec.yml` file.
* **Containerization:** I wrote the `Dockerfile` to package the Python FastAPI application, its dependencies, and the runtime environment into a lightweight, portable container image.
* **Kubernetes Deployment:** I created the Kubernetes manifest files (`deployment.yaml` and `service.yaml`) to define how the application should be deployed, scaled, and exposed to the internet via an AWS Load Balancer within the EKS cluster.
* **Cloud Infrastructure Setup:** I was responsible for setting up and configuring the necessary AWS infrastructure, including the **Amazon ECR** private repository for storing Docker images and the **Amazon EKS** cluster to serve as the deployment environment.

### 3. Technologies Used

* **CI/CD & Automation:** AWS CodePipeline, AWS CodeBuild
* **Cloud & Orchestration:** Amazon Web Services (AWS), Amazon EKS (Elastic Kubernetes Service), Amazon ECR (Elastic Container Registry)
* **Application & Containerization:** Python (FastAPI), Docker
* **Source Control:** Git & GitHub

### 4. Project Links

* **<a href="https://github.com/githubabhay2003/cicd-app-repo" target="_blank" rel="noopener noreferrer">View Code & Architecture on GitHub</a>**

---