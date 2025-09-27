---
layout: default
title: "Java CI/CD Pipeline with Jenkins & Maven"
category: "Personal"
order: 30
tech-stack: "Jenkins, Docker, Maven, Java, AWS"
github-link: "https://github.com/githubabhay2003/jenkins-java-pipeline"
summary: "A complete CI/CD pipeline tailored for Java applications using Jenkins for automation, Maven for building, and Docker for containerization."
---

# Project: Java CI/CD Pipeline with Jenkins, Docker, and Maven

This project demonstrates a complete, automated CI/CD pipeline for a Java Spring MVC web application. The pipeline is designed to automatically build, containerize, and deploy the application upon any code change, ensuring a fast and reliable software delivery process for Java-based projects.

[Back to Home](./index.md)

---

### 1. The Goal

The primary goal of this project was to establish a robust and automated CI/CD workflow specifically tailored for a Java application. The key objective was to use industry-standard tools like Jenkins, Maven, and Docker to create a seamless process that takes the application from source code in a Git repository to a running container in a development environment without any manual intervention.

---

### 2. My Role & Contributions

As the sole DevOps engineer for this project, I was responsible for designing, building, and documenting the entire CI/CD pipeline from scratch.

* **Pipeline Architecture:** I designed the end-to-end workflow, mapping out the stages required to build and deploy a Java Spring application reliably.
* **Declarative Pipeline Creation:** I wrote the `Jenkinsfile` using declarative syntax to define the entire CI/CD process as code. This includes stages for checking out source code, building the application, creating a Docker image, and deploying the final container.
* **Build Automation:** I integrated Apache Maven into the Jenkins pipeline to handle the compilation of the Java code, manage dependencies, and package the application into a deployable `.war` file.
* **Containerization:** I authored the `Dockerfile` to containerize the compiled Java web application, ensuring a consistent and portable runtime environment across different systems.
* **Jenkins Environment Configuration:** I set up the Jenkins server with all the necessary plugins (Maven Integration, Docker Pipeline), configured tools, and managed security by storing Docker Hub credentials securely.

---

### 3. Technologies Used

* **CI/CD:** Jenkins
* **Build Tool:** Apache Maven
* **Containerization:** Docker & Docker Hub
* **Language & Framework:** Java, Spring MVC
* **Source Control:** Git & GitHub
* **Cloud Provider:** AWS

---

### 4. Project Links

* **<a href="https://github.com/githubabhay2003/jenkins-java-pipeline" target="_blank" rel="noopener noreferrer">View Code & Jenkinsfile on GitHub</a>**

---