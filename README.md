## 🏷️ Project

Secure and Highly Available AWS VPC Architecture with Auto Scaling and Load Balancing

## Description

This project demonstrates how to design and implement a secure, resilient AWS Virtual Private Cloud (VPC) suitable for a production environment. The architecture is built to ensure high availability, fault tolerance, and security by leveraging multiple AWS networking and compute services.

A custom VPC is created with public and private subnets distributed across two Availability Zones. Application servers are deployed in private subnets using an Auto Scaling Group to automatically adjust capacity based on demand. An Application Load Balancer is used to distribute incoming traffic across instances in multiple Availability Zones.

For security, the servers are not directly exposed to the internet. Outbound internet access from private instances is enabled using NAT Gateways deployed in each Availability Zone, ensuring both security and resiliency. This setup follows AWS best practices for production-grade cloud infrastructure.

The project showcases real-world concepts such as network isolation, high availability, load balancing, and secure internet access forprivate resources.


