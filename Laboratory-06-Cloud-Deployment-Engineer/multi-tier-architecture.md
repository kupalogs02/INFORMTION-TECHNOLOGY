# Multi-Tier Architecture

## What Is a Two-Tier Architecture?

A two-tier architecture is a system design that separates an application into two main parts: the web/application tier and the database tier. In this laboratory activity, Nextcloud serves as the web application, while MariaDB stores the data needed by the application. Both run in separate Docker containers and communicate with each other.

## The Web/Application Tier

The web/application tier is responsible for displaying the user interface and handling requests from users through a web browser. In this project, **Nextcloud** serves as the web application. Users can access its setup page through port `8080`, which is mapped to port `80` inside the Nextcloud container.

## The Database Tier

The database tier stores and manages information required by the application, such as user account information and file metadata. In this project, **MariaDB** acts as the database server. It stores the application's data and allows Nextcloud to retrieve and manage information when needed.

## Why Separate Them?

Separating the web application and database into two containers makes the system easier to manage, maintain, and troubleshoot. Each container has its own responsibility, so the application and database can be configured or updated independently. This setup also makes it easier to scale the services and organize the deployment.

## How the Two Tiers Communicate

Docker Compose connects the Nextcloud and MariaDB services within the same application environment. The `MYSQL_HOST=database` environment variable tells Nextcloud to connect to the database service named `database`. This allows the application to communicate with MariaDB without needing to use a public IP address.

## Conclusion

Through this activity, I learned that a two-tier architecture separates the web application from the database while allowing them to work together. Using Nextcloud and MariaDB with Docker Compose makes the deployment more organized and easier to manage. This approach also demonstrates how containers can be used to build a private cloud storage system.
