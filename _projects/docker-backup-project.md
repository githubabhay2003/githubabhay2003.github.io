---
layout: default
title: "Docker Volume Backup System"
category: "Personal"
order: 180
tech-stack: "Python, Docker, Docker Compose, Shell Scripting"
github-link: "https://github.com/githubabhay2003/Docker-volume-backup-system"
summary: "A containerized, automated tool that uses a Python scheduler to create, compress, and manage backups for Docker volumes with a configurable retention policy."
---

# Project: Docker Volume Backup System

This project is a self-contained, automated solution for backing up persistent data from Docker volumes, packaged as an easy-to-use Docker container.

[Back to Home](../index.md)

---

### 1. The Goal
The goal of this project was to provide an automated solution for backing up Docker volumes. The system uses a Python-based scheduler running inside its own Docker container to periodically create compressed `.tar.gz` backups of all Docker volumes, storing them in a specified directory with a configurable retention policy.

---

### 2. My Role & Contributions
As the developer, I architected this tool to be a standalone, "set-it-and-forget-it" utility for DevOps workflows.

* **Containerization:** I wrote the `Dockerfile` and `docker-compose.yml` files to package the entire Python application, its dependencies, and its configuration into a portable and isolated container.
* **Automation Scripting:** I developed the core `backup_manager.py` script in Python to handle the backup logic, including finding volumes, creating compressed archives using `tar`, and managing the retention policy to prune old backups.
* **Scheduling & Entrypoint:** I used a Python scheduling library and an `entrypoint.sh` shell script to ensure the backup process runs automatically at a user-defined interval after the container starts.
* **Configuration Management:** I implemented a simple `config.json` file to allow users to easily configure source/destination paths, backup intervals, and retention days without modifying the code.

---

### 3. Technologies Used
* **Core Technology:** Docker, Docker Compose
* **Primary Language:** Python
* **Automation:** Shell Scripting, Task Scheduling
* **Data Handling:** `tar` for archiving, JSON for configuration

---

### 4. Project Links
* **<a href="https://github.com/githubabhay2003/Docker-volume-backup-system" target="_blank" rel="noopener noreferrer">View Code on GitHub</a>**

---