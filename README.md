# **📝 Notes App - Django**

A simple **Notes Application** built with **React** (frontend) and **Django** (backend), containerized using **Docker**, and deployed using **Jenkins CI/CD**.

---

## **🚀 Features**
✔️ Create, update, and delete notes  
✔️ REST API with Django backend  
✔️ Containerized with Docker  
✔️ Automated deployment with Jenkins  

---

## **🛠 Tech Stack**
- **Backend:** Django (Python 3.9)  
- **Frontend:** React (Node.js)  
- **Database:** SQLite/PostgreSQL  
- **Containerization:** Docker & Docker Compose  
- **Deployment:** Nginx + Jenkins  

---

## **📸 Screenshots**
![Notes App Screenshot](./screenshots/homepage.png)  
*Home Page of the Notes App*  

![Notes App Screenshot](./screenshots/add-note.png)  
*Adding a new note*  

_(Make sure you upload your screenshots to `screenshots/` in your repo.)_

---

## **🛠 Installation & Setup**  

### **🔹 Clone the Repository**
```bash
git clone https://github.com/Anushkahetawal/Notes-App-Django.git
cd Notes-App-Django
```

### **🔹 Run with Docker**
1️⃣ **Build the Docker image**  
```bash
docker build -t notes-app .
```
2️⃣ **Run the container**  
```bash
docker run -d -p 8000:8000 notes-app:latest
```

### **🔹 Running with Docker Compose**
```bash
docker-compose up -d
```

---

## **🌐 Nginx Setup**
To expose this app using **Nginx Reverse Proxy**, install Nginx and configure it:  

```bash
sudo apt update
sudo apt install nginx
```
Then configure `nginx.conf` to route traffic to the Django app.

---

## **🚀 CI/CD with Jenkins**
This project uses **Jenkins CI/CD** for automated deployment. The **Jenkinsfile** is included in this repo.

---
