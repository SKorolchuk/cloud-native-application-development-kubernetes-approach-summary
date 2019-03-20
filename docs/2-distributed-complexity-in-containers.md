# Distributed complexity and isolation restrictions in containers

### As the containerization and microservices evolves in an organization, they will soon need a strategy to maintain many containers and microservices. Some organizations will have hundreds or even thousands of containers running at the same time.

## Questions in containerized microservice architecture:

    - How will we automatically recover when a container fails?
    - Which upstream services are affected by such an outage?
    - How will we patch our applications with minimal downtime?
    - How will we scale up our containers and services as our traffic grows?
    - Networking and processing are also important concerns. Some processes are part of the same service and may benefit from proximity on the network. Databases, for example, may send large amounts of data to a particular microservice for processing.
    - How will we place containers near each other in our cluster?
    - Is there common data that needs to be accessed?
    - How will new services be discovered and made available to other systems?

### This is where orchestration tools such as Kubernetes offer the biggest value.

    `Kubernetes helps deal with resource utilization, high availability, updates, patching, networking, service discovery, monitoring and logging.`

    Google released the project as part of an effort to share their own infrastructure and technology advantage with the community. Google launches billions of containers a week in their infrastructure and has been using container technology for over a decade. Originally they were building a system named Borg, to schedule their vast quantities of workloads across their data center footprint. They took many of the lessons over the years and rewrote their existing data center management tool for wide adoption by the rest of the world. The result was the Kubernetes open source project.
