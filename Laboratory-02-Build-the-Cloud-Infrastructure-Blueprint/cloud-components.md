# ☁️ Laboratory 02 — Cloud Infrastructure Components

## Checkpoint 3 — Identify Cloud Infrastructure Components

### 📌 Overview

Checkpoint 3 identifies the cloud infrastructure components observed in the **KillerCoda Ubuntu 24.04 Linux environment**.

The components are grouped into four major categories:

1. ⚙️ Compute Resources
2. 💾 Storage Resources
3. 🌐 Networking Resources
4. 🐧 Operating System

Each component is explained based on its purpose, importance in cloud computing, and relationship to the KillerCoda Linux environment.

---

# ⚙️ 1. Compute Resources

## Example: Intel Xeon CPU

The KillerCoda environment provides an **Intel Xeon E312xx (Sandy Bridge)** processor with **1 CPU core**.

### Purpose

The CPU performs the calculations and processing required by applications and operating-system processes.

It executes instructions and allows the Linux environment to run commands, applications, and services.

### Importance in Cloud Computing

Compute resources are one of the fundamental components of cloud computing.

Cloud providers allocate virtualized CPU resources to users depending on the requirements of their applications.

The amount of compute resources affects:

* Application performance
* Processing speed
* Number of simultaneous tasks
* Scalability
* Overall system capacity

### Relation to KillerCoda

The KillerCoda playground provides a virtualized CPU resource to the Ubuntu environment.

The investigation showed:

```text
CPU Model: Intel Xeon E312xx (Sandy Bridge)
CPU Cores: 1
```

This demonstrates how cloud environments can provide users with allocated computing resources without requiring them to own or physically manage the underlying hardware.

---

# 💾 2. Storage Resources

## Example: `/dev/vda1`

The primary storage device observed in the environment is:

```text
/dev/vda1
```

It provides approximately **19 GB of storage**, with around **13 GB available**.

### Purpose

Storage resources are used to permanently store:

* Operating-system files
* Applications
* Configuration files
* User files
* Project files
* Logs
* Other data

### Importance in Cloud Computing

Cloud storage allows organizations and applications to store large amounts of information without maintaining physical storage infrastructure themselves.

Cloud storage can also provide:

* Scalability
* Reliability
* Backup capabilities
* Accessibility
* Data persistence

### Relation to KillerCoda

The KillerCoda Linux environment uses `/dev/vda1` as its primary filesystem.

The investigation showed:

```text
Size:       19G
Used:       5.4G
Available:  13G
Usage:      30%
Mounted on: /
```

This represents the storage resource allocated to the cloud server.

---

# 🌐 3. Networking Resources

## Example: Private IP Addresses

The KillerCoda environment provides the following IP addresses:

```text
172.30.1.2
172.17.0.1
```

### Purpose

Networking resources allow computers, applications, and cloud services to communicate with one another.

IP addresses provide an identity that allows network traffic to be directed to the appropriate system or service.

### Importance in Cloud Computing

Networking is essential because cloud applications depend on communication between:

* Users
* Servers
* Databases
* Storage services
* APIs
* Other cloud resources

Cloud networking also enables:

* Internet connectivity
* Private communication
* Network segmentation
* Security controls
* Service-to-service communication

### Relation to KillerCoda

The KillerCoda environment uses private IP addresses within its cloud/container networking environment.

The addresses observed were:

```text
172.30.1.2
172.17.0.1
```

These addresses demonstrate that the Linux environment operates within a virtualized network rather than directly using a public Internet address.

---

# 🐧 4. Operating System

## Example: Ubuntu 24.04.4 LTS

The cloud server is running:

```text
Ubuntu 24.04.4 LTS
```

with:

```text
Kernel: 6.8.0-138-generic
Architecture: x86_64
```

### Purpose

The operating system manages the computer's hardware and provides the environment required to run applications and services.

Linux handles:

* CPU processes
* Memory
* Storage
* Networking
* Users
* Permissions
* System services

### Importance in Cloud Computing

Operating systems provide the foundation for cloud servers and virtual machines.

Linux is widely used in cloud computing because it is:

* Flexible
* Reliable
* Lightweight
* Highly configurable
* Well supported
* Suitable for server environments

### Relation to KillerCoda

KillerCoda provides an Ubuntu Linux environment that can be accessed through the terminal.

The environment allows users to execute Linux commands and investigate the virtual server's resources.

The observed operating system was:

```text
Ubuntu 24.04.4 LTS
```

---

# 📊 5. Cloud Infrastructure Summary

| Component           | Example in KillerCoda      | Purpose                                 |
| ------------------- | -------------------------- | --------------------------------------- |
| ⚙️ Compute          | Intel Xeon CPU, 1 core     | Processes instructions and applications |
| 💾 Storage          | `/dev/vda1`, 19 GB         | Stores system and user data             |
| 🌐 Networking       | `172.30.1.2`, `172.17.0.1` | Enables network communication           |
| 🐧 Operating System | Ubuntu 24.04.4 LTS         | Manages resources and runs applications |

---

# 🔗 6. How the Components Work Together

The components work together to create a functional cloud server:

```text
                  ☁️ CLOUD SERVER
                        │
          ┌─────────────┼─────────────┐
          │             │             │
          ▼             ▼             ▼
      ⚙️ COMPUTE     💾 STORAGE    🌐 NETWORK
      Intel Xeon      /dev/vda1     IP Address
       1 Core          19 GB       172.30.1.2
          │             │             │
          └─────────────┼─────────────┘
                        ▼
                 🐧 UBUNTU LINUX
                 24.04.4 LTS
                        │
                        ▼
                  👨‍💻 USER
```

The operating system manages the compute, storage, and networking resources and provides an environment where users can execute applications and commands.

---

# 🧠 7. Key Learning

The KillerCoda environment demonstrates that a cloud server is made up of multiple interconnected infrastructure components.

The **CPU provides computing power**, **storage provides persistent data capacity**, **networking enables communication**, and the **operating system manages these resources**.

Together, these components form the foundation of a cloud computing environment.

---

# 🏁 Conclusion

The investigation of the KillerCoda environment provided a practical example of fundamental cloud infrastructure components.

The **Intel Xeon CPU** represents the compute resource, `/dev/vda1` represents the primary storage resource, the private IP addresses represent networking resources, and **Ubuntu 24.04.4 LTS** represents the operating system.

Understanding these components is important because they form the foundation of modern cloud infrastructure. By learning how these resources work together, cloud computing students can better understand how virtual machines, cloud servers, and other cloud services operate.
