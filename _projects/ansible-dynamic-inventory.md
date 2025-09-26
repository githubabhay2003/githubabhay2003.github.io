---
layout: default
title: "Automated HAProxy with Ansible Dynamic Inventory"
category: "Personal"
tech-stack: "AWS, Ansible, HAProxy, Jinja2"
github-link: "https://github.com/githubabhay2003/ansible-dynamic-inventory-project"
---

# Project: Automated HAProxy Configuration with Ansible Dynamic Inventory on AWS

This project demonstrates a fully automated, cloud-native solution for managing a high-availability web service architecture. It features an HAProxy load balancer that dynamically discovers and- configures its backend server pool using Ansible's dynamic inventory capabilities for AWS. The system is designed to automatically adapt to changes in the infrastructure—such as the addition or removal of web servers—without any manual intervention, ensuring continuous service availability and scalability.

[Back to Home](../index.md)

---

### 1. The Goal

In dynamic cloud environments, manually updating a load balancer's configuration every time a web server is launched or terminated is inefficient, slow, and highly prone to human error. This can lead to service downtime, as traffic might be sent to non-existent servers or new servers might not receive any traffic at all. The goal of this project was to automate that entire process, creating a self-managing and resilient system.

---

### 2. My Role & Contributions

As the sole engineer for this project, I was responsible for the entire lifecycle, from design and implementation to troubleshooting and documentation.

* **System Architecture:** I designed the tag-based discovery workflow and the overall cloud architecture within a custom AWS VPC.
* **Automation Development:** I authored the core Ansible playbooks, including using the `aws_ec2` dynamic inventory plugin to query the AWS API in real-time.
* **Configuration Templating:** I created the Jinja2 templates for both the HAProxy configuration (`haproxy.cfg.j2`) and the web server content (`index.html.j2`), allowing for dynamic and consistent deployments.
* **Idempotent Playbook Design:** I engineered the playbooks to be idempotent and utilized Ansible handlers to ensure HAProxy was gracefully reloaded only when necessary, preventing unnecessary downtime.
* **Troubleshooting and Problem Solving:** I diagnosed and resolved several real-world issues, including Ansible SSH authentication failures, race conditions with EC2 user data scripts, and load balancer caching problems, implementing robust solutions for each.

---

### 3. Technologies Used

* **Cloud Platform:** Amazon Web Services (AWS)
* **Automation Engine:** Ansible
* **Load Balancer:** HAProxy
* **Templating Engine:** Jinja2
* **Infrastructure:** AWS EC2, VPC, Subnets, Security Groups, IAM Roles
* **Operating System:** Ubuntu 24.04 LTS

---

### 4. Project Links

* **<a href="https://github.com/githubabhay2003/ansible-dynamic-inventory-project" target="_blank" rel="noopener noreferrer">View Code & Project Details on GitHub</a>**

---