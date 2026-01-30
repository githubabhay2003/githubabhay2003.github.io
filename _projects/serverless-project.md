---
layout: default
title: "AWS Cloud Intern (Navodita InfoTech)"
category: "Internship"
order: 130
tech-stack: "AWS Lambda, S3, Cognito, IAM, Python"
github-link: "https://github.com/githubabhay2003/Serverless-Image-Processing-using-AWS-Services"
summary: "An event-driven, serverless pipeline on AWS using S3, Lambda, and Cognito to automatically process and resize images upon secure upload."
---

# Project: Serverless Image Processing Pipeline on AWS

This project is an end-to-end, event-driven pipeline that automatically resizes images upon upload using a fully serverless architecture on Amazon Web Services.

[Back to Home](../index.md)

---

### 1. The Goal
The goal was to create a robust and efficient serverless image processing service on AWS. The system securely accepts image uploads via a web frontend, automatically triggers an AWS Lambda function to resize the image, and stores the processed image in a separate S3 bucket, providing real-time feedback to the user without any server management.

---

### 2. My Role & Contributions
As the architect and developer of this pipeline, I was responsible for integrating multiple AWS services to create a seamless, automated workflow.

* **Architecture Design:** I designed the serverless, event-driven architecture, where an S3 upload event directly triggers the Lambda function for processing.
* **Backend Development:** I wrote the Python-based AWS Lambda function, using the Pillow library, to perform the core image resizing logic.
* **Cloud Infrastructure Setup:** I configured all the necessary AWS services, including two S3 buckets (for input and output) with appropriate policies and CORS rules, and the S3 event trigger to invoke Lambda.
* **Security & Identity:** I implemented a secure access model using IAM roles for the Lambda function and Amazon Cognito Identity Pools to provide the frontend with temporary, limited-permission credentials for direct S3 uploads, eliminating the need to expose long-lived keys.
* **Frontend Integration:** I developed the simple HTML/JavaScript frontend, integrating the AWS SDK to facilitate the secure upload process and display the results to the user.

---

### 3. Technologies Used
* **Core AWS Services:** Amazon S3, AWS Lambda, IAM, Amazon Cognito
* **Backend:** Python (with Pillow library)
* **Frontend:** HTML, JavaScript, AWS SDK for JavaScript
* **Architecture:** Serverless, Event-Driven

---

### 4. Project Links
* **<a href="https://github.com/githubabhay2003/Serverless-Image-Processing-using-AWS-Services" target="_blank" rel="noopener noreferrer">View Code & Architecture on GitHub</a>**

---
