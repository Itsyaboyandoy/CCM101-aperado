# 📝 Reflection

During this laboratory activity, I learned how important it is to secure a cloud server by controlling incoming and outgoing network connections. Before this activity, I mainly focused on making sure applications were running properly. Now, I understand that protecting the server from unauthorized access is equally important.

One of the things I learned was how to configure the UFW firewall in Ubuntu 24.04. I used commands to allow SSH connections, deny incoming connections by default, and allow outgoing connections. I also learned why SSH must be allowed before enabling the firewall to avoid losing remote access to the server.

Another important part of the activity was allowing TCP port 8080. This allowed me to access the Nginx web application running inside my Docker container. I used `docker ps` to check whether the container was running and `curl http://localhost:8080` to verify that the application was working correctly.

I also learned about the Principle of Least Privilege and the Default Deny Policy. These security concepts help reduce unnecessary access and protect important resources. Allowing only the required ports makes the server less exposed to possible attacks.

During the activity, I encountered a small error when I initially entered the SSH firewall command incorrectly. I corrected it by using `sudo ufw allow ssh`. This reminded me that even small typing mistakes can affect server configuration, so checking command results is important.

Finally, I uploaded my completed Lab 8 files to my GitHub repository. This helped me practice documenting my work, using Git commands, and keeping a record of my progress in cloud computing.

Overall, this activity improved my understanding of cloud server security. I learned that properly configuring a firewall, limiting unnecessary access, testing applications, and documenting the process are important responsibilities when managing a cloud environment.
