<div align="center">

# ☁️ Cloud Infrastructure Blueprint

### Laboratory 02 — Build the Cloud Infrastructure Blueprint

**CCM101 — Cloud Computing**

**Ashley B. Perado**

**Bachelor of Science in Information Technology (BSIT)**  
**University of Eastern Pangasinan (UEP)**

---

![Ubuntu](https://img.shields.io/badge/Ubuntu-24.04.4-orange?style=for-the-badge&logo=ubuntu)
![Linux](https://img.shields.io/badge/Linux-Server-black?style=for-the-badge&logo=linux)
![Git](https://img.shields.io/badge/Git-Version_Control-F05032?style=for-the-badge&logo=git)
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
- Investigate the hardware and software resources available in a Linux environment.
- Differentiate compute, storage, networking, and identity resources.
- Interpret the relationship between cloud infrastructure components.
- Create professional technical documentation using Markdown.
- Continue building a structured GitHub Cloud Computing Portfolio.

---

# 3. Cloud Infrastructure Components

The main cloud infrastructure components identified in the KillerCoda environment were:

## 3.1 Compute Resources

The server uses an **Intel Xeon E312xx (Sandy Bridge) virtual CPU** with **1 available CPU core**.

Compute resources provide the processing capability required to:

- Execute commands
- Run applications
- Process data
- Execute workloads
- Support cloud services

In cloud computing, compute resources are commonly provided through virtual machines, containers, and other virtualized environments.

---

## 3.2 Storage Resources

The primary storage resource identified during the investigation was the **`/dev/vda1`** partition with a capacity of approximately **19 GB**.

| Storage Information | Result |
|---|---|
| Device | `/dev/vda1` |
| Capacity | 19 GB |
| Used Space | Approximately 5.4 GB |
| Available Space | Approximately 13 GB |
| Mount Point | `/` |

Storage resources provide persistent space for the operating system, applications, configuration files, logs, and other data.

---

## 3.3 Networking Resources

The server has network connectivity through the following IP addresses:

| Network Information | Result |
|---|---|
| Hostname | `ubuntu` |
| IP Address | `172.30.1.2` |
| Additional IP Address | `172.17.0.1` |

Networking resources allow the server, applications, users, and other cloud resources to communicate with each other and with external networks.

In cloud computing, networking commonly involves:

- IP addresses
- Virtual networks
- Subnets
- Routing
- Firewalls
- Network security controls

---

## 3.4 Operating System

The server runs:

| System Information | Result |
|---|---|
| Operating System | Ubuntu 24.04.4 LTS |
| Codename | Noble |
| Kernel Version | `6.8.0-138-generic` |
| Architecture | x86_64 |

The operating system manages and coordinates the available compute, memory, storage, networking, and application resources.

Ubuntu Linux also provides the command-line environment used to investigate and manage the cloud server.

---

## 3.5 Identity and Access Management

Identity and Access Management (IAM) determines **who can access cloud resources and what actions they are permitted to perform**.

Examples of cloud identity and access services include:

| Cloud Provider | Identity and Access Service |
|---|---|
| Amazon Web Services | AWS IAM |
| Microsoft Azure | Azure RBAC |
| Google Cloud Platform | Cloud IAM |

IAM is important in cloud computing because it helps protect resources from unauthorized access and provides controlled permissions for users and services.

---

# 4. Infrastructure Investigation Results

The following information was collected from the KillerCoda Linux environment:

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

The following Linux commands were used to create, navigate, inspect, and document the cloud environment.

## 6.1 Directory and File Commands

```bash
cd ~/CCM101-aperado

mkdir -p Laboratory-02-Build-the-Cloud-Infrastructure-Blueprint

cd Laboratory-02-Build-the-Cloud-Infrastructure-Blueprint

mkdir screenshots

touch README.md infrastructure-report.md cloud-components.md cloud-provider-comparison.md reflection.md

pwd

ls -la

ls -la screenshots
```

These commands were used to create the laboratory directory, organize the required files, and verify the folder structure.

---

## 6.2 Editing and Viewing Files

The `nano` text editor was used to create and edit the Markdown documentation files.

```bash
nano README.md
nano infrastructure-report.md
nano cloud-components.md
nano cloud-provider-comparison.md
nano reflection.md
```

The `cat` command was used to view and verify the contents of the documentation files.

```bash
cat README.md
cat infrastructure-report.md
cat cloud-components.md
cat cloud-provider-comparison.md
cat reflection.md
```

---

## 6.3 Linux Server Investigation

The following commands were used to investigate the Linux cloud server:

```bash
lsb_release -a
```

Used to identify the Linux distribution and operating-system version.

```bash
uname -r
```

Used to identify the Linux kernel version.

```bash
lscpu | grep "Model name"
```

Used to identify the CPU model.

```bash
nproc
```

Used to determine the number of available CPU cores.

```bash
free -h
```

Used to investigate total and available memory.

```bash
df -h
```

Used to investigate disk capacity and mounted filesystems.

```bash
hostname
```

Used to identify the server hostname.

```bash
hostname -I
```

Used to identify the server IP addresses.

---

## 6.4 Git Commands

Git was used to manage the laboratory files and synchronize the completed work with GitHub.

```bash
git status

git add .

git commit -m "Complete Laboratory 2 cloud infrastructure blueprint"

git push
```

---

# 7. Cloud Infrastructure Relationship

The investigated infrastructure components work together as an integrated cloud environment.

```text
                         INTERNET
                            │
                            ▼
                    ┌───────────────┐
                    │    NETWORK    │
                    │ IP / Routing  │
                    └───────┬───────┘
                            │
                            ▼
                  ┌───────────────────┐
                  │      COMPUTE      │
                  │   Virtual CPU     │
                  │    1 CPU Core     │
                  └─────────┬─────────┘
                            │
                 ┌──────────┴──────────┐
                 ▼                     ▼
        ┌────────────────┐    ┌────────────────┐
        │    STORAGE     │    │  OPERATING     │
        │   /dev/vda1    │    │    SYSTEM      │
        │     19 GB      │    │ Ubuntu Linux   │
        └────────────────┘    └───────┬────────┘
                                      │
                                      ▼
                              ┌───────────────┐
                              │      IAM      │
                              │ Access Control│
                              └───────┬───────┘
                                      │
                                      ▼
                                    USERS
```

The architecture demonstrates how the major cloud infrastructure components work together.

**Networking** provides communication, **compute** provides processing power, **storage** provides persistent data storage, the **operating system** manages the server environment, and **identity and access management** controls access to resources.

Together, these components form the foundation required to operate cloud workloads.

---

# 8. Skills Learned

Through this laboratory activity, I learned how to inspect a Linux cloud environment and identify its basic infrastructure resources.

I practiced using Linux commands to obtain information about:

- Operating systems
- Kernel versions
- CPU resources
- Memory
- Storage
- Mounted filesystems
- Hostnames
- IP addresses

I also learned how compute, storage, networking, operating systems, and identity services work together to support cloud computing environments.

In addition, I learned how to compare equivalent services between **Amazon Web Services (AWS), Microsoft Azure, and Google Cloud Platform (GCP)**.

I gained experience creating a cloud infrastructure architecture diagram and organizing professional technical documentation using Markdown and GitHub.

---

# 9. Challenges Encountered

One challenge I encountered was understanding the different Linux commands required to obtain specific server information.

Some commands produced multiple values, so I needed to carefully identify which information represented the CPU, memory, storage, mounted filesystems, and network configuration.

Another challenge was understanding how the resources observed in the KillerCoda environment relate to real-world cloud infrastructure.

I also needed to carefully organize the required screenshots and Markdown files according to the laboratory folder structure.

Another challenge was comparing AWS, Microsoft Azure, and Google Cloud Platform because the three providers offer similar infrastructure capabilities but use different service names and implementations.

Researching and comparing these services helped me better understand how major cloud providers approach compute, storage, networking, and identity management.

---

# 10. Laboratory Deliverables

The completed laboratory folder is organized as follows:

```text
Laboratory-02-Build-the-Cloud-Infrastructure-Blueprint/
├── README.md
├── infrastructure-report.md
├── cloud-components.md
├── cloud-provider-comparison.md
├── reflection.md
└── screenshots/
    ├── server-information.png
    ├── network-information.png
    ├── storage-information.png
    └── cloud-architecture.png
```

## File Description

| File / Folder | Description |
|---|---|
| `README.md` | Contains the complete technical documentation and laboratory overview. |
| `infrastructure-report.md` | Contains the results of the Linux cloud server investigation. |
| `cloud-components.md` | Explains the compute, storage, networking, and operating system components identified in the Linux environment. |
| `cloud-provider-comparison.md` | Compares infrastructure services provided by AWS, Microsoft Azure, and Google Cloud Platform. |
| `reflection.md` | Contains the personal reflection and insights gained from the laboratory activity. |
| `screenshots/` | Contains screenshots captured as evidence during the investigation and documentation activities. |
| `server-information.png` | Screenshot showing the Linux server and system information. |
| `network-information.png` | Screenshot showing hostname and network/IP information. |
| `storage-information.png` | Screenshot showing disk capacity and filesystem information. |
| `cloud-architecture.png` | Cloud infrastructure architecture diagram showing how the major components work together. |

---

# 11. Conclusion

This laboratory provided practical experience in investigating and documenting cloud infrastructure using a Linux environment.

Through the KillerCoda Playground, I investigated the operating system, kernel version, CPU model, CPU cores, RAM, disk capacity, mounted filesystems, hostname, and IP addresses.

The activity demonstrated how **compute, storage, networking, operating systems, and identity management** work together to create a functional cloud environment.

It also strengthened my practical skills in:

- Linux
- Bash
- Cloud Computing
- Networking
- Git
- GitHub
- Technical Documentation
- Cloud Infrastructure Research

By completing this laboratory, I gained a better understanding of how cloud infrastructure is investigated, analyzed, documented, compared, and prepared before deployment.

> **Great cloud engineers build systems — exceptional cloud engineers document and justify every design decision.**

---

<div align="center">

### ☁️ CCM101 — Cloud Computing

**Laboratory 02: Build the Cloud Infrastructure Blueprint**

**Ashley B. Perado**

**University of Eastern Pangasinan**

</div>
