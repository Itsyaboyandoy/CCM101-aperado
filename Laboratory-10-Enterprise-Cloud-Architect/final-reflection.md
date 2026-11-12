# 🎓 Final Reflection
## CCM101 – Cloud Computing
### Mission 10: The Enterprise Cloud Architect

## 📖 Introduction

My journey through the ten laboratory missions in CCM101 gave me a deeper appreciation of cloud computing and the responsibilities involved in managing modern IT infrastructure. At the beginning of the course, I had a basic understanding of cloud technology. However, as I progressed through each activity, I discovered that operating cloud-based systems requires knowledge of several connected technologies.

The course helped me recognize that cloud computing goes beyond accessing online services and storing information on the internet. It also involves managing server environments, connecting applications, maintaining data availability, implementing security measures, and automating important processes.

Each mission contributed to my understanding and prepared me for the more challenging tasks in our final laboratory activity.

## ☁️ Knowledge and Skills Developed from Missions 1–9

The earlier laboratory activities helped me establish the technical foundation needed to understand cloud infrastructure.

One of the topics I explored was the relationship between computing resources, networking, and storage. I learned how these components support applications and why proper infrastructure planning is necessary before deploying a system. Studying cloud platforms such as AWS, Microsoft Azure, and Google Cloud also introduced me to different technologies and services used in cloud environments.

Another important part of my learning experience was becoming more comfortable with Linux. By executing commands through the terminal, I practiced gathering information about the operating system, processor, memory, storage, and other system resources. These activities strengthened my familiarity with command-line operations and basic server administration.

I also explored automation through Windows PowerShell. This helped me understand how scripts can simplify system monitoring and reduce the amount of repetitive manual work. Instead of performing the same checks individually, I learned that certain processes can be executed more efficiently through automation.

The previous missions also emphasized system security. I became more aware of the importance of controlling access, managing network connections, configuring security rules, and protecting information from unauthorized access.

Looking back, these activities were valuable because they gradually connected theoretical concepts with practical applications.

## 🏗️ Applying My Knowledge in Mission 10

The final mission, **The Enterprise Cloud Architect**, challenged me to combine the skills I had developed throughout the course into a functional infrastructure project.

For this activity, I worked on **CloudNova**, a web application hosting environment built using Ubuntu Server and Oracle VirtualBox.

I configured a virtual server and established network connectivity between the Ubuntu environment and my Windows computer. This allowed me to access the deployed WordPress website through a web browser and observe how the application operated within the virtualized environment.

I also worked with Docker and Docker Compose to manage two interconnected services: WordPress and MariaDB. Through this setup, I gained a better understanding of containerization and how applications communicate with databases.

A particularly useful concept was persistent storage. I learned that Docker volumes help preserve database information even when containers are stopped, restarted, or recreated.

Security was another significant part of the activity. I configured the UFW firewall, applied restrictions to network access, and implemented SSH key authentication instead of relying on password-based SSH access. I also worked with Docker-related firewall settings to control access to the hosted application.

Additionally, I explored server automation by developing a Bash script for database backups. The script was designed to create and compress database backup files, verify their validity, and remove backups older than seven days. I then configured Cron to execute the process automatically on a daily schedule.

Completing these tasks helped me understand how virtualization, networking, containers, security, storage, and automation contribute to maintaining a functional server environment.

## ⚠️ Difficulties Encountered and What I Learned

Mission 10 was not entirely easy because several configurations required careful attention and troubleshooting.

One of the challenges I encountered involved establishing stable communication between my Windows computer and the Ubuntu virtual machine. I also needed to understand how SSH settings, firewall configurations, and Docker networking affected access to different services.

There were times when I had to review my configurations, inspect the system's behavior, and repeat certain tests before achieving the expected results.

Developing the automated backup process was another challenge. I had to understand how the Bash script interacted with the database, how backup files were generated and compressed, and how Cron could execute the task without manual intervention.

These experiences reminded me that working with servers is not simply about entering commands and expecting everything to function immediately. It requires logical thinking, troubleshooting skills, patience, and an understanding of how different components affect one another.

Most importantly, I learned the value of verifying configurations and understanding their purpose instead of executing commands without knowing their possible effects.

## 🎯 Personal Reflection and Conclusion

After completing the CCM101 laboratory missions, I can say that my understanding of cloud computing has improved significantly.

The activities allowed me to gain practical exposure to Linux administration, virtual machines, cloud infrastructure, networking, PowerShell, Docker, server security, and Bash automation.

Among all the missions, Mission 10 was particularly meaningful because it required me to apply several concepts together rather than completing them as separate exercises. Building the CloudNova infrastructure helped me appreciate the planning, technical decisions, and maintenance responsibilities involved in managing a server.

I also realized that successful IT solutions depend not only on making applications work but also on ensuring that they remain secure, accessible, and reliable.

Although I still have much to learn about cloud technologies and infrastructure management, this course helped me develop greater confidence in working with unfamiliar tools and solving technical problems.

The knowledge and experiences I gained from CCM101 will be useful in my future academic projects and professional development as an aspiring IT practitioner.
