# ☁️ Mission 1 — Welcome to the Cloud

<p align="center">
  <img src="https://img.shields.io/badge/Platform-KillerCoda-blue?style=for-the-badge" alt="KillerCoda">
  <img src="https://img.shields.io/badge/OS-Ubuntu%2024.04-orange?style=for-the-badge&logo=ubuntu&logoColor=white" alt="Ubuntu">
  <img src="https://img.shields.io/badge/Linux-Kernel%206.8-green?style=for-the-badge&logo=linux&logoColor=white" alt="Linux">
  <img src="https://img.shields.io/badge/Architecture-x86__64-purple?style=for-the-badge" alt="Architecture">
</p>

<p align="center">
  <b>Cloud Computing & Linux Environment Investigation</b><br>
  <i>CCM 101 — Mission 1</i>
</p>

---

## 📌 Overview

This repository documents **Mission 1 — Welcome to the Cloud**, completed using the **KillerCoda Ubuntu Linux Playground**.

The objective of this mission was to explore a cloud-based Linux environment and identify its fundamental system resources, including:

* 🐧 Linux distribution
* ⚙️ Kernel version
* 🖥️ CPU information
* 🧠 Memory resources
* 💾 Disk capacity
* 🌐 Network configuration
* 🏷️ Hostname
* 💻 Linux command-line environment

This activity provides practical experience with Linux administration and cloud computing fundamentals.

---

# 🖥️ System Information

| Category                | Information                      |
| ----------------------- | -------------------------------- |
| 🐧 **Operating System** | Ubuntu 24.04.4 LTS               |
| 📦 **Release**          | 24.04                            |
| 🏷️ **Codename**        | Noble                            |
| ⚙️ **Kernel**           | 6.8.0-138-generic                |
| 🏗️ **Architecture**    | x86_64                           |
| 🖥️ **CPU**             | Intel Xeon E312xx (Sandy Bridge) |
| 🔢 **CPU Count**        | 1                                |
| 🚀 **CPU Speed**        | Approximately 2.0 GHz            |
| 🧠 **Total RAM**        | 1.9 GiB                          |
| ✅ **Available RAM**     | 1.4 GiB                          |
| 💾 **Total Disk**       | 19 GB                            |
| 📂 **Used Disk**        | 5.4 GB                           |
| 💿 **Available Disk**   | 13 GB                            |
| 📊 **Disk Usage**       | 30%                              |
| 🏷️ **Hostname**        | ubuntu                           |
| 🌐 **IP Address**       | 172.30.1.2 / 172.17.0.1          |

---

# 🔎 Environment Investigation

## 1. 🐧 Linux Distribution

The Linux distribution was identified using:

```bash
lsb_release -a
```

### Output

```text
Distributor ID: Ubuntu
Description:    Ubuntu 24.04.4 LTS
Release:        24.04
Codename:       noble
```

### Finding

The cloud environment is running **Ubuntu 24.04.4 LTS**, with the codename **Noble**.

---

## 2. ⚙️ Kernel Version

The Linux kernel was checked using:

```bash
uname -r
```

### Output

```text
6.8.0-138-generic
```

### Finding

The environment uses the **6.8.0-138-generic Linux kernel**.

---

## 3. 🖥️ CPU Information

CPU information was obtained using:

```bash
lscpu | grep "Model name"
```

### Output

```text
Model name: Intel Xeon E312xx (Sandy Bridge)
```

The system reports:

```text
CPU Count: 1
CPU Speed: Approximately 2.0 GHz
```

### Finding

The KillerCoda environment provides a virtualized **Intel Xeon E312xx processor**.

---

## 4. 🧠 Memory Information

Memory usage was checked using:

```bash
free -h
```

### Memory Status

| Resource   |  Amount |
| ---------- | ------: |
| Total      | 1.9 GiB |
| Used       | 424 MiB |
| Free       | 779 MiB |
| Available  | 1.4 GiB |
| Swap Total | 1.0 GiB |
| Swap Used  |     0 B |

### Finding

The environment has approximately **1.9 GiB of RAM**, with approximately **1.4 GiB available** during the investigation.

The system also has **1.0 GiB of swap space**, which was not being used at the time of checking.

---

## 5. 💾 Disk Space

Disk usage was checked using:

```bash
df -h
```

### Main Filesystem

```text
Filesystem      Size  Used Avail Use% Mounted on
/dev/vda1        19G  5.4G   13G  30% /
```

### Finding

The main filesystem provides approximately:

* **19 GB total storage**
* **5.4 GB used**
* **13 GB available**
* **30% utilization**

