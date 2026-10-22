# ☁️ MULTI-TIER ARCHITECTURE
### 🖥️ Cloud Deployment Engineering | Laboratory Guide

━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## 🔍 01 — Understanding Two-Tier Architecture

A **two-tier architecture** is a system divided into two main components: the application tier and the database tier. Each component has its own function, and they communicate with one another to make the application work properly.

In our laboratory activity, **Nextcloud** serves as the application, while **MariaDB** manages the database. Both components run in separate Docker containers and are managed using Docker Compose.

---

## 🌐 02 — Web / Application Tier

**Technology:** Nextcloud  
**Container:** `nextcloud-deployment_app_1`

The application tier provides the interface that users access through a web browser. It processes requests and allows users to interact with the application's features.

In our deployment, **Nextcloud** acts as the web application for managing files. Based on our screenshots, its container started successfully, and the Nextcloud setup page was accessible through the browser.

**Key responsibilities:**
- 🖥️ Provides the web interface.
- 📩 Receives and processes user requests.
- 📁 Allows users to manage files.
- 🔗 Communicates with the database when information is needed.

---

## 🗄️ 03 — Database Tier

**Technology:** MariaDB  
**Container:** `nextcloud-deployment_database_1`

The database tier stores and organizes the information required by the application. It allows the application to save, retrieve, and manage data.

In our activity, **MariaDB** serves as the database system. Its container was configured in the `docker-compose.yml` file and launched alongside the Nextcloud container.

**Key responsibilities:**
- 💾 Stores application data.
- 🔎 Handles data retrieval and database queries.
- 🛡️ Supports organized data management.
- 🔄 Works with Nextcloud to provide the required information.

---

## 🔗 04 — Why Separate the Two Tiers?

Separating the application and database into different containers makes the system easier to manage, maintain, and troubleshoot. Each container performs a specific role, allowing its configuration and operation to be handled independently.

Docker Compose simplifies this process by defining both services in one configuration file.

**Main advantages:**
- 🧩 **Organization** — Each service has a clear responsibility.
- 🛠️ **Maintainability** — Services can be configured and troubleshot separately.
- 📈 **Scalability** — Resources can be adjusted for individual services when needed.
- 🔁 **Reproducibility** — The same Compose configuration can be reused to deploy the application again.

---

## ⚙️ 05 — How the Components Communicate

The `docker-compose.yml` file defines the Nextcloud and MariaDB services. The application connects to the database through the environment variable:

`MYSQL_HOST=database`

The hostname `database` matches the MariaDB service name. Docker Compose provides service-name-based communication between containers on the same project network, so a manually entered database IP address is unnecessary.

---

## 🧱 06 — Architecture Diagram

```text
              👤 USER
                 │
                 ▼
          🌐 WEB BROWSER
                 │
                 ▼
    ┌──────────────────────────┐
    │   🌐 APPLICATION TIER    │
    │        Nextcloud         │
    │    Docker Container      │
    └──────────────────────────┘
                 │
          🔗 Database
           Connection
                 │
                 ▼
    ┌──────────────────────────┐
    │     🗄️ DATABASE TIER     │
    │         MariaDB          │
    │     Docker Container     │
    └──────────────────────────┘
                 ▲
                 │
         ⚙️ Docker Compose
        Manages Both Services
```

**Architecture flow:**

`👤 User → 🌐 Browser → Nextcloud → MariaDB`

---

## 📌 07 — Conclusion

This laboratory activity demonstrated how a two-tier architecture can be deployed using Docker Compose. Nextcloud provides the web interface, while MariaDB manages the database. Running these components in separate containers helps organize their responsibilities, while Docker Compose simplifies configuration, deployment, and cleanup.

Through this activity, I gained a better understanding of how application and database tiers work together in a containerized environment.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━

### ☁️ END OF LABORATORY GUIDE
