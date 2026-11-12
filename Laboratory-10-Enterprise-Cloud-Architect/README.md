# ☁️ Mission 10: Enterprise Cloud Architect

**CCM101 – Cloud Computing | CloudNova Infrastructure Project**

---

## 📌 Project Overview

**CloudNova** is a cloud infrastructure project developed for CCM101 – Cloud Computing. It demonstrates how to build, manage, and secure a web application using a virtual machine and Docker.

The project uses Ubuntu Server to run two connected services: WordPress and MariaDB. WordPress handles the website, while MariaDB stores its data.

The system also includes firewall protection, secure remote access, permanent data storage, and automatic database backups.

## 🎯 Project Objectives

- Set up a Linux server using Oracle VirtualBox.
- Configure network connections between the laptop and the virtual machine.
- Install Docker and Docker Compose.
- Deploy WordPress and MariaDB as connected services.
- Set up storage to keep application and database data safe.
- Protect the server using firewall rules and secure SSH access.
- Create a Bash script for automatic database backups.
- Schedule backups using Cron.
- Document the setup and maintenance procedures.

---

## 🏛️ Infrastructure Design and Architecture

The CloudNova infrastructure follows a virtualized and container-based approach, allowing the website, database, security controls, and automated operations to function within one organized environment.

The architecture consists of the following components:

1. **Windows Host Computer:** A Windows 11 laptop serves as the primary workstation for managing the virtual infrastructure and accessing the deployed website.

2. **Oracle VirtualBox:** Provides the virtualization environment required to operate Ubuntu Server independently from the host operating system.

3. **Ubuntu Server:** Functions as the central server where Docker Engine, Docker Compose, and the necessary system services are installed.

4. **Network Connectivity:** Two network configurations are utilized. NAT enables the Ubuntu Server to access the internet, while the Host-only adapter establishes communication between the Windows laptop and the virtual machine.

5. **Network Security:** UFW and Docker-related firewall rules are configured to regulate incoming connections and reduce unnecessary network exposure.

6. **Docker Environment:** Handles the deployment, operation, and management of the application and database containers.

7. **WordPress Service:** Serves as the web application that users can access through a browser.

8. **MariaDB Service:** Manages and stores the information required by WordPress.

9. **Persistent Storage:** Docker volumes maintain application files and database records independently of container restarts or recreation.

10. **Automated Operations:** Bash scripting and Cron scheduling support routine database backups without requiring manual execution each day.

The complete infrastructure layout is illustrated in the [Architecture Diagram](architecture-diagram.png).

---

## 🛠️ Development Tools and Technologies

The project integrates several tools and technologies to support virtualization, container management, system administration, security, and automated maintenance.

| Infrastructure Component | Technology / Version |
|---|---|
| Host Operating System | Windows 11 |
| Virtualization Platform | Oracle VirtualBox |
| Guest Operating System | Ubuntu Server 26.04.1 LTS |
| Containerization Engine | Docker Engine 29.9.2 |
| Container Orchestration | Docker Compose 5.6.1 |
| Web Application | WordPress |
| Database Management System | MariaDB 11.4 |
| Security Management | UFW and iptables |
| Task Automation | Bash and Cron |
| Remote Server Administration | OpenSSH |
| Authentication Method | ED25519 SSH Key |

Each technology has a specific responsibility within the system, contributing to the overall operation, accessibility, and maintenance of the deployed infrastructure.

---

## 🌐 Network Setup and Connectivity

CloudNova utilizes a dual-network configuration to separate internet connectivity from local communication between the host computer and the virtual server.

| Network Component | Assigned Address | Function |
|---|---|---|
| NAT Interface (`enp0s3`) | `10.0.2.15/24` | Enables internet connectivity for the Ubuntu virtual machine |
| Host-only Interface (`enp0s8`) | `192.168.56.103/24` | Provides a private connection between the host and virtual server |
| Windows Host-only Adapter | `192.168.56.1` | Allows the Windows workstation to communicate with Ubuntu Server |
| WordPress Web Service | `192.168.56.103:8080` | Provides browser access to the deployed website |

### 🌍 Website Access

The WordPress application is accessible from the Windows host through the following address:

`http://192.168.56.103:8080`

This configuration allows the website to be accessed through the Host-only network while maintaining a separate interface for the server's internet connection.

---

## 🐳 Container Deployment and Service Integration

CloudNova uses Docker Compose to deploy and coordinate two interconnected containers.

| Container Name | Docker Image | Responsibility |
|---|---|---|
| `cloudnova-wordpress` | `wordpress:latest` | Hosts the WordPress website and application components |
| `cloudnova-database` | `mariadb:11.4` | Manages the database used by WordPress |

Both services are connected through the dedicated Docker network named `cloudnova-network`.

This arrangement allows WordPress to communicate with MariaDB internally without requiring the database service to be publicly accessible.

### 💾 Persistent Data Management

Two Docker volumes are used to retain important application information:

- **`wordpress_data`** — preserves WordPress application files and uploaded content.
- **`mariadb_data`** — maintains the database files and records used by the website.

Using persistent volumes ensures that stored information remains available even if the containers are restarted or recreated.

For additional protection, the MariaDB database port is not published directly to the host network.

