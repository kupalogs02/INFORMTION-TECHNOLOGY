# Types of Cloud Storage

| Storage Type       | Description                                                                                                                 | Primary Use Case                                                                     | Cloud Provider Example |
| ------------------ | --------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------ | ---------------------- |
| **Block Storage**  | Stores data in fixed-size blocks that can be managed individually by an operating system.                                   | Virtual machine disks, databases, and applications that require low-latency storage. | AWS EBS                |
| **File Storage**   | Stores data as files organized in folders and directories. Multiple systems can access the same file system over a network. | Shared files, documents, application files, and content repositories.                | AWS EFS                |
| **Object Storage** | Stores data as objects together with metadata and a unique identifier inside a storage container called a bucket.           | Images, videos, backups, logs, and other large amounts of unstructured data.         | Amazon S3              |

## Why Object Storage Is Suitable for the Client

Object Storage is well suited for the client's photo-sharing application because images are unstructured files that can be stored as individual objects and accessed when needed. It is also designed for large-scale storage, making it appropriate for applications that may eventually contain millions of user-uploaded photos.

