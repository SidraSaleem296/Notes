# 📘 Lecture 5: Virtualization, Containerization, and Docker

#### 📌 Topics of Lecture

1. **Virtualization**: Hypervisors and Types
2. **Containerization**: Containers and Tools
3. **Docker**: Terminologies, Architecture, and Management

***

#### 💻 Virtualization

* **Virtualization** creates an abstraction layer between applications and hardware, allowing multiple **virtual machines (VMs)** to share resources (CPU, memory, storage) on a single computer.
* **Benefits**: Optimizes hardware usage, enhances security, and supports multi-tenancy in cloud computing.

**Host Machine**: The physical computer running virtual machines.\
**Guest Machine**: The virtual machine itself.

***

**🖥️ Hypervisor Types**

1. **Type 1 Hypervisor (Bare Metal)**:
   * Runs directly on hardware for high efficiency.
   * Examples: VMware ESXi, Microsoft Hyper-V.
2. **Type 2 Hypervisor (Hosted)**:
   * Runs on an OS as an application, ideal for end-user productivity.
   * Examples: Oracle VM VirtualBox, VMware Workstation.

**💡 Exam Questions**:

1. Define virtualization and explain its role in cloud computing.
2. Differentiate between Type 1 and Type 2 hypervisors.

***

#### 📦 Containerization

* **Containerization** isolates applications in user spaces called **containers**, packaging everything the app needs (libraries, binaries, dependencies).
* **Difference from Virtualization**: Containers share the host OS kernel, unlike VMs which have separate OS instances.

**Popular Containerization Tools**:

1. **Docker**: Leading container platform, simplifies container creation and management.
2. **Kubernetes**: Manages containerized applications across multiple hosts.

**💡 Exam Questions**:

1. Explain containerization and its advantages over virtualization.
2. List and describe two popular containerization tools.

***

#### 🐳 Docker: Overview and Key Terms

**🛠️ Docker Terminologies**

* **Dockerfile**: A text file with instructions to build a Docker image.
* **Docker Image**: Read-only package that includes everything needed to run an application.
* **Docker Container**: A running instance of a Docker image.
* **Docker Hub**: A public repository for sharing Docker images.

**🏗️ Docker Architecture**

1. **Docker Host**: Runs the Docker daemon and hosts images, containers, networks, and storage.
2. **Docker Client**: Sends commands to Docker Daemon for managing Docker services.
3. **Docker Registry**: Manages and stores Docker images, like Docker Hub.

**💡 Exam Questions**:

1. Describe the role of a Dockerfile in Docker.
2. Explain the three main components of Docker architecture.

***

#### ⚙️ Dockerfile Commands

1. **FROM**: Base image for the Docker image.
2. **MAINTAINER**: Specifies the image’s maintainer.
3. **RUN**: Runs commands in the container.
4. **COPY**: Copies files from host to container.
5. **EXPOSE**: Opens a port in the container.

**Dockerfile Example**:

```Dockerfile
DockerfileCopy codeFROM python:latest
RUN apt-get update
COPY app.py .
CMD python app.py
```

**💡 Exam Questions**:

1. Explain the purpose of the `FROM` and `RUN` commands in a Dockerfile.
2. What does the `COPY` command do in Dockerfile syntax?

***

#### 📝 Docker Management Commands Cheat Sheet

**🚀 Docker CLI Commands (from Docker Cheat Sheet PDF)**

* **Build an Image**: `docker build -t <image_name>`
* **Run a Container**: `docker run --name <container_name> <image_name>`
* **Start/Stop a Container**: `docker start|stop <container_name>`
* **View Logs**: `docker logs -f <container_name>`
* **Delete an Image**: `docker rmi <image_name>`
* **Open Shell in Container**: `docker exec -it <container_name> sh`

**💡 Exam Questions**:

1. Write the command to build a Docker image from a Dockerfile.
2. How would you open a shell in a running Docker container?
