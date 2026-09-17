<div align="center">

<img src="https://github.com/Itsyaboyandoy.png" width="180"/>

# Ashley B. Perado

## Learning Cloud Technologies ☁️

Bachelor of Science in Information Technology (BSIT)

University of Eastern Pangasinan (UEP)

CCM101 - Cloud Computing

Instructor: Cledmar N. Badongen

</div>

---

# 👨‍💻 About

This repository serves as my portfolio for **CCM101 – Cloud Computing**, containing laboratory activities, Linux exercises, Git and GitHub activities, cloud computing research, cloud platform comparisons, Docker exercises, containerization activities, and technical documentation completed throughout the semester.

Each laboratory reflects my progress in understanding and applying cloud computing concepts through hands-on activities.

### Areas of Learning

* Linux
* Git & GitHub
* Shell Commands
* Cloud Computing
* Cloud Infrastructure
* Cloud Platforms
* Networking
* Cloud Migration
* Docker
* Containerization
* Cloud-Native Technologies
* Technical Documentation

I enjoy learning new technologies and improving my practical skills through hands-on activities and real-world cloud computing exercises.

---

# 🛠️ Skills

* Linux
* Ubuntu
* Git
* GitHub
* Bash
* Shell Commands
* Cloud Computing
* Cloud Infrastructure
* Cloud Architecture
* Networking
* Cloud Migration
* Docker
* Containers
* Nginx
* AWS
* Microsoft Azure
* Google Cloud Platform (GCP)
* Markdown
* Technical Documentation

---

# 📚 Laboratory Activities

| Activity | Laboratory | Status |
|---|---|---|
| Lab 1 | Welcome to the Cloud | ✅ |
| Lab 2 | Build the Cloud Infrastructure Blueprint | ✅ |
| Lab 3 | Multi-Cloud Explorer | ✅ |
| Lab 4 | The Cloud-Native Engineer | ✅ |

---

# ☁️ Laboratory 1 – Welcome to the Cloud

**Mission:** Welcome to the Cloud

This laboratory introduced the fundamentals of cloud computing and Linux server environments. I used the **KillerCoda Playground** to explore a Linux server and practice basic Linux commands.

### Activities

* Explored the Linux environment
* Identified the operating system
* Checked system information
* Practiced basic Linux commands
* Investigated Linux server resources
* Created technical documentation
* Used Git and GitHub to organize laboratory outputs

### Skills Practiced

* Linux
* Ubuntu
* Shell Commands
* Git
* GitHub
* Technical Documentation

---

# 🏗️ Laboratory 2 – Build the Cloud Infrastructure Blueprint

**Mission:** Build the Cloud Infrastructure Blueprint

This laboratory focused on identifying the major components of cloud infrastructure and understanding how they work together to support cloud-based systems.

### Activities

* Investigated cloud infrastructure components
* Examined compute resources
* Studied cloud storage
* Explored networking
* Learned about Identity and Access Management (IAM)
* Created a cloud infrastructure blueprint
* Documented the investigation and findings

### Cloud Infrastructure Components

* Compute
* Storage
* Networking
* Identity and Access Management (IAM)

### Skills Practiced

* Cloud Infrastructure
* Linux
* Cloud Architecture
* Networking
* Technical Documentation
* GitHub Portfolio Management

---

# 🌐 Laboratory 3 – Multi-Cloud Explorer

**Mission:** Multi-Cloud Explorer

This laboratory focused on exploring and comparing three major cloud platforms:

* **Amazon Web Services (AWS)**
* **Microsoft Azure**
* **Google Cloud Platform (GCP)**

The laboratory included cloud platform research, service comparisons, Linux server investigation, cloud migration analysis, and client recommendations.

### Activities

* Researched AWS
* Researched Microsoft Azure
* Researched Google Cloud Platform
* Compared cloud platforms
* Mapped equivalent cloud services
* Investigated a Linux server using KillerCoda
* Analyzed cloud migration options
* Recommended cloud platforms based on different business requirements
* Documented the results using Markdown
* Organized screenshots and technical documentation in GitHub

### ☁️ Cloud Platform Services

