# 🚀 Dockerized NGINX Static Website

## 📌 Project Overview
This project demonstrates containerizing a static web application using Docker and deploying it with the official NGINX image on Ubuntu Linux.

The website is built using HTML and served through an NGINX container with port mapping. The application was tested using VirtualBox networking (NAT/Bridged Adapter).

---

## 🛠 Technologies Used
- Ubuntu Linux
- NGINX
- Docker
- Git & GitHub
- VirtualBox Networking

---

## 📂 Project Structure

```
index.html
Dockerfile
README.md
```

---

## 🐳 Dockerfile

```dockerfile
FROM nginx:latest
COPY . /usr/share/nginx/html
EXPOSE 80
```

---

## 🔧 How to Run the Project

### 1️⃣ Build Docker Image
```
sudo docker build -t mywebsite .
```

### 2️⃣ Run Docker Container
```
sudo docker run -d -p 8080:80 mywebsite
```

### 3️⃣ Access in Browser
```
http://<your-server-ip>:8080
```

---

## 🎯 Key Concepts Learned
- Docker image creation
- Container lifecycle management
- Port mapping (8080:80)
- Serving static applications using NGINX
- Basic Linux server handling
- Git remote repository management
- Virtual machine networking configuration

---

## 📈 Outcome
Successfully deployed and accessed a containerized static website from the host system browser, demonstrating understanding of containerization and networking fundamentals.
