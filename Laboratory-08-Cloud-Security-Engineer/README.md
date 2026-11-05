## 🎯 Mission Overview

Congratulations! Your proactive approach to system monitoring has earned you a spot on the elite  
**Cloud Security Team** at CloudNova Technologies.  
In the cloud, leaving a server unsecured for even a few minutes can lead to automated brute-force  
attacks and data breaches. Your mission today applies the security concepts you learned in Chapter 8. You will  
implement the principle of defense in depth by locking down a live server using a host-based firewall.  
Using the KillerCoda Playground, you will step into the role of a Cloud Security Engineer. You will  
deploy a web application, audit the server's open ports, and configure the Uncomplicated Firewall (UFW) to block  
malicious traffic while allowing legitimate users to access the application.  
Remember: **Security is not a product you buy; it is a continuous process you maintain.**

## 📌 Objectives

At the end of this laboratory activity, you should be able to:

- Understand the concept of the Attack Surface and the Principle of Least Privilege (PoLP).
- Perform a basic security audit of active network ports on a Linux server.
- Configure the Uncomplicated Firewall (UFW) with a Default Deny policy.
- Implement granular port management to selectively allow SSH and HTTP traffic.
- Document firewall rules and security best practices using Markdown.
- Continue expanding your professional GitHub Cloud Computing Portfolio.

## 💻 Commands Executed

| Command | What This Command Does |
|---|---|
| `sudo ufw allow ssh` | Allows SSH connections so administrators can remotely access and manage the server. |
| `sudo ufw default deny incoming` | Blocks incoming connections unless they are specifically allowed by a firewall rule. |
| `sudo ufw default allow outgoing` | Allows outgoing connections from the server by default. |
| `sudo ufw enable` | Activates UFW and applies the configured firewall rules. |
| `sudo ufw allow 8080/tcp` | Allows incoming TCP connections through port 8080 for accessing the Nginx web application. |
| `sudo ufw status verbose` | Displays the firewall status, default policies, and other configuration details. |
| `sudo ufw status numbered` | Displays firewall rules with assigned numbers for easier identification and management. |
| `docker run -d -p 8080:80 --name secure-web-app nginx` | Creates and runs an Nginx container named `secure-web-app` in detached mode, mapping host port 8080 to container port 80. |
| `docker ps` | Displays currently running Docker containers and their port mappings. |
| `curl http://localhost:8080` | Sends an HTTP request to the local Nginx application to verify that it is responding correctly. |
| `git clone https://github.com/Itsyaboyandoy/CCM101-aperado.git` | Downloads the GitHub repository containing the Cloud Computing laboratory activities. |
| `git config --global user.name "Itsyaboyandoy"` | Sets the Git username used for identifying commits. |
| `git config --global user.email "andoyonly@gmail.com"` | Sets the Git email address used for identifying commits. |
| `mkdir screenshots` | Creates a directory for storing laboratory screenshots. |
| `touch README.md security-audit-report.md firewall-configuration.md reflection.md` | Creates the Markdown files needed to document the laboratory activity. |
| `git add .` | Stages the created and modified files for committing. |
| `git commit -m "Creating Lab work 8"` | Saves the staged changes in the local Git repository with a descriptive commit message. |
| `git push` | Uploads the committed laboratory files to the remote GitHub repository. |
| `ls -a` | Lists files and directories, including hidden files, to verify the repository contents. |

## 🧠 Skills Learned

- Understanding the Principle of Least Privilege and the concept of attack surface.
- Configuring the UFW firewall on Ubuntu 24.04.
- Applying a Default Deny policy to incoming network connections.
- Allowing SSH access before enabling the firewall to maintain remote administration.
- Managing specific firewall rules for TCP port 8080.
- Checking firewall status, default policies, and numbered rules.
- Deploying an Nginx web application using Docker.
- Managing Docker containers and checking their running status.
- Testing web application connectivity using `curl`.
- Understanding how Docker port mapping connects a host port to a container port.
- Creating and organizing Markdown documentation for laboratory reports.
- Using Git commands to clone, configure, stage, commit, and push project files.
- Uploading laboratory documentation to GitHub.
- Maintaining and expanding a professional Cloud Computing portfolio.
