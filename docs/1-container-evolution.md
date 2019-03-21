# Evolution of containers and orchestrators

### [Back](../README.md)

#### Docker lies at the heart of the mass adoption and the excitement in the container space. As Malcom McLean revolutionized the physical shipping world in 1957 by creating a standardized shipping container, which is used today for everything from ice cube trays to automobiles, Linux containers are revolutionizing the software development world by making application environments portable and consistent across the infrastructure landscape. As an organization, Docker has taken the existing container technology to a new level by making it easy to implement and replicate across environments and providers.

| Containerization technology             | Release   | Orchestration technology                 | Release |
| --------------------------------------- | --------- | ---------------------------------------- | ------- |
| Solaris UNIX containers                 | 2004      | Kubernetes                               | 2015    |
| OpenVZ                                  | 2005      | Google Container Engine                  | 2015    |
| Linux kernel control groups and LXC     | 2007-2008 | Amazon EC2 Container Service             | 2015    |
| Docker                                  | 2013      | Mesosphere DC/OS (based on Apache Mesos) | 2016    |
| CoreOS rkt(Rocket)                      | 2014      | Docker Swarm                             | 2016    |
| Windows Hyper-V containers for docker   | 2016      | Azure Container Service                  | 2016    |
| cri-o                                   | 2017      | Azure Kubernetes Service                 | 2017    |
| Open Container Initiative(OCI) Standard | 2018      | Amazon EKS                               | 2018    |

### Currently container ecosystem still have:
- Containers adoption is still growing
- Rapid growth in container technologies has led to the need in standardization, integration and collaboration between container technologies
- Fragmentation: Docker, rkt, LXC/LXD, Hyper-V, VMWare, OpenVZ
- Cloud consumers wants to not be bound within concrete orchestration system, OS, architecture, vendor, cloud, etc.