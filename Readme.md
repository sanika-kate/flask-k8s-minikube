# Flask Application Deployment using Docker & Kubernetes (Minikube)

## 📌 Project Overview
This project demonstrates containerization and deployment of a Python Flask application using Docker and Kubernetes (Minikube).

The application is containerized using Docker and deployed on a local Kubernetes cluster using Minikube.

---

## 🛠 Tech Stack
- Python (Flask)
- Docker
- Kubernetes
- Minikube

---

## 📂 Project Structure

k8s-project/
│
├── app.py
├── Dockerfile
├── templates/
│     └── index.html
├── k8s/
│     ├── deployment.yaml
│     ├── service.yaml
│     ├── pv.yaml
│     ├── pvc.yaml
└── README.md

---

## 🚀 Steps Performed

1. Created a simple Flask application.
2. Created Dockerfile to containerize the application.
3. Built Docker image and pushed the image on dockerhub.
4. Deployed application using Kubernetes Deployment.
5. Exposed application using NodePort Service.
6. Configured PersistentVolume and PersistentVolumeClaim.
7. Tested application using Minikube.

---

## ▶️ How to Run

### 1️⃣ Start Minikube