---

## 🔒 Server Protection and Access Security

Security configurations were incorporated into the CloudNova infrastructure to control access to the server and its deployed services.

The implemented security measures include:

- **Default-Deny Firewall Policy:** UFW is activated with incoming connections blocked by default.
- **Outbound Network Access:** Outgoing traffic is permitted to support necessary server operations.
- **Restricted SSH Connectivity:** Remote administration is limited to the Host-only network.
- **Password Authentication Disabled:** SSH password-based login is turned off to reduce unauthorized login attempts.
- **Root SSH Login Disabled:** Direct remote login using the root account is prohibited.
- **SSH Key Authentication:** Public-key authentication is enabled using an ED25519 key.
- **Docker Network Restrictions:** Additional firewall rules limit website access to the Windows host.
- **Database Isolation:** MariaDB communicates exclusively through the internal Docker network.
- **Credential Protection:** Database passwords are maintained in a protected `.env` file rather than being committed to the public GitHub repository.

These configurations provide multiple layers of protection while allowing authorized users to administer and access the application.

---

## ⚙️ Automated Database Backup System

To support data recovery and routine maintenance, CloudNova includes a Bash-based backup mechanism that operates through scheduled execution.

### Backup Configuration

| Setting | Configuration |
|---|---|
| Script Filename | `automation-script.sh` |
| Backup Directory | `/opt/cloudnova/backups/` |
| Scheduling Tool | Cron |
| Execution Frequency | Daily |
| Scheduled Time (UTC) | 2:00 AM |
| Philippine Time | 10:00 AM |
| Backup Retention | 7 days |

### Backup Process

When executed, the automation script carries out the following operations:

1. **Database Export:** Produces a backup copy of the MariaDB database.
2. **File Compression:** Uses Gzip to reduce the size of the generated backup.
3. **Timestamp Assignment:** Includes the date and time in each filename for easier identification.
4. **Backup Validation:** Checks the generated backup file to determine whether it meets the script's validity checks.
5. **Retention Management:** Automatically removes backup files older than seven days.
6. **Activity Logging:** Records the result of each backup operation for monitoring and troubleshooting.

With Cron managing the execution schedule, database backups can be performed regularly without the need to manually run the script every day.

---

## 📂 Repository Organization

All important deployment configurations, scripts, diagrams, and documentation are maintained within the Mission 10 directory of the CCM101 GitHub portfolio.

```text
Laboratory-10-Enterprise-Cloud-Architect/
│
├── README.md
├── architecture-diagram.png
├── docker-compose.yml
├── automation-script.sh
├── operational-manual.md
└── final-reflection.md
```

This arrangement provides a clear reference for reviewing the infrastructure and understanding the purpose of each project file.

---

## 🚀 Application Deployment and Management

The following commands are used for basic administration of the CloudNova environment.

### 1. Navigate to the Project Directory

Open the Ubuntu Server terminal and access the directory containing the deployment files.

```bash
cd /opt/cloudnova
```

### 2. Launch the Docker Services

Start the application containers in detached mode.

```bash
sudo docker compose up -d
```

### 3. Verify Container Operation

Display the running Docker containers to confirm that the services are active.

```bash
sudo docker ps
```

### 4. Inspect Application Logs

Review the container logs to identify system events, service messages, and possible errors.

```bash
sudo docker compose logs
```

### 5. Access the WordPress Website

From the Windows host computer, open a web browser and enter:

```text
http://192.168.56.103:8080
```

If the required services are operating correctly and network access is permitted, the deployed WordPress website should become accessible through this address.

For detailed procedures involving installation, server security, backup management, and troubleshooting, refer to the [Operational Manual](operational-manual.md).

---

## 📦 Required Project Files and Deliverables

The Mission 10 submission contains the essential files necessary to present and document the infrastructure.

| File | Description |
|---|---|
| `README.md` | Introduces CloudNova and summarizes its architecture, technologies, security, and deployment process |
| `architecture-diagram.png` | Illustrates the network topology, virtual machine, containers, and infrastructure components |
| `docker-compose.yml` | Defines the WordPress and MariaDB services and their required configurations |
| `automation-script.sh` | Contains the Bash commands responsible for scheduled database backups |
| `operational-manual.md` | Provides documentation covering server deployment, maintenance, security, and recovery procedures |
| `final-reflection.md` | Presents the knowledge, experiences, and lessons gained throughout CCM101 |

Together, these resources serve as both the project's technical documentation and a reference for its ongoing operation.

---

## 📝 Project Conclusion

The CloudNova project brings together essential cloud computing and system administration concepts within a single virtualized infrastructure.

Through the integration of Ubuntu Server, Docker, WordPress, and MariaDB, the project demonstrates how containerized applications and databases can operate together while maintaining persistent storage.

Its network configuration, security controls, and scheduled backup process further emphasize the importance of protecting system resources and maintaining application data.

Overall, CloudNova represents a practical application of the knowledge developed throughout CCM101. It highlights how proper infrastructure planning, container deployment, access management, and automation contribute to creating a manageable and functional server environment.

---

**☁️ CloudNova | CCM101 – Cloud Computing | Mission 10: Enterprise Cloud Architect**
