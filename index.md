---
layout: default
title: MediCare Direct - AWS Infrastructure Design
---

# MediCare Direct: AWS Infrastructure Design Blueprint

**Student Name:** Robert Angel B. Santiago  
**Student ID:** 23-1360-266  
**Course & Section:** BSIT-4-A — SAM10 Systems Administration & Maintenance  
**Instructor:** Romack L. Natividad, MIT  
**Institution:** Angeles University Foundation — College of Computer Studies (AUF CCS)  
**AWS Region:** `ap-southeast-1` (Singapore)  

---

## 📽️ System Architecture Demonstration Video

Below is the walkthrough video demonstrating the 3-Tier VPC Architecture, Network Flow, and IAM Governance for MediCare Direct:

<video controls width="100%" poster="assets/video-thumbnail.png" style="border-radius: 8px; border: 1px solid #30363d;">
  <source src="demo-video.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

---

## 📄 Project Deliverables & Documents

Click below to view or download the official project PDF documentation:

| Deliverable Name | Description | View / Download |
| :--- | :--- | :---: |
| **Deliverable 1: System Proposal** | High-level system requirements, AWS service mapping, and network topology. | [📄 View PDF](SAM10_System_Proposal_Santiago.pdf) |
| **Deliverable 2: AWS Architecture Diagram** | Complete 3-Tier VPC diagram, routing tables, and security group chaining. | [📄 View PDF](SAM10_AWS_Architecture_Diagram_Santiago.pdf) |
| **Deliverable 3: Infrastructure Design Document** | Comprehensive 4-page cloud blueprint, compute specifications, and cost analysis. | [📄 View PDF](SAM10_Infrastructure_Design_Document_Santiago.pdf) |

---

## 🏗️ Architecture Overview & Specifications

MediCare Direct is deployed across a 3-tier isolated Virtual Private Cloud (VPC) in the Singapore region (`10.0.0.0/16`).

### Network & Subnet Topology

* **Public Web Tier (`10.0.1.0/24`):** Hosts NGINX Reverse Proxy (`t3.micro`) connected to the Internet Gateway (`IGW`) via Ports 80 and 443.
* **Private Application Tier (`10.0.2.0/24`):** Hosts Node.js Express REST API (`t3.small`) on Port 5000, strictly accessible only from `sg-WebTier`.
* **Private Data Tier (`10.0.3.0/24`):** Hosts PostgreSQL 15 Database (`t3.small`) on Port 5432 with 100 GB KMS-encrypted `gp3` storage, accessible only from `sg-AppTier`.

---

## 🔒 Security & IAM Governance

* **Least Privilege:** Security Group ID chaining ensures backend instances accept connections strictly from upstream tiers.
* **Closed Administrative Ports:** SSH (Port 22) is completely disabled across all instances. Administrative access is granted exclusively through **AWS Systems Manager (SSM) Session Manager**.
* **Root Lock Down:** Hardware MFA enforced on Root Account; operational duties mapped to RBAC roles (`CloudAdmin`, `SysAdmin`, `ReadOnlyAudit`).

---

## 💰 Monthly AWS Cost Summary

* **Estimated Baseline Cost:** `$57.98 / month` (`$695.76 / year`)
* **Optimization:** 1-Year Compute Savings Plan applied to reduce EC2 runtime costs by up to 34%.
