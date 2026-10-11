# Mission 6: The Cloud Deployment Engineer

## Laboratory Reflection

In this laboratory activity, I learned how to deploy a private cloud storage system using Docker Compose. I realized that writing a `docker-compose.yml` file makes a cloud engineer's job easier because all the configurations are placed in one file. Instead of typing separate commands for every container, I can use one command to start the application and its database. This saves time and makes the deployment process more organized.

I also learned that YAML indentation is very important. If I use incorrect spacing or a Tab instead of spaces, Docker Compose may show an error and fail to read the configuration properly. Because of this, I need to check the format and indentation carefully before deploying the containers.

Environment variables, such as `MYSQL_PASSWORD`, are used to provide configuration values to the containers. They help Nextcloud connect to the MariaDB database using the correct database name, username, password, and host. I also realized that passwords should be protected and handled securely, especially when working with real applications.

Deploying Nextcloud was an interesting experience because I learned that a cloud storage application can be prepared in just a few minutes using Docker Compose. It helped me understand how different containers can work together as one system. I also learned the importance of checking whether the containers are running and accessing the application through a browser.

Since Mission 1, my understanding of cloud computing has improved. Before, I mainly understood cloud computing as using online services to store files and access applications. Now, I have a better understanding of how cloud services can be built and managed using containers and configuration files. This activity taught me that planning, proper configuration, and documentation are important skills for an IT student who wants to become a cloud engineer.

Overall, this laboratory activity improved my knowledge of Docker Compose, multi-tier architecture, and Infrastructure as Code. I believe these skills will help me in future cloud computing activities and projects.
