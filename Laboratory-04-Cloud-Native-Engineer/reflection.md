# Mission Reflection

Through this laboratory activity, I learned how containerization makes application deployment faster and more efficient compared to traditional Virtual Machines. A Docker container can start within seconds because it does not need to install or boot a complete operating system. In contrast, setting up a Virtual Machine requires installing a Guest OS, configuring its resources, and waiting for the operating system to boot. This makes containers more practical when applications need to be deployed or scaled quickly.

Port mapping such as `-p 8080:80` is necessary because the web server inside the container listens on port 80, while the host machine needs a way to access that service. Port 8080 on the host is connected to port 80 inside the container, allowing me to access the Nginx web server through `http://localhost:8080`. Without port mapping, the service running inside the container may not be directly accessible from the host.

When the `docker rm` command is used, the container itself is permanently removed. Any data stored only inside the container's writable layer is also deleted. This shows why persistent data should be stored using Docker volumes or other external storage when it needs to survive the removal of a container.

Containerization also improves collaboration between software developers and IT operations teams. Developers can package an application together with its dependencies into a container, while operations teams can deploy the same container consistently across different environments. This supports DevOps by reducing environment-related problems and making development, testing, and deployment more consistent.

My GitHub portfolio is also evolving as I add more laboratory activities, documentation, screenshots, and projects. It is becoming a record of the technical skills I am developing in cloud computing, Docker, programming, and IT systems. By continuously organizing and updating my repositories, I can demonstrate my progress and practical experience as an Information Technology student.

