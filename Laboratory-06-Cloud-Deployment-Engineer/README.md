# ☁️ The Cloud Deployment Engineer

## 🎯 Mission Overview

Congratulations! Your flawless work in deploying data storage solutions has earned you a spot on the Cloud Deployment Team at CloudNova Technologies.

Up until now, you have been deploying single containers (like a standalone web server or a storage bucket). However, real-world enterprise applications are rarely just one container. They are "multi-tier" systems that require a frontend web application communicating seamlessly with a backend database. Deploying these one by one manually is prone to error.

Enter Docker Compose. In this mission, you will transition from manual commands to Infrastructure as Code (IaC). Using a YAML configuration file, you will define a multi-container private cloud storage application (Nextcloud and MariaDB) and deploy the entire stack simultaneously with a single command!

Remember: A junior engineer deploys servers by typing commands; a senior engineer deploys infrastructure by writing code.

## 🎯 Mission Objectives

At the end of this laboratory activity, you should be able to:

- Explain the concept of a multi-tier application architecture.
- Understand the purpose and structure of a `docker-compose.yml` file.
- Use a Linux command-line text editor (`nano`) to create configuration files.
- Deploy a multi-container application (Nextcloud + Database) using Docker Compose.
- Document deployment procedures and Infrastructure as Code (IaC) principles using Markdown.
- Continue expanding your professional GitHub Cloud Computing Portfolio.

## 💻 Commands Executed

| Command | Purpose |
|---|---|
| `docker-compose up -d` | Starts the Nextcloud and MariaDB containers in the background. |
| `docker-compose ps` | Displays the status of the containers. |
| `docker-compose down` | Stops and removes the project's containers and its default network. |

*Note: These are the deployment, status-checking, and teardown commands discussed from your screenshots. Add other commands only if they appear in your terminal history or screenshots.*

## 🏗️ Multi-Tier Architecture

The application consists of two main services that work together:

- 🌐 **Application Tier — Nextcloud:** Provides the web interface that users can access through a browser.
- 🗄️ **Database Tier — MariaDB:** Stores database information needed by the Nextcloud application.

Docker Compose allows these services to run together and communicate over the project's network. Nextcloud can identify the database through its Compose service name, configured using the `MYSQL_HOST` environment variable.

## ⚙️ Infrastructure as Code (IaC)

Infrastructure as Code involves defining infrastructure and service configurations in files rather than relying entirely on manual commands. In this activity, the `docker-compose.yml` file describes the services and their configuration.

This approach makes deployment more repeatable, organized, and easier to maintain. Instead of starting each container separately, Docker Compose can manage the services together.

## 🔐 Environment Variables

Environment variables provide configuration values required by the containers.

- `MYSQL_PASSWORD` — Specifies the database user's password.
- `MYSQL_HOST` — Identifies the database service that Nextcloud connects to.

These variables help organize configuration and enable communication between the application and database. Passwords should be protected and not exposed in public repositories.

## 🧠 Skills Learned

- 🐳 Using Docker Compose to manage multiple containers.
- 🏗️ Understanding multi-tier application architecture.
- 📝 Understanding YAML configuration and indentation.
- ⚙️ Configuring services using environment variables.
- 🌐 Accessing the Nextcloud setup page through a browser.
- 🔍 Checking container status and managing the deployment lifecycle.
- 📚 Documenting cloud computing activities using Markdown.

## 🚀 Mission Accomplished

This laboratory activity helped me understand how Docker Compose simplifies the deployment of applications that require multiple services. I started the Nextcloud and MariaDB containers, checked their status, and accessed the Nextcloud setup page through a browser.

Through this experience, I gained a better understanding of containerization, service communication, and Infrastructure as Code. I also learned how automation makes cloud deployment more organized and efficient.
