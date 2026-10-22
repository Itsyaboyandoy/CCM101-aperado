# ☁️ Mission Reflection
Writing a docker-compose.yml file makes a cloud engineer's job easier because it organizes the configurations for multiple services in one file. Instead of manually typing commands to start each container, I was able to define the Nextcloud application and MariaDB database in the Compose file and start them together. This saves time, reduces repetitive work, and makes deployment easier to manage.

A YAML file requires proper formatting, especially spacing and indentation. If I make an indentation error or use a Tab instead of Spaces, Docker Compose may fail to read the configuration file and display an error. As a result, the containers may not start until the mistake is corrected. Through this activity, I learned the importance of following the correct YAML structure.

Environment variables such as MYSQL_PASSWORD were used to provide the configuration settings needed by the containers. These settings help Nextcloud connect to the MariaDB database correctly. I also learned that passwords must be handled carefully and should not be exposed in public repositories.

Deploying Nextcloud in just a few minutes was an exciting and valuable experience. Based on my screenshots, I was able to start the Nextcloud and MariaDB containers, check their status using Docker Compose, and access the Nextcloud setup page through a browser. This helped me understand how different services work together to support a cloud application.

Since Mission 1, my understanding of Cloud Computing has improved. Before, I mainly viewed cloud computing as accessing services through the internet. After completing this activity, I gained a better understanding of containers, service communication, environment variables, and automated deployment.

Overall, this laboratory helped me understand how Docker Compose makes cloud deployment more organized and efficient. I also learned how to check running containers and stop the deployment when it was no longer needed. This experience gave me more confidence in working with cloud technologies and understanding how applications are deployed and managed.
