# Laboratory 04 – Cloud-Native Engineer

## Mission Overview

This laboratory introduced the fundamentals of cloud-native computing by comparing Virtual Machines (VMs) and containers. Using the KillerCoda Docker Playground, I learned how to pull Docker images, deploy an Nginx web server, and manage the container lifecycle.

## Objectives

* Understand the differences between Virtual Machines and Containers.
* Verify that Docker is installed and running.
* Pull and use an official Docker image.
* Deploy an Nginx web server using Docker.
* Manage containers using basic Docker commands.
* Understand the container lifecycle from creation to removal.
* Practice documenting cloud-native deployment procedures.

## Docker Commands Executed

### Checkpoint 3 – Enter the Docker Playground

```bash
docker --version
docker info
docker run hello-world
```

### Checkpoint 4 – Deploy Your First Container

```bash
docker pull nginx
docker run -d -p 8080:80 --name nginx-server nginx
curl http://localhost:8080
docker ps
```

### Checkpoint 5 – The Container Lifecycle

```bash
docker ps
docker stop nginx-server
docker ps
docker rm nginx-server
```

## Skills Learned

* Learned how to verify a Docker installation and environment.
* Learned how to download Docker images from Docker Hub.
* Learned how to create and run containers in detached mode.
* Learned how to map host ports to container ports.
* Learned how to test a web server using `curl`.
* Learned how to list, stop, verify, and remove Docker containers.
* Learned the basic lifecycle of a Docker container.

## Challenges Encountered

One challenge was understanding the difference between a Docker image and a container. Another challenge was correctly mapping port 8080 on the host to port 80 inside the Nginx container. I also had to make sure that the container was stopped before removing it. By following the commands step by step, I was able to successfully deploy and manage the Nginx container.

