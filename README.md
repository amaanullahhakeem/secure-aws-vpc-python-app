# Secure Python Application Deployment on AWS with Auto Scaling and Load Balancing


## 📌 Project Overview

This project demonstrates the design and implementation of a secure, highly available cloud infrastructure on AWS for deploying a Python-based application. The architecture follows production-level best practices, including network isolation, auto scaling, load balancing, and controlled access to private resources.

A custom AWS VPC was created with public and private subnets across multiple Availability Zones to ensure high availability. The Python application runs on EC2 instances in private subnets, while an Application Load Balancer distributes incoming traffic. A Bastion Host and NAT Gateway are used to securely manage access and outbound connectivity for private instances.

---

## 🛠️ Tech Stack

- **Cloud Provider:** AWS  
- **Compute:** EC2, Auto Scaling Group  
- **Networking:** VPC, Public & Private Subnets  
- **Security:** Security Groups, Bastion Host, NAT Gateway  
- **Load Balancing:** Application Load Balancer (ALB)  
- **Application:** Python 3  
- **Automation:** Bash

---

## 🏗️ Architecture Highlights

- Custom VPC with isolated public and private subnets
- One Auto Scaling Group per Availability Zone for high availability
- Python application deployed on private EC2 instances
- Application Load Balancer for traffic distribution
- Bastion Host used for secure SSH access to private servers
- NAT Gateway enables outbound internet access while masking private IPs
- Security Groups configured with least-privilege access

---

## 🔒 Security Implementation

- Private EC2 instances are not exposed to the internet
- SSH access restricted via Bastion Host only
- NAT Gateway used to prevent direct public exposure of private instances
- Inbound traffic allowed only through the Load Balancer
- Outbound access tightly controlled using routing and security rules

---

## 🚀 Outcome

- Achieved a secure, scalable, and highly available Python application setup
- Ensured fault tolerance using multi-AZ Auto Scaling
- Implemented enterprise-grade networking and security practices
- Created a production-like AWS infrastructure suitable for real-world deployments

---

## Summary

Deployed a Python application in private subnets using Auto Scaling across multiple Availability Zones, secured access via a Bastion Host, and distributed traffic using an Application Load Balancer with NAT-based outbound access.
