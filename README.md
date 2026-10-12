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

This repository serves as my portfolio for **CCM101 – Cloud Computing**, containing laboratory activities, Linux exercises, Git and GitHub activities, cloud computing research, cloud platform comparisons, Docker exercises, containerization activities, object storage deployment, and technical documentation completed throughout the semester.

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
* Cloud Storage
* Object Storage
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
* MinIO
* Object Storage
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
| Lab 5 | The Cloud Data Engineer | ✅ |

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

# 🪣 Laboratory 5 – The Cloud Data Engineer

**Mission:** The Cloud Data Engineer

This laboratory focused on cloud storage and how modern applications store large amounts of unstructured data such as photos, videos, and backups. Acting as a cloud data engineer for a photo-sharing client, I deployed an S3-compatible **MinIO** object storage server using Docker on the **KillerCoda Playground**, created a storage bucket, and uploaded a test file to confirm the system worked.

The laboratory combined the Docker skills from Laboratory 4 with cloud storage concepts, including port mapping, environment variables, and managing a service through its web console.

### Activities

* Compared Block Storage, File Storage, and Object Storage
* Explained why Object Storage suits user-uploaded images
* Deployed a MinIO object storage server using Docker
* Set the administrator login using environment variables
* Mapped the MinIO API port `9000` and the web console port `9001`
* Verified the running container with `docker ps`
* Tested the server with a `curl` health check
* Accessed the MinIO Web Console through KillerCoda port forwarding
* Created a bucket named `client-photos`
* Uploaded a sample file to the bucket
* Troubleshot an image pull error and used a mirror image to continue
* Documented the deployment using Markdown
* Added screenshots as laboratory evidence

### 🗄️ Cloud Storage Types

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Stores data in fixed-size blocks attached to a server. | Operating systems and databases. | AWS EBS |
| File Storage | Stores data as files in a shared folder hierarchy. | Shared files across multiple servers. | AWS EFS |
| Object Storage | Stores data as objects with metadata and unique IDs in buckets. | Photos, videos, and backups at large scale. | AWS S3 |

### 🐳 MinIO Deployment

| Item | Detail |
|---|---|
| Server | MinIO (S3-compatible object storage) |
| Environment | KillerCoda Ubuntu Playground |
| Container Name | `minio-server` |
| API Port | `9000` |
| Web Console Port | `9001` |
| Bucket Created | `client-photos` |

### ⚠️ Troubleshooting

The image `minio/minio` from the lab instructions could not be pulled because MinIO no longer publishes its container images on Docker Hub. I replaced only the image name with a community mirror of the last official release and kept the ports, environment variables, and server command the same.

### 🪣 Bucket Storage Flow

```text
User Uploads File
       ↓
MinIO Web Console (Port 9001)
       ↓
Bucket: client-photos
       ↓
Object Stored in MinIO
```

### Skills Practiced

* Object Storage
* MinIO
* Docker
* Environment Variables
* Port Mapping
* Cloud Storage Concepts
* Troubleshooting
* Linux
* Bash
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

Cloud storage showed me that not all data is stored the same way. Block, file, and object storage each serve different needs, and object storage is well suited for large amounts of unstructured data such as user-uploaded photos because it scales easily and is accessed over the web.

### Important Cloud Computing Concepts

* Cloud Infrastructure
* Compute
* Storage
* Block, File, and Object Storage
* Buckets
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
✅ Cloud Storage Types Research  
✅ MinIO Object Storage Deployment  
✅ Bucket Creation and File Upload  
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
* **MinIO**
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
├── Laboratory-05-Cloud-Data-Engineer/
│   ├── screenshots/
│   │   ├── minio-deployed.png
│   │   └── minio-bucket-upload.png
│   │
│   ├── README.md
│   ├── storage-types-research.md
│   ├── minio-deployment.md
│   └── reflection.md
│
└── README.md
````

---

# 🎯 Learning Journey

My CCM101 Cloud Computing portfolio documents my progression from fundamental Linux concepts to cloud infrastructure, multi-cloud environments, cloud-native technologies, and cloud storage.

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
       ↓
Cloud Storage & Object Storage
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
