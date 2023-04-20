# Container overview
A **container** is a lightweight, standalone executable package that contains everything an application needs to run, including code, libraries, dependencies, and system tools. Containers are designed to be portable, scalable, and isolated from the host system and other containers.

**Key concepts**
* **Image**: An image is a read-only template that defines the application and its dependencies.
* **Container**: A container is a runtime instance of an image. It is isolated from other containers and the host system, and has its own file system, network interfaces, and resources.
* **Registry**: A registry is a repository for storing and distributing container images. The most popular registry is Docker Hub, but you can also use private registries for storing images.

**Benefits of containers**
* **Portability**: Containers can run on any platform that supports containerization, from laptops to cloud servers. This makes it easy to move applications between development, testing, and production environments.
* **Isolation**: Containers are isolated from the host system and other containers, which makes them more secure and less prone to conflicts.
* **Efficiency**: Containers are lightweight and share the host system's resources, which makes them more efficient than traditional virtual machines.

**Drawbacks of containers**
* **Limited resource allocation**: Containers share the resources of the host system, which means that each container has a limited amount of CPU, memory, and disk space. This can become a problem if an application requires more resources than the container can provide.
* **Security concerns**: Containers are isolated from the host system and other containers, but they still share the same kernel as the host system. This can create potential security risks, especially if the container has vulnerabilities or is misconfigured.
* **Complexity**: Containers add an extra layer of complexity to software development and deployment. You need to manage the container runtime, container images, container networking, and container orchestration, which can be challenging if you're not familiar with these technologies.
* **Debugging difficulties**: Debugging applications in containers can be more difficult than debugging applications on the host system. You need to understand how the container runtime and container networking work to troubleshoot issues effectively.
* **Dependency management**: While containers help manage dependencies by bundling everything an application needs to run, they can also introduce dependency management issues. If two containers require different versions of the same library, for example, you'll need to find a way to resolve the conflict.


## Running single container applications
### `docker`
## Running multi-container applications
### `docker-compose`
### Kubernetes
### Helm