| Category | AWS | Microsoft Azure | Google Cloud |
|---|---|---|---|
| Virtual Machines | Amazon EC2 | Azure Virtual Machines | Google Compute Engine |
| Storage | Amazon S3 | Azure Blob Storage | Google Cloud Storage |
| Database | Amazon RDS | Azure SQL Database | Cloud SQL |
| Serverless | AWS Lambda | Azure Functions | Cloud Functions |

### 🐧 Linux Investigation

The Linux server investigation used the following commands:

| Information | Linux Command |
|---|---|
| Operating System | `cat /etc/os-release` |
| CPU Information | `lscpu` |
| Memory | `free -h` |
| Disk Space | `df -h` |

### Skills Practiced

* AWS
* Microsoft Azure
* Google Cloud Platform
* Linux
* Bash
* Cloud Migration
* Cloud Service Comparison
* Cloud Architecture
* Technical Documentation
* GitHub

---

# 🐳 Laboratory 4 – The Cloud-Native Engineer

**Mission:** The Cloud-Native Engineer

This laboratory introduced the transition from traditional Virtual Machines to **containerization** and cloud-native technologies. Using the **KillerCoda Playground**, I explored Docker and deployed an Nginx web server inside a container.

The laboratory provided hands-on experience with Docker commands, container deployment, port mapping, web server testing, and container lifecycle management.

### Activities

* Compared Virtual Machines and Containers
* Explored the Docker environment using KillerCoda
* Verified the Docker installation
* Pulled the official Nginx Docker image
* Created and started an Nginx container
* Used detached mode with Docker
* Mapped host port `8080` to container port `80`
* Tested the Nginx web server using `curl`
* Listed running Docker containers
* Stopped a running container
* Verified a stopped container
* Removed a Docker container
* Verified container removal
* Documented Docker operations using Markdown
* Added screenshots as laboratory evidence

### 🐳 Docker Commands

| Command | Purpose |
|---|---|
| `docker version` | Displays Docker client and server version information. |
| `docker info` | Displays information about the Docker environment. |
| `docker pull nginx` | Downloads the official Nginx image from Docker Hub. |
| `docker run -d -p 8080:80 nginx` | Creates and starts an Nginx container while mapping host port `8080` to container port `80`. |
| `curl http://localhost:8080` | Tests the Nginx web server through the mapped port. |
| `docker ps` | Lists currently running containers. |
| `docker stop competent_panini` | Stops the running Nginx container. |
| `docker ps -a` | Lists all containers, including stopped containers. |
| `docker rm competent_panini` | Removes the stopped Nginx container. |

### 🔄 Container Lifecycle

The Nginx container was managed through the following lifecycle:

```text
Create
  ↓
Run
  ↓
Verify
  ↓
Stop
  ↓
Remove
  ↓
Verify Removal
```

The container lifecycle demonstrated how Docker containers can be created, executed, inspected, stopped, and removed using Docker CLI commands.

### 🌐 Port Mapping

The Nginx container used the following port mapping:

```text
Host Port 8080
      ↓
Container Port 80
      ↓
Nginx Web Server
```

The mapping `-p 8080:80` allowed the Nginx web server inside the container to be accessed through port `8080` on the host environment.

### Skills Practiced

* Docker
* Containerization
* Nginx
* Docker CLI
* Port Mapping
* Container Lifecycle Management
* Linux
* Bash
* Cloud-Native Concepts
* Technical Documentation
* GitHub

---

# 🔄 Virtual Machines vs. Containers

| Category | Virtual Machines | Containers |
|---|---|---|
| Architecture | Each VM includes a complete guest operating system. | Containers share the host operating system's kernel while packaging applications and dependencies. |
| Boot Time | Generally slower because a complete operating system must start. | Generally faster because a complete guest operating system does not need to boot. |
| Resource Usage | Generally requires more resources because each VM includes its own operating system. | Generally uses fewer resources because containers share the host kernel. |
| Isolation | Provides VM-level isolation. | Provides process and application-level isolation. |
| Portability | Can be moved between compatible virtualization environments. | Container images can provide consistent application environments across supported platforms. |
| Deployment | Often requires more setup and configuration. | Applications can be packaged and deployed as container images. |

### Summary

Virtual Machines and containers both provide isolated environments for running applications, but they use different approaches.

Virtual Machines virtualize complete operating systems, while containers package applications and their dependencies while sharing the host operating system's kernel. This makes containers particularly useful for lightweight application deployment, portability, and cloud-native development.

