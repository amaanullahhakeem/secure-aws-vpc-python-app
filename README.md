# k8s-project
Project Overview This project demonstrates the end-to-end containerization and orchestration of a Node.js web application. It follows DevOps best practices by using Docker for containerization and Kubernetes (K8s) for automated deployment, scaling, and management.

Scalable Web App Deployment on Kubernetes
🚀 Project Overview
This project demonstrates a production-ready workflow for containerizing a Node.js application and orchestrating it using Kubernetes. It focuses on high availability, externalized configuration, and automated scaling—core principles required for a DevOps Intern role.

🛠 Tech Stack
Runtime: Node.js (Express framework)

Containerization: Docker (Multi-stage/Alpine builds)

Orchestration: Kubernetes (K8s)

Cloud Platform: AWS (EC2 & Security Groups)

Infrastructure as Code: YAML Manifests

🏗 Key Components
Deployment: Manages 3 replicas of the application to ensure the app stays online even if a server (Node) fails.

Service: A LoadBalancer that acts as a single gateway, directing traffic from Port 80 to the internal containers.

ConfigMap: Separates environment variables (like Database URLs or App Colors) from the application code for better security and flexibility.

Docker Optimization: Uses the node:18-alpine image to reduce the attack surface and speed up deployment times.

🚦 Getting Started
1. Build the Image
Bash
docker build -t your-username/node-k8s-app:1.0 .
2. Deploy to Kubernetes
Apply the configuration and the deployment manifests:

Bash
kubectl apply -f configmap.yaml
kubectl apply -f app-deploy.yaml
3. Verify the Cluster State
Bash
kubectl get all
