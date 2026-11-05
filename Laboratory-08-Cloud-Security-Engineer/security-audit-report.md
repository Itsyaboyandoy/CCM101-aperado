# 🛡️ Security Audit Report

## 🔑 1. Principle of Least Privilege (PoLP)

The Principle of Least Privilege means giving users and services only the permissions they need to perform their tasks. This helps protect cloud servers by reducing unnecessary access and preventing unauthorized users from reaching important resources.

## 🎯 2. Attack Surface

An attack surface refers to all the possible entry points that attackers could use to access a system. Examples include open network ports, running services, applications, and exposed server resources. Reducing unnecessary services and open ports helps minimize security risks.

## 🚫 3. Default Deny Policy

A Default Deny Policy blocks incoming connections unless they are specifically allowed. In this activity, I configured UFW to deny incoming traffic by default and allow outgoing connections. This provides better protection against unauthorized network access.

## 🔥 4. Firewall Configuration

I configured UFW to allow SSH connections and TCP port 8080. SSH allows remote server administration, while port 8080 provides access to the Nginx web application. The firewall status and numbered rules confirmed that these permissions were successfully added.

## 🐳 5. Docker Application Verification

I created and ran a Docker container named `secure-web-app` using the Nginx image.

```bash
docker run -d -p 8080:80 --name secure-web-app nginx
```

I checked the running container using:

```bash
docker ps
```

The output confirmed that the container was running and that host port 8080 was mapped to container port 80.

I also tested the application using:

```bash
curl http://localhost:8080
```

The command returned the default Nginx welcome page, confirming that the web application was accessible.

## 🔍 6. Security Assessment

Based on the activity, the firewall was successfully enabled with a default deny incoming policy. SSH and port 8080 were explicitly allowed, and the Nginx application was successfully tested.

These configurations demonstrate how a cloud server can use firewall rules and application verification to improve security while maintaining the necessary services.
