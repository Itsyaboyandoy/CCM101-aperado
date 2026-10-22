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

This repository serves as my portfolio for **CCM101 – Cloud Computing**, containing laboratory activities, Linux exercises, Git and GitHub activities, cloud computing research, cloud platform comparisons, Docker exercises, containerization activities, object storage deployment, multi-container deployment with Docker Compose, system monitoring and observability, and technical documentation completed throughout the semester.

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
* Docker Compose
* Multi-Tier Architecture
* Infrastructure as Code (IaC)
* Monitoring & Observability
* Log Analysis
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
* Nano
* Cloud Computing
* Cloud Infrastructure
* Cloud Architecture
* Networking
* Cloud Migration
* Docker
* Docker Compose
* YAML
* Containers
* Nginx
* MinIO
* Nextcloud
* MariaDB
* Object Storage
* Infrastructure as Code (IaC)
* System Monitoring
* Container Observability
* Log Analysis
* curl
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
| Lab 6 | The Cloud Deployment Engineer | ✅ |
| Lab 7 | The Cloud Operations Engineer | ✅ |

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

# 🧩 Laboratory 6 – The Cloud Deployment Engineer

**Mission:** The Cloud Deployment Engineer

This laboratory moved from deploying single containers to deploying a **multi-tier application**. Acting as a cloud deployment engineer for a university client that wanted its own private cloud storage system, I used **Docker Compose** to define and deploy a two-tier **Nextcloud** and **MariaDB** stack on the **KillerCoda Playground** with a single command.

The laboratory introduced **Infrastructure as Code (IaC)**: instead of typing a separate command for each container, the whole environment was described in one `docker-compose.yml` file that can be reviewed, repeated, and shared.

### Activities

* Defined a two-tier architecture with a web/application tier and a database tier
* Explained why the tiers run in separate containers
* Created a project directory and a `docker-compose.yml` file using the `nano` text editor
* Defined two services, `app` (Nextcloud) and `database` (MariaDB 10.6), in YAML
* Connected the app to the database using the `MYSQL_HOST` environment variable
* Mapped host port `8080` to container port `80`
* Deployed both containers with `docker-compose up -d`
* Verified the running containers with `docker-compose ps`
* Accessed the Nextcloud setup page through KillerCoda port forwarding
* Shut down the stack with `docker-compose down`
* Documented the Compose file and deployment using Markdown
* Added screenshots as laboratory evidence

### 🏗️ Two-Tier Architecture

| Tier | Service | Image | Role |
|---|---|---|---|
| Web/Application | `app` | `nextcloud` | Serves the web interface and handles user requests |
| Database | `database` | `mariadb:10.6` | Stores user accounts and file metadata |

```text
Browser
   ↓
Host Port 8080
   ↓
app (Nextcloud) — container port 80
   ↓  MYSQL_HOST=database
database (MariaDB) — internal port 3306
```

### 🐳 Docker Compose Commands

| Command | Purpose |
|---|---|
| `mkdir nextcloud-deployment` | Creates the project directory. |
| `cd nextcloud-deployment` | Moves into the project directory. |
| `nano docker-compose.yml` | Opens the text editor to create the Compose file. |
| `cat docker-compose.yml` | Displays the file to check its contents and indentation. |
| `docker-compose up -d` | Pulls the images and starts all services in the background. |
| `docker-compose ps` | Lists the containers in the project and their state. |
| `docker-compose down` | Stops and removes the containers and the project network. |

### 🔄 Deployment Lifecycle

```text
Write docker-compose.yml
          ↓
docker-compose up -d
          ↓
Verify with docker-compose ps
          ↓
Access Nextcloud on Port 8080
          ↓
docker-compose down
```

### Skills Practiced

* Docker Compose
* YAML
* Infrastructure as Code (IaC)
* Multi-Tier Architecture
* Nextcloud
* MariaDB
* Environment Variables
* Port Mapping
* Linux
* Nano
* Technical Documentation
* GitHub

---

# 📊 Laboratory 7 – The Cloud Operations Engineer

**Mission:** The Cloud Operations Engineer

This laboratory focused on **observability and monitoring**, the work of keeping a deployed application healthy. Acting as a Cloud Operations Engineer for a client preparing a large marketing campaign, I checked the health of the host server, deployed the client's Nginx web server in a container, generated test traffic, and used logs and real-time metrics to confirm the infrastructure could handle the expected visitors. The work was done on the **KillerCoda Playground**.

The laboratory showed that deploying an application is only the first step: engineers use measurements and records, not guesses, to prove a system is working.

### Activities

* Checked the server's memory usage with `free -h`
* Checked the root file system's disk capacity with `df -h`
* Observed running processes and CPU load with `top`
* Recorded a host baseline of the server's total RAM and root storage
* Deployed an Nginx container named `client-website` on port `8080`
* Simulated website visitors by sending HTTP requests with `curl`
* Triggered an HTTP 404 error by requesting a page that does not exist
* Retrieved application logs with `docker logs` and identified the 200 and 404 responses
* Monitored real-time container CPU, memory, and network usage with `docker stats`
* Recorded the container's memory and CPU usage
* Documented the baseline, logs, and metrics using Markdown
* Added screenshots as laboratory evidence

