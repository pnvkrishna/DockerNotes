# 🚀 Docker Interview Q&A with Real-Time Scenarios

## 1️⃣ What are the major components of Docker?
**Answer:**  
Docker has three main components:
- **Docker Client** → Used to run docker commands
- **Docker Daemon (Server)** → Executes commands and manages containers
- **Docker Registry** → Stores images (ex: Docker Hub)

**Real-Time Scenario:**  
Developer runs `docker run nginx` → Client sends request → Daemon pulls image from Docker Hub → Starts container.

---

## 2️⃣ What is a Docker Repository?
**Answer:**  
A repository is a storage location inside a registry that holds one or more versions (tags) of a Docker image.

**Real-Time Scenario:**  
Your team maintains a **private repository** for application images in AWS ECR/GitHub Container Registry.

---

## 3️⃣ What is Docker Client?
**Answer:**  
CLI tool where we execute commands (`docker run`, `docker ps`) which are sent to Docker daemon.

**Real-Time Scenario:**  
A DevOps engineer uses Docker CLI in a CI/CD pipeline to build and push images to registry.

---

## 4️⃣ What is Docker Server (Daemon)?
**Answer:**  
A background service that handles building, running, and managing containers.

**Real-Time Scenario:**  
Daemon pulls images from the registry, starts containers on production nodes in Kubernetes.

---

## 5️⃣ What is NGINX?
**Answer:**  
NGINX is a lightweight web server, reverse proxy, and load balancer commonly used in container environments.

**Real-Time Scenario:**
In microservices, NGINX acts as a reverse proxy — directing API traffic to backend services inside containers.

---

## 6️⃣ What is a Docker Image?
**Answer:**  
Image is a lightweight and read-only template used to create containers.

**Real-Time Scenario:**
A Java developer builds an application once → creates an image → Same image runs in Dev, QA, and Prod without changes.

---

## 7️⃣ What is Docker Hub?
**Answer:**  
A public Docker registry where users can upload and download container images.

**Real-Time Scenario:**  
You run `docker pull tomcat` → Docker Hub provides the official Tomcat image.

---

## 8️⃣ What is a Docker Tag?
**Answer:**  
A tag refers to a specific version of an image (ex: `nginx:1.25`, `tomcat:9.0`).

**Real-Time Scenario:**  
Prod requires stable version:  
`docker pull myapp:v1.0` → Ensures no accidental version upgrade.

---

## 9️⃣ What is a Docker Command?
**Answer:**  
A Docker command is used to manage images, containers, networks, volumes, etc.

Examples:
- `docker run`
- `docker ps`
- `docker stop`

**Real-Time Scenario:**  
Developer runs `docker logs app` to debug production issue.

---

## 🔟 What is Tomcat?
**Answer:**  
Tomcat is an open-source web/application server used to deploy Java-based applications (WAR files).

**Real-Time Scenario:**  
Java app is deployed inside Tomcat container in AWS/ECS or Kubernetes cluster using CI/CD.

---

### 📝 Exercise
Run a Tomcat container using Docker with a single command.

---
