<div align="center">

# ☁️ Cloud Infrastructure Blueprint

### Laboratory 02 — Cloud Computing

**CCM101 | University of Eastern Pangasinan**

**Ashley B. Perado**

---

![Ubuntu](https://img.shields.io/badge/Ubuntu-24.04.4-orange?style=for-the-badge&logo=ubuntu)
![Linux](https://img.shields.io/badge/Linux-Server-black?style=for-the-badge&logo=linux)
![GitHub](https://img.shields.io/badge/GitHub-Portfolio-181717?style=for-the-badge&logo=github)
![Markdown](https://img.shields.io/badge/Markdown-Documentation-000000?style=for-the-badge&logo=markdown)

</div>

---

# Technical Documentation

## 1. Mission Overview

Congratulations,

Your onboarding has been successfully completed, and your Cloud Computing Portfolio has been approved by your supervisor.

CloudNova Technologies has now assigned you to your first official project.

Before deploying cloud services, every cloud engineer must understand the infrastructure that powers modern cloud computing. This mission focuses on investigating the fundamental components of cloud infrastructure and understanding how **compute, storage, networking, operating systems, and identity services** work together.

Using the **KillerCoda Playground**, Linux command-line tools, official cloud documentation, and GitHub, this laboratory simulates the planning and investigation phase of a cloud deployment.

> **Great cloud engineers build systems — exceptional cloud engineers document and justify every design decision.**

---

# 2. Objectives

The objectives of this laboratory activity were to:

- Explain the major components of cloud infrastructure.
- Investigate hardware and software resources available in a Linux environment.
- Differentiate compute, storage, networking, and identity resources.
- Interpret the relationship between cloud infrastructure components.
- Create professional technical documentation using Markdown.
- Continue building a structured GitHub Cloud Computing Portfolio.
- Investigate a cloud-based Linux environment using command-line tools.
- Compare infrastructure services provided by major cloud platforms.

---

# 3. Cloud Infrastructure Components

The investigation identified the following major infrastructure components in the KillerCoda environment.

## 3.1 Compute Resources

The server uses an **Intel Xeon E312xx (Sandy Bridge) virtual CPU** with **1 available CPU core**.

Compute resources provide the processing capability required to:

- Execute commands
- Run applications
- Process data
- Execute workloads
- Support cloud services

In cloud computing, compute resources are commonly delivered through virtual machines, containers, and other virtualized environments.

---

## 3.2 Storage Resources

The primary storage resource identified during the investigation was:

| Resource | Information |
|---|---|
| Device | `/dev/vda1` |
| Capacity | 19 GB |
| Used | 5.4 GB |
| Available | 13 GB |
| Mount Point | `/` |

Storage resources provide persistent space for:

- Operating-system files
- Applications
- Configuration files
- User data
- Logs and other system information

Reliable storage is essential for maintaining applications and data in cloud environments.

---

## 3.3 Networking Resources

The Linux server was assigned the following IP addresses:

| Network Information | Result |
|---|---|
| Hostname | `ubuntu` |
| IP Address | `172.30.1.2` |
| Additional IP | `172.17.0.1` |

Networking resources allow servers, applications, users, and other cloud services to communicate.

In a cloud environment, networking typically includes:

- IP addresses
- Virtual networks
- Subnets
- Routing
- Firewalls
- Network security controls

---

## 3.4 Operating System

The server operates using:

| Component | Result |
|---|---|
| Operating System | Ubuntu 24.04.4 LTS |
| Distribution | Ubuntu |
| Codename | Noble |
| Kernel | `6.8.0-138-generic` |

The operating system manages and coordinates the server's compute, memory, storage, networking, and application resources.

Ubuntu Linux provides the command-line environment used to investigate and manage the cloud server.

---

## 3.5 Identity and Access Management

Identity and Access Management (IAM) determines **who can access cloud resources and what actions they are permitted to perform**.

Examples of cloud IAM services include:

| Cloud Provider | IAM Service |
|---|---|
| Amazon Web Services | AWS IAM |
| Microsoft Azure | Azure RBAC |
| Google Cloud | Cloud IAM |

IAM is an important component of cloud infrastructure because it helps protect resources from unauthorized access and allows organizations to control user permissions.

---

# 4. Infrastructure Investigation Results

The following information was collected from the KillerCoda Linux environment.

| Infrastructure Resource | Investigation Result |
|---|---|
| **Operating System** | Ubuntu 24.04.4 LTS |
| **Kernel Version** | `6.8.0-138-generic` |
| **CPU Model** | Intel Xeon E312xx (Sandy Bridge) |
| **CPU Cores** | 1 |
| **Total RAM** | 1.9 GiB |
| **Available RAM** | 1.4 GiB |
| **Disk Capacity** | 19 GB |
| **Available Disk Space** | 13 GB |
| **Main Filesystem** | `/dev/vda1` |
| **Hostname** | `ubuntu` |
| **IP Address** | `172.30.1.2` |
| **Additional IP** | `172.17.0.1` |

---

# 5. Tools Used

The following tools and technologies were used during the laboratory activity:

| Tool | Purpose |
|---|---|
| **KillerCoda Playground** | Provided the cloud-based Linux environment |
| **Ubuntu Linux** | Operating system investigated during the activity |
| **Linux Terminal** | Used to execute system investigation commands |
| **Bash** | Command-line environment |
| **Git** | Version control |
| **GitHub** | Repository hosting and portfolio management |
| **draw.io** | Cloud infrastructure architecture diagram |
| **Markdown** | Technical documentation |
| **AWS Documentation** | Cloud service research |
| **Microsoft Azure Documentation** | Cloud service research |
| **Google Cloud Documentation** | Cloud service research |

---

# 6. Linux Commands Executed

The following commands were used to create, navigate, inspect, and document the cloud environment.

## 6.1 Directory and File Management

```bash
cd ~/CCM101-aperado

mkdir -p Laboratory-02-Build-the-Cloud-Infrastructure-Blueprint

cd Laboratory-02-Build-the-Cloud-Infrastructure-Blueprint

mkdir screenshots

touch README.md infrastructure-report.md cloud-components.md cloud-provider-comparison.md reflection.md

pwd

ls -la

ls -la screenshots
