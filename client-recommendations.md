# Client Recommendations

## Client A – Startup Company

### Recommended Platform: AWS

AWS is a suitable choice for the startup because it provides many cloud services that can scale as the mobile application grows. The company can begin with smaller resources and increase capacity when demand increases. AWS also provides services for application hosting, databases, storage, and content delivery.

**Recommended Services:**

* Amazon EC2
* Amazon S3
* Amazon RDS
* Amazon CloudFront

---

## Client B – University

### Recommended Platform: Microsoft Azure

Microsoft Azure is the most appropriate choice because the university already uses Windows Server, Microsoft 365, and Active Directory. Azure provides strong integration with Microsoft's identity and enterprise technologies. This can make cloud migration and centralized identity management easier.

**Recommended Services:**

* Azure Virtual Machines
* Microsoft Entra ID
* Azure SQL Database
* Azure Blob Storage

Microsoft Entra ID is Microsoft's identity and access-management service, and Microsoft documentation confirms its integration with Azure SQL for centralized identity and permission management.

---

## Client C – AI Research Company

### Recommended Platform: Google Cloud

Google Cloud is a strong choice for the AI research company because it provides services designed for artificial intelligence and machine learning workloads. Compute Engine can provide high-performance virtual machines, including GPU resources where available. Google Kubernetes Engine can also support containerized AI applications.

**Recommended Services:**

* Compute Engine
* Google Kubernetes Engine
* Cloud Storage
* Vertex AI

Google Cloud documents GPU availability for Compute Engine and GKE workloads, including specialized locations intended for large-scale AI and machine-learning workloads.

---

## Client D – Global E-Commerce Company

### Recommended Platform: AWS

AWS is a suitable choice for the global e-commerce company because it provides global infrastructure and services designed for scalability and high availability. The company can distribute resources across multiple Availability Zones and Regions. Load balancing and automatic scaling can help the application handle changing customer demand.

**Recommended Services:**

* Amazon EC2
* Elastic Load Balancing
* Amazon RDS
* Amazon CloudFront
* EC2 Auto Scaling

AWS recommends distributing applications across multiple Availability Zones to improve availability when an individual location experiences a failure.

# Multi-Cloud Decision Matrix

| Business Requirement    | Recommended Platform | Justification                                       |
| ----------------------- | -------------------- | --------------------------------------------------- |
| Startup Company         | AWS                  | Broad services and flexible scalability             |
| Enterprise Organization | AWS                  | Broad service portfolio and enterprise capabilities |
| Microsoft Environment   | Azure                | Strong Microsoft integration                        |
| AI / Machine Learning   | GCP                  | Strong AI/ML capabilities and GPU options           |
| Kubernetes Deployment   | GCP                  | Google Kubernetes Engine                            |
| Global Web Application  | AWS                  | Global infrastructure and scalability               |

