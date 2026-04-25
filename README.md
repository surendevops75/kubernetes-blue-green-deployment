# 🚀 Kubernetes Blue-Green Deployment

## 📌 Repository Description

Production-ready Kubernetes Blue-Green deployment strategy using YAML manifests for zero-downtime application releases with main service switching, preview environment testing, and controlled traffic routing.

---

## 📌 Project Overview

This repository demonstrates Blue-Green deployment implementation in Kubernetes using native YAML manifests.

It enables safe application releases by deploying a new version (Green), validating it through preview service, and switching production traffic from current version (Blue) to the new version with minimal risk and zero downtime.

---

## 🛠️ Tools & Technologies

- Kubernetes
- YAML
- Deployments
- Services
- Blue-Green Strategy
- kubectl
- DevOps
- CI/CD

---

## 🏗️ Deployment Components

- Main Production Service
- Green Version Deployment
- Preview Testing Service
- Application Deployment Manifests
- Traffic Switching Strategy
- Zero Downtime Release Process

---

## 📂 Repository Structure

```bash
01-main-service.yaml
02-green-deployment.yaml
03-preview-service.yaml
20-deployment.yaml
```
---

### 🚀 Deployment Steps
```bash
kubectl apply -f 20-deployment.yaml
kubectl apply -f 01-main-service.yaml

kubectl apply -f 02-green-deployment.yaml
kubectl apply -f 03-preview-service.yaml

kubectl get pods
kubectl get svc
```
---

### 🔐 Key Features

- Zero Downtime Deployment
- Safe Production Releases
- Easy Rollback Strategy
- Preview Testing Before Go-Live
- Controlled Traffic Switching
- Kubernetes Native YAML Setup
- CI/CD Friendly Deployment Pattern

---

## 📸 Architecture Flow

Users → Main Service (Blue) → Current Pods
QA Team → Preview Service (Green) → New Pods
After Approval → Main Service Switches to Green Pods

---

## 📈 Real-Time Use Cases
- Application version upgrades without downtime
- Production release validation before traffic cutover
- Safer deployments in Kubernetes environments
- Fast rollback during failed releases
- CI/CD controlled release strategy

---

## 👨‍💻 Author

Surendra DevOps Engineer

---

⭐ If you like this project, give it a star