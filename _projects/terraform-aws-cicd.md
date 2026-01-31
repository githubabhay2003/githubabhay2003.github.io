---

layout: default

title: "Secure \& Cost-Aware AWS CI/CD Pipeline"

category: "Personal"

order: 97

tech-stack: "Terraform, AWS, GitHub Actions, Checkov, Infracost"

github-link: "https://github.com/githubabhay2003/terraform-aws-cicd"

summary: "A professional-grade CI/CD pipeline for AWS infrastructure that integrates security scanning, cost estimation, and manual approval gates."

---



\# Secure \& Cost-Aware AWS CI/CD Pipeline with Terraform



This project demonstrates a fully automated, professional-grade CI/CD pipeline for provisioning and managing AWS infrastructure. It moves beyond simple automation by embedding "shift-left" security principles, financial governance, and strict deployment controls directly into the GitOps workflow.



```mermaid

graph TD

&nbsp;   A\[Dev creates Pull Request] --> B\[GitHub Action: terraform-plan.yml]

&nbsp;   B --> C\[Security Scan Checkov]

&nbsp;   B --> D\[Cost Estimation Infracost]

&nbsp;   B --> E\[Terraform Plan]



&nbsp;   subgraph CI\_Workflow\[CI Workflow on Pull Request]

&nbsp;       C --> F\[Posts SARIF results]

&nbsp;       D --> F

&nbsp;       E --> F\[PR Comments for Review]

&nbsp;   end



&nbsp;   F --> G\[Team Reviews \& Approves PR]

&nbsp;   G --> H\[Merge to main]



&nbsp;   H --> I\[GitHub Action: terraform-apply.yml]



&nbsp;   subgraph CD\_Workflow\[CD Workflow on Merge to main]

&nbsp;       I --> J\[Wait for Manual Approval]

&nbsp;       J --> K\[Terraform Apply]

&nbsp;       K --> L\[AWS Infrastructure Deployed]

&nbsp;   end



&nbsp;   %% Colors

&nbsp;   style A fill:#f2f2f2,stroke:#555,stroke-width:1px,color:#000

&nbsp;   style B fill:#fdd835,stroke:#f57f17,stroke-width:2px,color:#000

&nbsp;   style C fill:#ef5350,stroke:#c62828,color:#fff

&nbsp;   style D fill:#42a5f5,stroke:#1565c0,color:#fff

&nbsp;   style E fill:#66bb6a,stroke:#2e7d32,color:#fff

&nbsp;   style F fill:#d1c4e9,stroke:#512da8,color:#000

&nbsp;   style G fill:#ffb74d,stroke:#ef6c00,color:#000

&nbsp;   style H fill:#a1887f,stroke:#5d4037,color:#fff

&nbsp;   style I fill:#fdd835,stroke:#f57f17,color:#000

&nbsp;   style J fill:#90caf9,stroke:#1976d2,color:#000

&nbsp;   style K fill:#81c784,stroke:#388e3c,color:#000

&nbsp;   style L fill:#26a69a,stroke:#004d40,color:#fff

&nbsp;   style CI\_Workflow fill:#ede7f6,stroke:#7e57c2,stroke-width:1px,color:#000

&nbsp;   style CD\_Workflow fill:#e0f2f1,stroke:#26a69a,stroke-width:1px,color:#000

```



\[Back to Home](/)



---



\### 1. The Goal



In traditional infrastructure workflows, deploying changes is often risky and opaque. Engineers typically have limited visibility into whether a change will introduce security vulnerabilities or significantly impact cloud costs until after it has already been applied. This lack of early feedback increases the risk of misconfigurations, unexpected expenses, and production incidents.



The goal of this project was to eliminate that uncertainty by building a GitOps-driven CI/CD pipeline for infrastructure changes. The objective was to ensure that every Terraform change is automatically security-scanned, cost-estimated, and explicitly approved by a human before it ever reaches the production environment.



---



\### 2. My Role \& Contributions



As the sole engineer on this project, I designed and implemented the entire GitOps workflow end to end, integrating multiple tools into a single, reliable pipeline.



\* \*\*Pipeline Architecture:\*\* I designed a split-workflow CI/CD model using GitHub Actions, with a Continuous Integration workflow for Pull Requests (planning, validation, and analysis) and a Continuous Deployment workflow for merges to the `main` branch.

\* \*\*Security Integration (DevSecOps):\*\* I integrated Checkov to perform static security analysis on Terraform code, configured to fail the pipeline on insecure configurations and upload SARIF results directly to the GitHub Security tab.

\* \*\*Financial Governance (FinOps):\*\* I implemented Infracost to automatically calculate and comment on the estimated monthly cost delta for every Pull Request, providing immediate cost visibility before approval.

\* \*\*Secure Authentication:\*\* I configured OpenID Connect (OIDC) between GitHub Actions and AWS, removing the need for long-lived static credentials such as `AWS\_ACCESS\_KEY\_ID`.

\* \*\*Governance \& Safety Controls:\*\* I implemented GitHub Environments with required reviewers to enforce manual approval gates, ensuring that no infrastructure changes are applied to production without explicit authorization.



---



\### 3. Technologies Used



\* \*\*Automation Platform:\*\* GitHub Actions (CI/CD)

\* \*\*Infrastructure as Code:\*\* Terraform

\* \*\*Cloud Provider:\*\* Amazon Web Services (AWS)

\* \*\*Identity \& Access:\*\* IAM, OpenID Connect (OIDC)

\* \*\*State Management:\*\* Amazon S3, DynamoDB

\* \*\*Security Scanning:\*\* Checkov (Terraform SAST)

\* \*\*Cost Estimation:\*\* Infracost

\* \*\*Version Control:\*\* Git \& GitHub



---



\### 4. Project Links



\* \*\*<a href="https://github.com/githubabhay2003/terraform-aws-cicd" target="\_blank" rel="noopener noreferrer">View Code \& Project Details on GitHub</a>\*\*



---



