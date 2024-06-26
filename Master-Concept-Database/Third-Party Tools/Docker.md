---
tags: Azure
---

Building and testing with a multi-stage [[Docker]] file executes from within a container meaning the results are not published back to any pipeline. A multi-stage build is useful for optimising Dockerfiles whilst maintaining readability and maintenance.

Docker is a platform and toolset that allows you to develop, deploy, and run applications in containers. Containers are lightweight, portable, and self-sufficient units that encapsulate an application and its dependencies, including libraries, runtime, and system tools. Docker provides a consistent environment across different stages of the application lifecycle, from development to testing and production.

Key features of Docker include:

1. **Containerization:** Docker allows you to package an application and its environment into a single container image. This image contains everything needed to run the application, making it easy to move between different environments and ensuring consistent behavior.
    
2. **Isolation:** Containers provide process isolation, allowing applications to run without interfering with each other. This isolation helps avoid conflicts between dependencies and simplifies the management of software components.
    
3. **Portability:** Docker containers can run on any system that supports Docker, whether it's a developer's laptop, on-premises servers, or cloud infrastructure. This portability eliminates the "it works on my machine" problem and simplifies deployment.
    
4. **Versioning:** Docker images can be versioned, enabling you to track changes over time and revert to previous versions if needed. This is especially useful for maintaining a history of application releases.
    
5. **Efficiency:** Containers share the host OS kernel, which results in lower overhead compared to traditional virtualization. This efficiency allows for greater resource utilization and faster startup times.
    
6. **Scalability:** Docker makes it easy to scale applications horizontally by creating multiple instances of containers. Container orchestration tools like Kubernetes can help manage and scale containers across a cluster of machines.
    
7. **Microservices:** Docker is often used in microservices architectures, where different components of an application are containerized and can communicate through APIs. This approach promotes modularity and flexibility in building and deploying complex applications.
    
8. **DevOps and CI/CD:** Docker simplifies continuous integration and continuous deployment (CI/CD) pipelines by providing consistent environments for testing and deployment stages. Developers can build, test, and package applications in containers, ensuring that the same environment is used from development to production.
    

Docker has become a widely adopted technology in software development and deployment due to its flexibility, ease of use, and ability to streamline development workflows, improve resource utilization, and enhance application scalability and maintainability.