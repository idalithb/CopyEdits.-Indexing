# Indexer Operations and Containers

Containers are a vital component of the work that Indexers perform within The Graph protocol. Therefore, it’s crucial to understand their functionality. 

The Graph relies on a decentralized network of indexers to provide the computational resources required to query and index data from various blockchains and containers enable the work of indexers. Containers provide a consistent and reliable environment for running the indexing software that is required by indexers. By packaging the indexing software and its dependencies into a container, indexers can easily deploy and run the software on their local machines or on cloud infrastructure. This not only makes Indexer's jobs more efficient, but it also reduces the barrier for new indexers who want to join the network.

Containers facilitate the mechanisms Indexers need to compute resources within The Graph. They provide a way to isolate the indexing software from the host operating system, which improves security and stability. Each container runs within its own isolated environment, so issues with the indexing software or its dependencies do not affect other parts of the system. This process reduces the risk of conflicts and makes it easier to manage and update the software. 

Overall, containers play a crucial role because they enable indexers to perform efficiently within the The Graph’s protocol, they provide a consistent and reliable environment for running indexing software, and they make it easier for indexers to join the network within a stable and secure system.

In this unit, we will cover the basics needed to better understand Indexer Operations and Containers:

- ***Lesson 1: Introduction to Indexer Operations***: Wallets, Multisigs, Faucets, Network Registration.
  - In this lesson you will explore:
    - The differences between hot and cold wallets, and the difference between indexer wallets and operator wallets
    - The efficiency of multisigs wallets and how they enable secure transactions
    - How to utilize faucets, mechanisms to distribute tokens or cryptocurrencies for testing purposes, and their role in the indexing process
    - The basics of network registration
   
- ***Lesson 2: Getting Started with Containers***: Docker, docker-compose, Kubernetes, and Helm. 
    - In this lesson you will learn:
      - The basics to Docker, a popular containerization platform
      - How to use Docker Compose to compose multiple containers and create more complex indexer setups
      - An understanding of Kubernetes, an open-source container orchestration
      - How to work with Helm, a package manager for Kubernetes that simplifies the deployment and management of applications

- ***Lesson 3: Lab 2 - Configure Your Indexing Stack***: Indexing stack and Gnosis RPC node 
    - In this lesson you will understand: 
      - How to deploy The Graph indexing stack and connect to your Gnosis RPC (Remote Procedure Call) node to ensure a smooth data flow
     
  Overall, this unit provides a foundation for indexer operations, containers, and the necessary configurations for a successful indexing stack deployment.
