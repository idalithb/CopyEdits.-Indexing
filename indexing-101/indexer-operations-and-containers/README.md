# Indexer Operations and Containers

Containers are a vital component of the work that indexers perform within The Graph protocol. Therefore, it’s crucial to understand their functionality. Containers provide a consistent and reliable environment for running the indexing software that is required by indexers. By packaging the indexing software and its dependencies into a container, indexers can easily deploy and run the software on their local machines or on cloud infrastructure. This not only makes Indexer's jobs more efficient, but it also reduces the barrier for new indexers who want to join the network.

Containers facilitate the mechanisms indexers need to compute resources within The Graph. They provide a way to isolate the indexing software from the host operating system, which improves security and stability. Each container runs within its own isolated environment, so issues with the indexing software or its dependencies do not affect other parts of the system. This process reduces the risk of conflicts and makes it easier to manage and update the software. 

Overall, containers play a crucial role because they enable indexers to perform efficiently within The Graph’s protocol, they provide a consistent and reliable environment for running indexing software, and they make it easier for indexers to join the network within a stable and secure system.

In this unit, we will cover the fundamentals of Indexer Operations and Containers:

- ***Lesson 1: Introduction to Indexer Operations***: Wallets, Multisigs, Faucets, Network Registration
    - Differences between hot and cold wallets, and between indexer wallets and operator wallets
    - The efficiency of multisigs wallets
    - How to utilize faucets, which are mechanisms to distribute tokens or cryptocurrencies for testing purposes, and their role in the indexing process
    - The basics of network registration
   
- ***Lesson 2: Getting Started with Containers***: Docker, docker-compose, Kubernetes, and Helm
    - The basics to Docker, a popular containerization platform 
    - How to use Docker Compose to compose multiple containers and create more complex indexer setups
    - An understanding of Kubernetes, an open-source container orchestration 
    - How to work with Helm, which is a package manager for Kubernetes that simplifies the deployment and management of applications

- ***Lesson 3: Lab 2 - Configure Your Indexing Stack***: Indexing stack and Gnosis RPC node 
    - Learn how to deploy The Graph indexing stack and connect to your Gnosis RPC (Remote Procedure Call) node to ensure a smooth data flow
     
By the end of this unit, students will have a foundation for indexer operations, containers, and the necessary configurations for a successful indexing stack deployment.
