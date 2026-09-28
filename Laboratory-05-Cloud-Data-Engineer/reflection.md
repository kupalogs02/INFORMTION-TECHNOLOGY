# Mission Reflection

This laboratory helped me understand why object storage is commonly used for applications that handle large amounts of unstructured data such as photos. Compared with traditional block storage, object storage organizes files as objects and provides metadata and unique identifiers for accessing them. For a photo-sharing application that may store millions of images, this approach is more suitable because the data can be managed as individual objects in a bucket rather than being treated like a traditional computer disk.

Docker made the deployment of MinIO easier because I did not have to manually install and configure every component required by the storage server. By using a Docker image and a single command, I was able to create a MinIO container, configure its ports, provide the administrator credentials through environment variables, and start the service. This also demonstrated how containers can make application deployment more consistent and portable.

A bucket is a storage container used to organize objects in an object storage system. In this activity, I created a bucket named `client-photos` and uploaded a sample file to verify that the MinIO server was working properly.

Large enterprise companies use several methods to reduce the possibility of permanent data loss. These can include redundancy, replication, backups, multiple storage devices, and geographically distributed copies of important data. These techniques help ensure that data can still be recovered when a physical server or storage device fails.

My confidence in navigating the Linux command line is also improving. I became more comfortable using Docker commands, checking running containers, and working with a cloud service from a terminal environment. This activity showed me that command-line skills are useful for cloud engineering because many deployment and administration tasks can be performed efficiently without relying entirely on graphical interfaces.

