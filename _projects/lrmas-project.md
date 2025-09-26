---
layout: default
title: "Linux Resource Monitoring & Alert System (LRMAS)"
category: "Personal"
order: 110
tech-stack: "Python, Linux, systemd, psutil"
github-link: "https://github.com/githubabhay2003/linux-resource-monitor"
summary: "A custom Python service that runs as a background systemd daemon to monitor Linux system resources and send real-time email alerts when thresholds are breached."
---

# Project: LRMAS - Linux Resource Monitoring & Alert System

LRMAS is a lightweight, custom-built monitoring tool that runs as a background service on a Linux system to track critical resources and send real-time alerts.

[Back to Home](./index.md)

---

### 1. The Goal
The goal of this project was to create a lightweight, Python-based Linux resource monitoring tool that runs as a background `systemd` service. It actively monitors CPU, memory, and disk usage and automatically sends real-time alerts via email when any of these metrics exceed user-defined thresholds, enabling proactive system administration.

---

### 2. My Role & Contributions
As the sole developer, I engineered this tool from the ground up, focusing on reliability and efficiency.

* **Core Monitoring Logic:** I wrote the Python script using the `psutil` library to accurately fetch real-time CPU, memory, and disk statistics from the Linux kernel.
* **Alerting Mechanism:** I implemented an email alerting system using Python's `smtplib`, allowing the tool to send immediate notifications through an SMTP relay.
* **Systemd Service Integration:** I created a `systemd` service unit file, enabling the script to run persistently as a background daemon, start automatically on boot, and be managed like any other standard Linux service. This demonstrates a key aspect of system administration.
* **Configuration & Logging:** I designed the tool to be easily configurable and to automatically log all warning events to a local file for later review.

---

### 3. Technologies Used
* **Primary Language:** Python
* **Key Libraries:** `psutil`, `smtplib`
* **Core Technology:** Linux System Administration
* **Service Management:** `systemd`
* **Alerting Protocol:** SMTP

---

### 4. Project Links
* **<a href="https://github.com/githubabhay2003/linux-resource-monitor" target="_blank" rel="noopener noreferrer">View Code on GitHub</a>**

---