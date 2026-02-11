# 🚀 Flask Application Deployment using Docker & Kubernetes (Minikube)

## 📌 Project Overview

This project demonstrates containerization and deployment of a Python Flask web application using Docker and Kubernetes.

The application is containerized using Docker and deployed on a local Kubernetes cluster using Minikube.  
It also includes Kubernetes resources like Deployment, Service (NodePort), PersistentVolume (PV), and PersistentVolumeClaim (PVC).

---

## 🛠 Tech Stack

- Python (Flask)
- Docker
- Kubernetes
- Minikube

---

## 📂 Project Structure

```
flask-docker-k8s/
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
```

---

## ⚙️ What This Project Demonstrates

- Creating a simple Flask web application
- Containerizing the application using Docker
- Building and pushing Docker image to Docker Hub
- Creating Kubernetes Deployment
- Exposing application using NodePort Service
- Configuring PersistentVolume (PV)
- Configuring PersistentVolumeClaim (PVC)
- Deploying and testing application on Minikube

---

## 🐳 Docker Workflow

### Build Docker Image

```
docker build -t flask-app .
```

### Run Docker Container (Optional Local Test)

```
docker run -p 5000:5000 flask-app
```

Access at:

```
http://localhost:5000
```

---

## ☸️ Kubernetes Deployment Steps

### 1️⃣ Start Minikube

```
minikube start
```

### 2️⃣ Apply Kubernetes Manifests

```
kubectl apply -f deployment.yaml
kubectl apply -f pv.yaml
kubectl apply -f pvc.yaml
kubectl apply -f service.yaml
```

### 3️⃣ Verify Resources

```
kubectl get pods
kubectl get svc
kubectl get pv
kubectl get pvc
```

### 4️⃣ Access the Application

```
minikube service flask-app-service
```

---

## 📊 Kubernetes Resources Used

- **Deployment** – Manages application pods
- **Service (NodePort)** – Exposes application externally
- **PersistentVolume (PV)** – Provides storage to cluster
- **PersistentVolumeClaim (PVC)** – Requests storage from PV

---

## 🎯 Learning Outcomes

Through this project, I gained hands-on experience with:

- Docker containerization
- Kubernetes architecture
- Pod & Service networking
- Persistent storage in Kubernetes
- Deploying applications on Minikube
- Structuring DevOps projects for GitHub