---

# ☁️ Cloud Computing Knowledge

Through these laboratory activities, I learned that cloud computing provides organizations with flexible and scalable computing resources without requiring them to maintain all physical infrastructure themselves.

I also learned that AWS, Microsoft Azure, and Google Cloud provide similar core cloud services while offering different tools, ecosystems, and service options.

Cloud-native technologies such as Docker introduced another approach to application deployment by allowing applications and their dependencies to be packaged into portable containers.

### Important Cloud Computing Concepts

* Cloud Infrastructure
* Compute
* Storage
* Networking
* Identity and Access Management
* Virtual Machines
* Containers
* Docker
* Cloud Migration
* Scalability
* Cloud-Native Technologies

---

# 📈 Portfolio Progress

This portfolio demonstrates my progression through hands-on cloud computing laboratory activities.

### Completed Learning Areas

✅ Linux Server Investigation  
✅ Cloud Infrastructure  
✅ Cloud Architecture  
✅ AWS Research  
✅ Microsoft Azure Research  
✅ Google Cloud Research  
✅ Cloud Platform Comparison  
✅ Cloud Service Mapping  
✅ Cloud Migration Analysis  
✅ Client Cloud Recommendations  
✅ Virtual Machine Investigation  
✅ Docker Fundamentals  
✅ Nginx Container Deployment  
✅ Port Mapping  
✅ Container Lifecycle Management  
✅ Git & GitHub  
✅ Technical Documentation  

---

# 🧰 Tools & Technologies

<p align="center">
  <img src="https://skillicons.dev/icons?i=linux,ubuntu,git,github,md,bash,vscode,docker,aws,azure,gcp" />
</p>

### Development & Cloud Tools

* **Ubuntu Linux**
* **KillerCoda Playground**
* **Git**
* **GitHub**
* **Markdown**
* **Bash**
* **Docker**
* **Nginx**
* **Amazon Web Services (AWS)**
* **Microsoft Azure**
* **Google Cloud Platform (GCP)**
* **Visual Studio Code**

---

# 📂 Repository Structure

```text
CCM101-aperado/
│
├── Laboratory-01-Welcome-to-the-Cloud/
│
├── Laboratory-02-Build-the-Cloud-Infrastructure-Blueprint/
│
├── Laboratory-03-Multi-Cloud-Explorer/
│
├── Laboratory-04-Cloud-Native-Engineer/
│   ├── Screenshots/
│   │   ├── Checkpoint-1.png
│   │   ├── Container-lifecycle.png
│   │   ├── Docker-version.png
│   │   └── Nginx-running.png
│   │
│   ├── README.md
│   ├── docker-deployment.md
│   ├── reflection.md
│   └── virtualization-vs-containers.md
│
└── README.md
```

---

# 🎯 Learning Journey

My CCM101 Cloud Computing portfolio documents my progression from fundamental Linux concepts to cloud infrastructure, multi-cloud environments, and cloud-native technologies.

### Learning Progression

```text
Linux Fundamentals
       ↓
Cloud Infrastructure
       ↓
Multi-Cloud Platforms
       ↓
Cloud Migration
       ↓
Virtual Machines
       ↓
Containers & Docker
       ↓
Cloud-Native Technologies
```

Each laboratory has provided hands-on experience that builds upon the previous activities. The progression has helped me develop a broader understanding of how modern cloud infrastructure is designed, deployed, managed, and documented.

---

# 📬 Contact

**Email:** [ashperado63@email.com](mailto:ashperado63@email.com)

**GitHub:** https://github.com/Itsyaboyandoy

---

# ☁️ Cloud Computing Journey

My goal throughout CCM101 is to develop practical knowledge that I can apply to future **Information Technology, cloud computing, networking, infrastructure, and software development projects**.

This repository serves as a record of my laboratory activities, technical documentation, hands-on exercises, and continued learning in cloud computing.

As I complete additional laboratory activities, I will continue improving this portfolio and expanding my knowledge of modern cloud and cloud-native technologies.

---

<div align="center">

### ☁️ Learning. Building. Documenting. Growing. 🚀

**CCM101 – Cloud Computing**

**Ashley B. Perado | BSIT | University of Eastern Pangasinan**

</div>
