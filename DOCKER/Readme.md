## Docker
Docker is a platform that allows you to develop, ship, and run applications inside containers. Containers are lightweight, portable, and self-sufficient environments that contain everything needed to run an application, including the code, runtime, system tools, libraries, and dependencies.

### What is Containerization?
- Docker enables containerization, which involves packaging an application and its dependencies into a standardized unit called a container. Containers are isolated from each other and from the underlying host system, providing consistency and reproducibility across different environments.

### Difference between VM And Container?
- Containers and virtual machines (VMs) are virtualization technologies used to run multiple environments on a single host, but they differ in architecture and approach. Containers share the host OS's kernel and resources, while VMs run a complete guest OS on top of a hypervisor. Containers are lightweight, with minimal resource overhead, making them ideal for microservices and rapid deployment. VMs have higher resource overhead due to their separate guest OS, making them less efficient in resource utilization. Containers are highly portable, running consistently across different environments, while VMs may require additional configuration for portability. Containers provide process-level isolation, while VMs offer stronger isolation with separate kernels. Containers are suited for modern, cloud-native applications, while VMs are often used for legacy or monolithic applications. The choice between containers and VMs depends on factors such as resource efficiency, isolation requirements, and application portability needs.

  ![Alt Text](https://images.contentstack.io/v3/assets/blt300387d93dabf50e/bltb6200bc085503718/5e1f209a63d1b6503160c6d5/containers-vs-virtual-machines.jpg)

### Archeitecture

#### Docker Daemon (dockerd):

- The Docker daemon (dockerd) is a background service that runs on the host system. It's responsible for managing Docker objects such as images, containers, volumes, and networks.
- The Docker daemon listens for Docker API requests and communicates with the Docker client (docker) to execute commands.

![Alt Text](https://miro.medium.com/v2/resize:fit:1358/1*Q-9FEZawpzE63afTdtEZ4w.gif)


#### The Docker client (docker):
- is a command-line interface (CLI) tool that allows users to interact with the Docker daemon. Users can use the Docker client to build, run, and manage containers using various commands.
The Docker client sends API requests to the Docker daemon, which executes the requested actions on the host system.
Docker Images:

#### Docker images:
- are read-only templates that contain the filesystem and configuration settings needed to run a container. Images are built using Dockerfiles, which specify the instructions for creating the image layer by layer.
Docker images are stored in a local or remote registry, such as Docker Hub or a private registry. They can be pulled from a registry to create containers on any Docker host.
Docker Containers:

#### Docker containers
- are lightweight, portable, and self-sufficient runtime environments that run applications and their dependencies. Each container is created from a Docker image and runs as a separate process on the host system.
Containers are isolated from each other and from the host system using kernel-level features like namespaces and control groups (cgroups).
Docker Registry:

#### The Docker registry:
- is a storage service that holds Docker images. It allows users to push, pull, and manage Docker images from local or remote repositories.
Docker Hub is the official public registry provided by Docker, where users can store and share Docker images publicly or privately. Organizations can also set up their private Docker registries for internal use.
Docker Engine:

#### Docker Engine:
- refers to the combination of the Docker daemon (dockerd), the Docker client (docker), and the container runtime (e.g., containerd or runc). Together, these components form the core of Docker's architecture and enable containerization on the host system.
Docker Engine is available on various platforms, including Linux, Windows, and macOS, allowing users to run containers on different operating systems.


### Docker Hub:
- Docker Hub is a cloud-based service provided by Docker that allows users to store, share, and manage Docker container images. It serves as a centralized resource for Docker users to find and distribute container images. Docker Hub provides public repositories for storing open-source images and private repositories for individuals or organizations to store proprietary images securely.

### dockerFile:
- A Dockerfile, on the other hand, is a text-based script that contains a series of instructions used to build a Docker image. These instructions define the steps needed to create a Docker image, including specifying a base image, installing dependencies, copying files, setting environment variables, and more. Dockerfiles provide a simple and efficient way to automate the creation of Docker images, making it easier to reproduce and distribute software environments consistently across different systems.

### Common Docker Command:

![Alt Text](https://raw.githubusercontent.com/sangam14/dockercheatsheets/master/dockercheatsheet8.png)




