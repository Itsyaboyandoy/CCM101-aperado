# 🐳 DOCKER COMPOSE GUIDE
### Laboratory Activity — Cloud Deployment Engineering

---

## 🎯 LABORATORY OVERVIEW

In this activity, we used Docker Compose to deploy Nextcloud and MariaDB in separate containers. We configured the services, checked their status, accessed the Nextcloud web interface, and practiced stopping the deployment.

---

## 01 | UNDERSTANDING SERVICES

**Question:** What does the `services:` block do?

**Answer**

The `services:` block defines the containers required to run an application. In our activity, it contains two services:

- **`app`** — runs Nextcloud, which provides the web interface for managing files.
- **`database`** — runs MariaDB, which stores the application's data.

Both services are configured in the `docker-compose.yml` file, allowing them to be managed together instead of setting up each container separately.

---

## 02 | CONNECTING TO THE DATABASE

**Question:** How did the Nextcloud app container know how to find the database container?

**Answer**

Nextcloud finds the MariaDB container through the `MYSQL_HOST=database` environment variable in the Compose file. The word `database` matches the name of the database service.

Docker Compose allows containers in the same project network to communicate using their service names. This means Nextcloud can connect to MariaDB without manually entering the database container's IP address.

---

## 03 | COMPARING DOCKER COMMANDS

**Question:** What is the difference between `docker run` and `docker-compose up -d`?

**Answer**

The `docker run` command starts an individual container using settings provided in the command line. When an application requires multiple containers, each container may need to be configured and started separately.

In contrast, `docker-compose up -d` reads the `docker-compose.yml` file and starts the services defined in it in the background. In our activity, this command launched both Nextcloud and MariaDB using the same configuration file, making deployment easier to repeat and manage.

---

## 📸 LABORATORY RESULTS

The following results were observed during the activity:

1. **Configuration:** Created the `docker-compose.yml` file with the Nextcloud and MariaDB services.
2. **Deployment:** Successfully started both containers using Docker Compose.
3. **Verification:** Used `docker-compose ps` to check that both containers were running.
4. **Web access:** Opened the Nextcloud setup page through the browser.
5. **Cleanup:** Ran `docker-compose down` to stop and remove the containers and the default project network.

---

## 📌 SUMMARY

Docker Compose makes it easier to deploy and manage applications that require multiple containers. Through this activity, I learned how to define services in a single configuration file, connect an application to its database using service names, verify running containers, access a web application, and clean up a deployment.

This activity helped me understand how containerized applications work together and how Docker Compose simplifies the deployment process.

---

**END OF LABORATORY GUIDE**
