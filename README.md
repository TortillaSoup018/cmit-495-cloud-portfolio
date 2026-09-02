# Cloud Infrastructure & Storage Architecture Portfolio
**Author:** Gael Garcia  
**Course:** CMIT 495 Capstone  
**Focus:** AWS Cloud Engineering, Hybrid OS Provisioning, Storage Management, and VPC Network Design  

---

## Project Overview
This repository contains hands-on infrastructure labs and architectural designs developed as part of my cybersecurity and cloud studies. The projects demonstrate core competencies in deploying virtual environments across mixed operating systems, configuring enterprise-grade cloud storage solutions, and designing secure, segmented virtual private clouds using AWS.

---

## Lab 1: Multi-OS Cloud Provisioning & Network Access
* **Objective:** Deploy and configure heterogeneous virtual instances on Amazon EC2 to simulate a hybrid enterprise cloud environment.
* **Key Implementation Details:**
  * Provisioned **Windows Server 2025** and **Ubuntu Linux** instances on AWS EC2.
  * Established secure remote administrative access via **RDP (Port 3389)** for Windows and **SSH (Port 22)** using cryptographic key-pair authentication for Linux.
  * Configured security groups and firewall rules to restrict inbound administrative traffic to authorized administrative IP blocks.

---

## Lab 2: Cloud Storage Management & NFS/S3 Integration
* **Objective:** Implement scalable cloud storage solutions and validate block-level performance across virtual hosts.
* **Key Implementation Details:**
  * Provisioned **Amazon Elastic File System (EFS)** shares and successfully mounted them across Linux virtual instances via **NFSv4**.
  * Configured **Amazon S3** object storage buckets for secure artifact collection and centralized file management.
  * Utilized block storage testing utilities (`dd`) to validate write speeds, volume persistence, and data integrity across mounted shares.

---

## Lab 3: VPC Design & Network Subnetting
* **Objective:** Design a custom, segmented network topology within AWS utilizing standard IP addressing principles.
* **Key Implementation Details:**
  * Engineered a custom **Virtual Private Cloud (VPC)** utilizing standard CIDR notation blocks (`/16` and `/20` prefixes).
  * Subdivided the network into isolated public and private subnets to enforce least-privilege network segmentation.
  * Configured Route Tables and Internet Gateways to manage traffic flow securely between internal resources and external networks.

---

## Technical Skills Demonstrated
* **Cloud Platforms:** Amazon Web Services (EC2, S3, EFS, VPC, IAM)
* **Operating Systems:** Ubuntu Linux (CLI, package management via `apt`), Windows Server (RDP, PowerShell administration)
* **Networking Protocols & Security:** TCP/IP, CIDR Subnetting, Security Groups, NFSv4, SSH, Access Control
