# Docker Compose Guide

## Introduction

Docker Compose is a tool that allows us to define and manage multiple Docker containers using a single YAML configuration file. In this laboratory activity, I used Docker Compose to deploy Nextcloud and MariaDB together. This made the deployment process easier because both services could be configured and started using one command.

## 1. The `services:` Block

The `services:` block defines the containers that will run in the application. In my `docker-compose.yml` file, I created two services: `database` and `app`.

* **database:** Uses the `mariadb:10.6` image to store the application's data.
* **app:** Uses the `nextcloud` image to provide the web application and user interface.

Each service has its own configuration, including environment variables and, for the Nextcloud application, port mapping.

## 2. How Nextcloud Finds the Database

The Nextcloud application connects to MariaDB through the following environment variable:

```yaml
MYSQL_HOST=database
```

The value `database` is the service name defined in the Compose file. Docker Compose provides network communication between the services, allowing Nextcloud to locate MariaDB using that name. The other environment variables, such as `MYSQL_DATABASE`, `MYSQL_USER`, and `MYSQL_PASSWORD`, provide the database connection settings.

## 3. Difference Between `docker run` and `docker-compose up -d`

### Docker Run

The `docker run` command starts an individual container. Its configuration, such as the image, ports, and environment variables, is usually provided directly in the command. When deploying multiple related containers, separate commands may be needed.

### Docker Compose

The `docker-compose up -d` command starts the services defined in a `docker-compose.yml` file in detached mode, meaning they run in the background. It is useful for multi-container applications because the services and their configurations are organized in one file.

## 4. Commands Used

The following commands were used during the deployment process:

```bash
# Create the project directory
mkdir nextcloud-deployment
cd nextcloud-deployment

# Create the Compose configuration file
nano docker-compose.yml

# Start the application services
docker-compose up -d

# Check the status of the containers
docker-compose ps

# Stop and remove the containers
docker-compose down
```

## 5. Port Mapping

The Compose file uses the following configuration:

```yaml
ports:
  - 8080:80
```

This maps port `8080` on the host environment to port `80` inside the Nextcloud container. It allows users to access the Nextcloud web interface through port `8080` using the KillerCoda playground's port-access feature.

## 6. Environment Variables

Environment variables provide configuration values to the containers. In this activity, variables such as `MYSQL_DATABASE`, `MYSQL_USER`, and `MYSQL_PASSWORD` configure the database connection. The `MYSQL_HOST` variable identifies the database service that Nextcloud should connect to.

For a real deployment, passwords should be handled securely rather than stored directly in a Compose file.

## Conclusion

Through this laboratory activity, I learned how Docker Compose simplifies the deployment of multi-container applications. I also learned how service names, port mapping, and environment variables help Nextcloud communicate with MariaDB. Overall, Docker Compose is useful for organizing infrastructure configuration and making deployments easier to repeat and manage.