### 🖥️ Host System Baseline

| Resource | Value | Command Used |
|---|---|---|
| Total RAM | 1.9Gi | `free -h` |
| Root (/) Storage Capacity | 19G | `df -h` |

### 📈 Monitoring Commands

| Command | Purpose |
|---|---|
| `free -h` | Displays total, used, and available memory in readable units. |
| `df -h` | Displays disk capacity and usage for each file system. |
| `top` | Shows running processes and CPU load in real time. |
| `docker run -d -p 8080:80 --name client-website nginx` | Starts the client's Nginx container in the background and maps host port `8080` to container port `80`. |
| `curl http://localhost:8080` | Simulates a visitor requesting the home page. |
| `curl http://localhost:8080/hidden-admin-page` | Simulates a visitor requesting a page that does not exist. |
| `docker logs client-website` | Displays the application logs from the container. |
| `docker stats` | Shows live CPU, memory, and network usage for running containers. |

### 🌐 Simulated Traffic and Log Results

| Request | HTTP Status |
|---|---|
| Home page (`/`), sent three times | `200 OK` |
| `/hidden-admin-page` | `404 Not Found` |

### 📋 Container Metrics

| Container | Memory Usage | CPU % |
|---|---|---|
| `client-website` | 2.773MiB | 0.00% |

### 🔍 Logs vs. Metrics

| | Logs | Metrics |
|---|---|---|
| What they show | Individual events, such as a request that returned a `404` | Numerical measurements, such as CPU, memory, and network usage |
| Command used | `docker logs client-website` | `docker stats` |
| Answers the question | What happened? | How is the container performing? |

### 🔄 Monitoring Workflow

```text
Check Host Baseline (RAM, Disk, CPU)
              ↓
Deploy Nginx Container
              ↓
Generate Traffic (200 and 404)
              ↓
Review Application Logs
              ↓
Review Real-Time Container Metrics
```

### Skills Practiced

* System Monitoring
* Linux Command Line
* Container Observability
* Log Analysis
* Docker
* Nginx
* HTTP Status Codes
* Troubleshooting
* curl
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

Docker Compose showed me that real applications are usually made of several connected containers. Describing the whole environment in one YAML file made the deployment easier to repeat and review than typing separate commands for each container.

Monitoring and observability showed me that running an application is not enough: its health has to be measured. Checking the host's memory and disk, reading container logs, and watching real-time metrics gave me evidence of how a system behaves instead of assumptions.

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
* Multi-Tier Architecture
* Docker Compose
* Infrastructure as Code (IaC)
* Monitoring and Observability
* Logs and Metrics
* HTTP Status Codes
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
✅ Multi-Tier Architecture Research  
✅ Docker Compose File Creation  
✅ Nextcloud and MariaDB Deployment  
✅ Infrastructure as Code Fundamentals  
✅ Host System Baseline Monitoring  
✅ Web Traffic Simulation  
✅ Container Log Analysis  
✅ Real-Time Container Metrics  
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
* **Nano**
* **Docker**
* **Docker Compose**
* **Nginx**
* **MinIO**
* **Nextcloud**
* **MariaDB**
* **curl**
* **Linux Monitoring Tools (`free`, `df`, `top`)**
* **Docker Monitoring Tools (`docker logs`, `docker stats`)**
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
├── Laboratory-06-Cloud-Deployment-Engineer/
│   ├── screenshots/
│   │   ├── compose-deployment.png
│   │   ├── nextcloud-web.png
│   │   └── compose-teardown.png
│   │
│   ├── README.md
│   ├── multi-tier-architecture.md
│   ├── docker-compose-guide.md
│   └── reflection.md
│
├── Laboratory-07-Cloud-Operations-Engineer/
│   ├── screenshots/
│   │   ├── memory-check.png
│   │   ├── disk-check.png
│   │   ├── install-nginx.png
│   │   ├── simulation1.png
│   │   ├── simulation2.png
│   │   ├── docker-logs.png
│   │   └── container-metrics.png
│   │
│   ├── README.md
│   ├── system-baseline-report.md
│   ├── container-observability.md
│   └── reflection.md
│
└── README.md
```

---

# 🎯 Learning Journey

My CCM101 Cloud Computing portfolio documents my progression from fundamental Linux concepts to cloud infrastructure, multi-cloud environments, cloud-native technologies, cloud storage, multi-container deployment, and system monitoring.

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
       ↓
Docker Compose & Infrastructure as Code
       ↓
Monitoring & Observability
```

Each laboratory has provided hands-on experience that builds upon the previous activities. The progression has helped me develop a broader understanding of how modern cloud infrastructure is designed, deployed, managed, monitored, and documented.

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
