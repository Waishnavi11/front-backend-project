# Front-Backend Project (MEAN Stack)

This project is a full-stack CRUD application built with **MongoDB, Express, Angular 15, and Node.js (MEAN stack)**.  
It demonstrates **containerization, deployment with Docker Compose**, and **CI/CD automation using GitHub Actions**. The frontend and backend are served via **Nginx reverse proxy**.

---

## **Project Overview**

- **Backend:** Node.js + Express REST API connected to MongoDB.  
- **Frontend:** Angular 15 application using HTTPClient to interact with backend APIs.  
- **Database:** MongoDB (Docker container).  
- **Containerization:** Docker & Docker Compose for all services.  
- **CI/CD:** GitHub Actions workflow to build Docker images, push to Docker Hub, and update VM.  
- **Reverse Proxy:** Nginx serves frontend and backend via port 80.  

---

## **Setup & Deployment**

All steps have been completed:

1. Repository cloned and Dockerfiles created for frontend & backend.  
2. Docker images built and pushed to Docker Hub.  
3. Ubuntu VM set up with Docker and Docker Compose.  
4. Application deployed via `docker compose up -d`.  
5. MongoDB running as a Docker container.  
6. Nginx configured as a reverse proxy.  
7. GitHub Actions CI/CD workflow configured and verified.

**Application Access:**  

http://<SERVER_IP>

---

## **CI/CD Pipeline**

The GitHub Actions workflow:![WhatsApp Image 2025-11-28 at 8 17 18 PM (1)]



- Builds Docker images for frontend and backend.  
- Pushes images to Docker Hub.  
- SSHs into the Ubuntu VM and runs:
```bash
sudo docker compose pull
sudo docker compose up -d
Automatically updates containers on VM on each push.





