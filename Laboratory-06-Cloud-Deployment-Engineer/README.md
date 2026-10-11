# Laboratory 06: Cloud Deployment Engineer

## Mission Overview

This laboratory activity focuses on deploying a private cloud storage system using **Docker Compose**. I used Nextcloud as the web application and MariaDB as the database. These two containers work together to create a two-tier application architecture. Instead of starting each container manually, I used a YAML configuration file to define the services and deploy them together.

## Objectives

* Understand the concept of a two-tier application architecture.
* Learn how to create and configure a `docker-compose.yml` file.
* Deploy Nextcloud and MariaDB using Docker Compose.
* Access the Nextcloud web interface through a browser.
* Understand Infrastructure as Code (IaC).
* Document the deployment process and organize screenshots in GitHub.

## Commands Executed

The following commands were used during the laboratory activity:

```bash
# Create and enter the project directory
mkdir nextcloud-deployment
cd nextcloud-deployment

# Create the Docker Compose configuration
nano docker-compose.yml

# Deploy the containers
docker-compose up -d

# Check the container status
docker-compose ps

# Stop and remove the containers
docker-compose down
```

## Skills Learned

Through this activity, I learned how to deploy multiple containers using Docker Compose. I understood how Nextcloud communicates with MariaDB through the `MYSQL_HOST` environment variable. I also learned the importance of correct YAML indentation, environment variables, and separating an application from its database. This activity helped me understand how Infrastructure as Code makes cloud deployment more organized, repeatable, and easier to manage.

## Screenshots

The following screenshots serve as evidence of the deployment process:

* `screenshots/compose-deployment.png` — Shows the containers running after deployment.
* `screenshots/nextcloud-web.png` — Shows the Nextcloud installation page in a browser.
* `screenshots/compose-teardown.png` — Shows the result of stopping and removing the containers.

## Conclusion

This laboratory activity helped me understand how a multi-container application can be deployed using a single configuration file. I gained practical experience with Docker Compose and learned how application and database services work together in a private cloud storage environment.
