---
layout: default
title: "Ansible Dynamic Load Balancer on AWS"
category: "Personal"
tech-stack: "AWS, Ansible, HAProxy, Apache, Jinja2"
github-link: "https://github.com/githubabhay2003/ansible-loadbalancer-project"
summary: "An automated setup that uses Ansible to deploy and configure an HAProxy load balancer and a fleet of backend Apache web servers on AWS.":
---

# Project: Ansible Dynamic Load Balancer on AWS

This project automates the deployment of a high-availability, dynamically scalable web architecture on AWS using Ansible. It provisions an HAProxy load balancer that automatically discovers and distributes traffic to a backend fleet of Apache web servers. The entire setup is dynamic: by simply adding a new web server's private IP to the Ansible inventory and re-running the master playbook, the new server is automatically provisioned, configured, and added to the load balancer's pool.

[Back to Home](../index.md)

---

### 1. The Goal

The goal of this project was to create a hands-off, scalable web infrastructure using Ansible's agentless automation. The key objective was to eliminate the manual steps involved in adding or removing web servers, allowing an operator to scale the backend fleet simply by editing a text-based inventory file. This approach reduces configuration errors and deployment time significantly.

---

### 2. My Role & Contributions

As the author of this project, I designed and implemented the entire automated deployment workflow from the ground up.

* **Ansible Role Development:** I developed modular Ansible roles for both the `webserver` (Apache) and `haproxy` components, which promotes code reuse and makes the automation easier to maintain and understand.
* **Dynamic Configuration:** I created a dynamic HAProxy configuration using a Jinja2 template that automatically reads the list of web servers from the Ansible inventory file and populates the backend server pool.
* **Master Playbook Orchestration:** I authored the master playbook (`site.yml`) to orchestrate the entire deployment, ensuring that web servers are configured first before the load balancer is set up to depend on them.
* **End-to-End Documentation:** I documented the complete setup process, including AWS prerequisites, security group configuration, and common troubleshooting steps for issues like SSH connectivity and service failures.

---

### 3. Technologies Used

* **Cloud Provider:** AWS EC2
* **Automation:** Ansible
* **Load Balancer:** HAProxy
* **Web Server:** Apache (`httpd`)
* **Templating:** Jinja2

---

### 4. Project Links

* **<a href="https://github.com/githubabhay2003/ansible-loadbalancer-project" target="_blank" rel="noopener noreferrer">View Code & Project Details on GitHub</a>**

---
