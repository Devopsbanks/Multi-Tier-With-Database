# 🏦 Banking Application - Java + MySQL on AKS

This is a **2-tier Banking Web Application** built using **Java (Spring Boot)** and **MySQL**, containerized with Docker and deployed to **Azure Kubernetes Service (AKS)** using an automated CI/CD pipeline in Azure DevOps.

---

## 📌 Features

- 🧩 Java-based frontend using Spring Boot
- 🗃️ MySQL as backend database
- 🐳 Dockerized for container deployment
- 🚀 CI/CD pipeline using Azure DevOps YAML
- 🔐 Trivy security scanning for both filesystem & image
- ☸️ Deployed on Azure Kubernetes Service (AKS)
- 📦 Artifacts pushed to Azure Container Registry (ACR) and Maven feed

---

## 🚧 CI/CD Pipeline Overview

| Stage | Description |
|-------|-------------|
| `maven_compile` | Compiles the Java application |
| `maven_test` | Runs unit tests using Maven |
| `trivy_scan` | Scans source code for vulnerabilities |
| `publish_artifact` | Publishes `.jar` to Maven feed |
| `Docker_buid` | Builds Docker image from Dockerfile |
| `trivy_image_scan` | Scans Docker image for vulnerabilities |
| `Docker_image_publish` | Pushes Docker image to ACR |
| `deploy_to_AKS` | Deploys the app to AKS using `ds.yml` |

---

## 🛠️ Tech Stack

- Java (Spring Boot)
- MySQL
- Docker
- Kubernetes (AKS)
- Azure DevOps YAML Pipelines
- Azure Container Registry (ACR)
- Trivy for vulnerability scanning

---
👤 Author
Hemant Kumar
Azure Cloud & DevOps Engineer | 10.5+ years experience
🔗 GitHub: Devopsbanks
