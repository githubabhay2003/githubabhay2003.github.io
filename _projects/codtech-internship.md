---
layout: default
title: "DevOps Internship Projects (CodTech)"
category: "Internship"
tech-stack: "Kubernetes, Docker, GitHub Actions, DevSecOps, Git"
github-link: "https://github.com/githubabhay2003/codtech-task4-devsecops"
---

# Project: DevOps Internship Projects at CodTech IT Solutions

This project is a comprehensive portfolio of the tasks completed during my DevOps internship at CodTech IT Solutions. It showcases a progression of skills, starting from foundational version control with Git, moving to CI/CD automation with Jenkins, container orchestration with Kubernetes, and finally integrating security into the pipeline with DevSecOps practices.

[Back to Home](../index.md)

---

### 1. The Goal

The primary goal of this internship was to build and demonstrate a complete, modern DevOps workflow. Each task was a building block, designed to solve a specific problem in the software development lifecycle, culminating in a secure, automated, and orchestrated deployment pipeline.

---

### 2. My Role & Contributions

As the intern responsible for these tasks, I independently handled the implementation, troubleshooting, and documentation for each module.

#### Task 4: DevSecOps - Integrating Security into CI/CD
* Integrated the OWASP ZAP security scanner directly into a GitHub Actions workflow to "shift security left" and automate vulnerability checks.
* Demonstrated adaptability and problem-solving by pivoting from a problematic SonarCloud integration to a successful implementation with OWASP ZAP.
* Configured the ZAP baseline scan action to target local files within the GitHub runner, ensuring the pipeline was self-contained and efficient.

#### Task 3: Kubernetes - Container Orchestration
* Containerized a two-tier microservices application (Nginx frontend, Node.js backend) using Dockerfiles.
* Utilized Docker Hub as a central container registry to store and serve images to the Kubernetes cluster, a standard industry practice.
* Defined the entire application stack as code using Kubernetes manifest files for `Deployments` and `Services`.
* Overcame local Minikube networking issues by migrating the deployment to a cloud-based Killercoda environment, demonstrating flexibility in tool selection.

#### Task 2: CI/CD - Automation Pipeline
* Built a complete, automated CI/CD pipeline using GitHub Actions to deploy a static website to GitHub Pages.
* Wrote the workflow file from scratch, configuring it to trigger automatically on every push to the `main` branch.
* Implemented the standard GitHub Actions workflow for Pages deployment, including checking out code, configuring pages, uploading the site as an artifact, and deploying it.

#### Task 1: Git - Foundation of Version Control
* Demonstrated a practical understanding of core Git principles, including creating and working with feature branches.
* Intentionally created and successfully resolved a merge conflict, documenting the process of identifying conflict markers, editing the file to a correct state, and finalizing the merge commit.

---

### 3. Technologies Used

* **DevSecOps & Security:** OWASP ZAP
* **Containerization & Orchestration:** Docker, Kubernetes, Minikube, Killercoda
* **CI/CD & Automation:** GitHub Actions
* **Hosting & Registry:** GitHub Pages, Docker Hub
* **Version Control:** Git, GitHub

---

### 4. Project Links

* **<a href="https://github.com/githubabhay2003/codtech-task4-devsecops" target="_blank" rel="noopener noreferrer">View DevSecOps Project on GitHub</a>**
* **<a href="https://github.com/githubabhay2003/codtech-task3-kubernetes" target="_blank" rel="noopener noreferrer">View Kubernetes Project on GitHub</a>**
* **<a href="https://github.com/githubabhay2003/codtech-task2-cicd" target="_blank" rel="noopener noreferrer">View CI/CD Project on GitHub</a>**
* **<a href="https://github.com/githubabhay2003/codtech-task1-git" target="_blank" rel="noopener noreferrer">View Git Project on GitHub</a>**

---