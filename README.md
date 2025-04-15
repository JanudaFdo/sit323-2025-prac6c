# 🧮 Calculator App – SIT323 6.2C

This project is part of the SIT323 – Cloud Native Application Development unit at Deakin University. The application is a simple calculator built with Node.js and Docker, then deployed to a Kubernetes cluster.

## ⚙️ Technologies Used

- **Node.js** – Backend runtime
- **Express.js** – Web framework
- **Docker** – Containerization
- **Kubernetes** – Orchestration
- **kubectl** – Command-line tool for Kubernetes

## 🧪 How to Run Locally

1. **Install dependencies:**

```bash
npm install
```
   
2. Run the app:
```bash
node server.js
```
App will be available at http://localhost:3000.

🐳 Docker Usage
Build Docker Image
```bash
docker build -t calculator-app .
```
Run Docker Container
```bash
docker run -p 3000:3000 calculator-app
```

☸️ Kubernetes Deployment
Apply Kubernetes Configurations
```bash
kubectl apply -f k8s/deployment.yaml
kubectl apply -f k8s/service.yaml
```

Check Running Pods
```bash
kubectl get pods
```

Access the App
After running ```minikube service calculator-service```, a browser tab should open with your app.