This indicates that the environment still has sufficient storage available for the activities in the playground.

---

## 6. 🏷️ Hostname

The hostname was checked using:

```bash
hostname
```

### Output

```text
ubuntu
```

### Finding

The hostname assigned to the Linux environment is:

**`ubuntu`**

---

## 7. 🌐 Network Information

The IP addresses were checked using:

```bash
hostname -I
```

### Output

```text
172.30.1.2 172.17.0.1
```

### Finding

The environment uses private IP addresses within its cloud/container networking environment.

| Interface Information | Address      |
| --------------------- | ------------ |
| Private IP            | `172.30.1.2` |
| Additional Private IP | `172.17.0.1` |

---

# 🧰 Commands Used

The following commands were used during the investigation:

```bash
# Check Linux distribution
lsb_release -a

# Check kernel version
uname -r

# Check CPU information
lscpu | grep "Model name"

# Check number of CPUs
nproc

# Check RAM and swap
free -h

# Check disk usage
df -h

# Check hostname
hostname

# Check IP addresses
hostname -I
```

---

# 📊 System Resource Summary

```text
┌──────────────────────────────────────────────┐
│              UBUNTU CLOUD ENVIRONMENT        │
├──────────────────────────────────────────────┤
│ OS           : Ubuntu 24.04.4 LTS            │
│ Kernel       : 6.8.0-138-generic             │
│ Architecture : x86_64                        │
│ CPU          : Intel Xeon E312xx             │
│ CPU Count    : 1                             │
│ RAM          : 1.9 GiB                       │
│ Available    : 1.4 GiB                       │
│ Storage      : 19 GB                         │
│ Available    : 13 GB                         │
│ Hostname     : ubuntu                        │
└──────────────────────────────────────────────┘
```

---

# 📁 Project Structure

The project workspace was created inside the Linux environment.

```text
CCM101-aperado/
│
├── 📄 README.md
│
├── 📄 system-information.md
│
└── 📁 Notes/
    │
    └── 📄 about-me.md
```

### File Descriptions

| File / Folder           | Purpose                                        |
| ----------------------- | ---------------------------------------------- |
| `README.md`             | Main project documentation                     |
| `system-information.md` | Linux environment investigation                |
| `Notes/`                | Workspace for notes                            |
| `about-me.md`           | Personal introduction and activity information |

---

# 📸 Evidence

The system information was collected directly from the **KillerCoda Ubuntu 24.04 Playground terminal**.

Recommended repository structure for evidence:

```text
CCM101-aperado/
│
├── README.md
│
├── system-information.md
│
├── Notes/
│   └── about-me.md
│
└── screenshots/
    └── system-information.png
```

> 💡 **Tip:** Save the screenshot of your KillerCoda terminal as `system-information.png` inside a `screenshots` folder. Then you can display it in this README.

Example:

```markdown
## 📸 Evidence

![Linux System Information](screenshots/system-information.png)
```

---

# 🎯 Learning Outcomes

After completing this activity, the following skills were practiced:

* ✅ Navigating a Linux cloud environment
* ✅ Using the Linux command line
* ✅ Identifying Linux distributions
* ✅ Checking kernel information
* ✅ Inspecting CPU resources
* ✅ Monitoring RAM and swap usage
* ✅ Checking disk capacity
* ✅ Identifying hostnames
* ✅ Checking network addresses
* ✅ Organizing project files in Linux
* ✅ Documenting cloud infrastructure information

---

# 🧠 Key Takeaways

This activity demonstrated how basic Linux commands can be used to quickly inspect a cloud computing environment.

The investigation showed that a cloud environment can provide a complete Linux operating system with virtualized CPU, memory, storage, and networking resources. These resources can be inspected and managed through the command line without requiring a graphical interface.

Understanding these commands is an important foundation for **Cloud Computing, Linux Administration, DevOps, Cybersecurity, and System Administration**.

---

# 🏁 Conclusion

Mission 1 successfully introduced the Linux cloud environment through the KillerCoda Ubuntu 24.04 Playground.

The investigation identified the operating system, kernel, CPU, memory, disk space, hostname, and network configuration. The activity also provided hands-on experience using essential Linux commands and organizing a project workspace.

This mission establishes the foundation for future cloud computing activities involving **Linux, infrastructure, networking, automation, and cloud services**.

---

<p align="center">

### ☁️ Cloud Computing • Linux • Infrastructure

**CCM 101 — Mission 1**

Made with 💻 and ☁️ by **Ashley B. Perado**

</p>
