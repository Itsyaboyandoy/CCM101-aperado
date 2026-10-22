# ☁️ The Cloud Operations Engineer

## 🎯 Mission Overview

Congratulations! Your ability to deploy multi-tier architectures has proven your technical capabilities.  
You have now been promoted to the **Cloud Operations Team** (often referred to in the industry as Site Reliability Engineering, or SRE) at CloudNova Technologies.  
Deploying a cloud application is only the first step; keeping it running smoothly is the real challenge.  
When a server crashes or a web page takes ten seconds to load, you cannot simply guess what is wrong. You must rely on **Observability and Monitoring** to see inside your infrastructure.  
Using the KillerCoda Playground, you will step into the role of a Cloud Operations Engineer. You will establish a performance baseline for your Linux server, deploy a containerized application, generate artificial web traffic, and hunt down performance metrics and system logs to prove the application is healthy.  
Remember: **A developer hopes the application works; a Site Reliability Engineer uses metrics and logs to prove it.**

## 🎯 Mission Objectives

At the end of this laboratory activity, you should be able to:

- Utilize native Linux command-line tools to monitor host CPU, Memory, and Disk capacity.
- Deploy a web container and track its real-time performance using Docker metrics.
- Generate web traffic and extract application access logs for analysis.
- Translate raw performance data into a readable technical report using Markdown.
- Continue expanding a professional GitHub Cloud Computing Portfolio.

## 🛠️ Monitoring Commands Executed

| **Command** | **Purpose** |
|---|---|
| `top` | Displays running processes, CPU usage, memory usage, and system activity. |
| `free -h` | Checks the server's total, used, and available RAM. |
| `df -h` | Displays filesystem disk capacity, used space, and available storage. |
| `docker run -d -p 8080:80 --name client-website nginx` | Downloads the Nginx image if needed and starts a website container in the background with port 8080 mapped to port 80. |
| `docker ps` | Checks the running container and its published ports. |
| `curl http://localhost:8080` | Sends HTTP requests to the Nginx website and retrieves its default HTML page. |
| `curl http://localhost:8080/hidden-admin-page` | Requests a nonexistent page to generate and investigate a 404 Not Found response. |
| `docker logs client-website` | Displays the Nginx container logs, including HTTP requests and the missing-page error. |
| `docker stats` | Displays live resource usage, including CPU and memory consumption, for running containers. |

## 📊 System Monitoring and Performance

During the activity, I used Linux monitoring tools to examine the server's resource usage. The `top` command displayed active processes and system activity, while `free -h` showed memory information and `df -h` displayed disk capacity.

These commands helped establish a basic understanding of the server's available resources before analyzing the containerized application.

## 🐳 Container Deployment

I deployed an Nginx web server using Docker and assigned it the container name `client-website`. Port `8080` on the host was mapped to port `80` inside the container, allowing me to send requests to the website through `localhost:8080`.

The `docker ps` output confirmed that the container was running and that the port mapping was active.

## 🔎 Web Traffic and Log Analysis

I used `curl` to access the default Nginx page repeatedly and confirmed that the server returned its HTML response. I then requested `/hidden-admin-page`, which returned a **404 Not Found** response because the requested resource did not exist.

Using `docker logs client-website`, I examined the server logs and identified successful HTTP requests and the failed request. This demonstrated how logs can help an engineer investigate application behavior and diagnose errors.

## 📈 Container Resource Monitoring

The `docker stats` command provided information about the container's CPU usage, memory consumption, network activity, and other resource metrics.

Monitoring these values helps cloud operations engineers understand how a container uses system resources and identify potential performance issues.

## 💡 Skills Learned

- Monitoring Linux processes and CPU activity using `top`.
- Checking RAM usage with `free -h`.
- Checking disk capacity using `df -h`.
- Deploying and managing an Nginx container using Docker.
- Understanding container port mapping between host port `8080` and container port `80`.
- Generating HTTP requests using `curl`.
- Identifying a 404 Not Found response from a nonexistent page.
- Analyzing web server access and error information using `docker logs`.
- Monitoring container resource consumption using `docker stats`.
- Documenting cloud operations activities using Markdown and GitHub.

## 🚀 Mission Accomplished

This laboratory activity helped me understand that deploying an application is only one part of cloud operations. Monitoring system resources, checking container status, generating test traffic, and reviewing logs are also important for evaluating application behavior.

By deploying Nginx, testing its response with `curl`, investigating a 404 error, and checking resource usage, I gained practical experience with basic observability and troubleshooting. These skills will help me understand how cloud operations engineers monitor applications and investigate issues in real-world environments.
