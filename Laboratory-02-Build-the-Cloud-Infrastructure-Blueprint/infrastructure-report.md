# ☁️ Laboratory 02 — Build the Cloud Infrastructure Blueprint

## Checkpoint 2 — Investigate the Cloud Server

### 📌 Overview

For Checkpoint 2, the Linux environment provided by the **KillerCoda Ubuntu 24.04 Playground** was investigated using terminal commands.

The purpose of this investigation was to identify the cloud server's operating system, kernel, CPU, memory, storage, mounted file systems, hostname, and IP address.

---

## 🖥️ 1. Operating System

### Command Used

```bash
lsb_release -a
```

### Result

```text
Distributor ID: Ubuntu
Description:    Ubuntu 24.04.4 LTS
Release:        24.04
Codename:       noble
```

### Finding

The cloud server is running **Ubuntu 24.04.4 LTS**, with the codename **Noble**.

Ubuntu is a Linux-based operating system commonly used for servers, cloud computing, development, and system administration.

---

## ⚙️ 2. Kernel Version

### Command Used

```bash
uname -r
```

### Result

```text
6.8.0-138-generic
```

### Finding

The Linux environment is running kernel version:

**`6.8.0-138-generic`**

The kernel is the core component of the Linux operating system responsible for managing hardware, memory, processes, and system resources.

---

## 🖥️ 3. CPU Model

### Command Used

```bash
lscpu | grep "Model name"
```

### Result

```text
Model name: Intel Xeon E312xx (Sandy Bridge), IBRS update
```

### Finding

The cloud server uses an **Intel Xeon E312xx (Sandy Bridge)** processor.

The CPU is a virtualized cloud-server resource provided by the KillerCoda environment.

---

## 🔢 4. Number of CPU Cores

### Command Used

```bash
nproc
```

### Result

```text
1
```

### Finding

The KillerCoda cloud server provides **1 CPU core** to the Linux environment.

The number of CPU cores determines how many processing tasks can be handled concurrently by the system.

---

## 🧠 5. Total RAM

### Command Used

```bash
free -h
```

### Result

```text
              total        used        free      shared  buff/cache   available
Mem:           1.9Gi       424Mi       779Mi       1.1Mi       870Mi       1.4Gi
Swap:          1.0Gi          0B       1.0Gi
```

### Finding

The cloud server has:

* **Total RAM:** 1.9 GiB
* **Used RAM:** 424 MiB
* **Free RAM:** 779 MiB
* **Available RAM:** 1.4 GiB
* **Total Swap:** 1.0 GiB
* **Used Swap:** 0 B

The available memory was sufficient for performing the laboratory activities.

---

## 💾 6. Disk Capacity

### Command Used

```bash
df -h
```

### Main Disk Result

```text
Filesystem      Size  Used Avail Use% Mounted on
/dev/vda1        19G  5.4G   13G  30% /
```

### Finding

The primary disk has:

* **Capacity:** 19 GB
* **Used:** 5.4 GB
* **Available:** 13 GB
* **Usage:** 30%
* **Mounted at:** `/`

The Linux environment therefore has approximately **19 GB of total disk capacity**.

---

## 📂 7. Mounted File Systems

### Command Used

```bash
df -h
```

### Result

The following mounted file systems were observed:

| File System  | Size | Used | Available | Usage | Mount Point |
| ------------ | ---: | ---: | --------: | ----: | ----------- |
| `/dev/vda1`  |  19G | 5.4G |       13G |   30% | `/`         |
| `tmpfs`      | 191M | 996K |      190M |    1% | `/run`      |
| `/dev/vda1`  |  19G | 5.4G |       13G |   30% | `/`         |
| `tmpfs`      | 952M |  84K |      952M |    1% | `/dev/shm`  |
| `tmpfs`      | 5.0M |   0B |      5.0M |    0% | `/run/lock` |
| `/dev/vda16` | 881M | 117M |      703M |   15% | `/boot`     |
| `/dev/vda15` | 105M | 6.2M |       99M |    6% | `/boot/efi` |

### Finding

The environment contains a primary Linux filesystem mounted at `/`, along with temporary filesystems and separate boot partitions.

The main filesystem is `/dev/vda1`, while `/boot` and `/boot/efi` are mounted separately for boot-related system files.

---

## 🏷️ 8. Hostname

### Command Used

```bash
hostname
```

### Result

```text
ubuntu
```

### Finding

The hostname of the cloud server is:

**`ubuntu`**

The hostname identifies the Linux system within its environment.

---

## 🌐 9. IP Address

### Command Used

```bash
hostname -I
```

### Result

```text
172.30.1.2 172.17.0.1
```

### Finding

The Linux environment has the following IP addresses:

* **172.30.1.2**
* **172.17.0.1**

These are private IP addresses used within the KillerCoda cloud/container networking environment.

---

# 📊 10. Complete Investigation Summary

| Requirement         | Result                                        |
| ------------------- | --------------------------------------------- |
| 🐧 Operating System | Ubuntu 24.04.4 LTS                            |
| ⚙️ Kernel Version   | 6.8.0-138-generic                             |
| 🖥️ CPU Model       | Intel Xeon E312xx (Sandy Bridge), IBRS update |
| 🔢 CPU Cores        | 1                                             |
| 🧠 Total RAM        | 1.9 GiB                                       |
| 💾 Disk Capacity    | 19 GB                                         |
| 📂 Main Filesystem  | `/dev/vda1` mounted on `/`                    |
| 🏷️ Hostname        | ubuntu                                        |
| 🌐 IP Address       | 172.30.1.2 / 172.17.0.1                       |

---

# 🧰 11. Commands Used

The following commands were used to investigate the cloud server:

```bash
lsb_release -a
uname -r
lscpu | grep "Model name"
nproc
free -h
df -h
hostname
hostname -I
```

Each command was used to retrieve a specific part of the Linux environment's configuration.

---

# 📸 12. Investigation Evidence

Screenshots of the KillerCoda terminal investigation are stored in the `screenshots` directory.

Recommended structure:

```text
Laboratory-02-Build-the-Cloud-Infrastructure-Blueprint/
│
└── screenshots/
    └── system-investigation.png
```

The screenshot provides visual evidence of the commands and system information collected during the investigation.

### Evidence

![KillerCoda Linux System Investigation](screenshots/system-investigation.png)

---

# 🏁 13. Conclusion

The investigation successfully identified the main characteristics of the Linux cloud server provided by KillerCoda.

The environment is running **Ubuntu 24.04.4 LTS** with the **6.8.0-138-generic kernel**. It provides **one CPU core**, **1.9 GiB of RAM**, and a **19 GB primary disk**. The server's hostname is `ubuntu`, and the environment uses private IP addresses `172.30.1.2` and `172.17.0.1`.

The investigation also identified the mounted file systems, including the main root filesystem, temporary filesystems, `/boot`, and `/boot/efi`.

This checkpoint provided practical experience in using Linux commands to inspect the resources and configuration of a cloud-based server environment.
