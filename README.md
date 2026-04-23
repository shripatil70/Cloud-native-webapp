# 🚀 Cloud-Native Scalable Web Application

A production-style cloud application built using **Flask**, **Docker**, and **AWS services** including EC2, Application Load Balancer (ALB), Auto Scaling, and CloudWatch.

---

## 🧠 Architecture Overview

**Flow:**  
User → ALB → Auto Scaling Group (EC2 Instances) → Docker → Flask App

- Load Balancer distributes incoming traffic  
- Auto Scaling dynamically launches/terminates EC2 instances  
- Docker ensures consistent deployment  
- CloudWatch monitors system performance  

---

## ⚙️ Tech Stack

- Python (Flask)  
- Docker  
- AWS EC2  
- AWS Application Load Balancer (ALB)  
- AWS Auto Scaling Group (ASG)  
- AWS CloudWatch  

---

## 🚀 Features

- ✅ Containerized Flask application  
- ✅ Load-balanced traffic distribution  
- ✅ Auto Scaling for high availability  
- ✅ Multi-AZ deployment  
- ✅ Real-time monitoring with CloudWatch  

---

## 🌐 Live Demo

👉 [http://flask-alb-1121615369.ap-south-1.elb.amazonaws.com/](http://flask-alb-1121615369.ap-south-1.elb.amazonaws.com/)

---

## 📊 CloudWatch Metrics (Proof of Performance)

### 1️⃣ Request Count (Traffic Monitoring)
![RequestCount](https://github.com/shripatil70/Cloud-native-webapp/blob/e76ebab10881d675060df980e2dd49c827f98033/Outputs/request_count.png)  
- Shows number of incoming requests handled by ALB  

---

### 2️⃣ Target Response Time (~0.1s)
![ResponseTime](https://github.com/shripatil70/Cloud-native-webapp/blob/e76ebab10881d675060df980e2dd49c827f98033/Outputs/target_response.png)  
- Demonstrates low-latency response under load  

---

### 3️⃣ Target Group Health
![HealthyHosts](https://github.com/shripatil70/Cloud-native-webapp/blob/e76ebab10881d675060df980e2dd49c827f98033/Outputs/target_group_health.png)  

---

### 4️⃣ EC2 Output
![ActiveConnections](https://github.com/shripatil70/Cloud-native-webapp/blob/e76ebab10881d675060df980e2dd49c827f98033/Outputs/ec2_output.png)  
- Displays Output EC2 DNS
---

### 5️⃣ Docker Connection
![LCU](https://github.com/shripatil70/Cloud-native-webapp/blob/e76ebab10881d675060df980e2dd49c827f98033/Outputs/docker_terminal.png)  

---

## 📸 Architecture Diagram
![Architecture](https://github.com/shripatil70/Cloud-native-webapp/blob/8122c72b192a3b3de103dae942bdcaaa23fa895e/Outputs/cloud-native-architecture.png)

---

# 🛠️ Setup Instructions

### 1. Clone Repository
```bash
git clone https://github.com/shripatil70/cloud-native-webapp.git
cd cloud-native-webapp
```

### 2. Build Docker Image
```bash
docker build -t flask-app .
```

### 3. Run Container
```bash
docker run -p 5000:5000 flask-app
```

### 4. Access Locally
```bash
http://localhost:5000
```

---

# AWS Deployment Steps (Summary)

- **Launch EC2 instance**
- **Install Docker & Git**
- **Clone repo and run container**
- **Create Application Load Balancer**
- **Create Target Group**
- **Configure Auto Scaling Group**
- **Attach ALB to ASG**
- **Monitor using CloudWatch**

## 🎯 Key Achievements

- ⚡ Achieved ~0.1s response time using ALB routing
- 🔄 Enabled automatic scaling based on demand
- 🟢 Maintained high availability using multi-instance architecture
- 📊 Implemented real-time monitoring using CloudWatch

## 🔮 Future Improvements

- Add CI/CD using AWS CodePipeline
- Add HTTPS (SSL via ACM)
- Integrate custom domain (Route 53)
- Push Docker image to Docker Hub

## 👨‍💻 Author
*Dhanashri Patil*


