# Importance of development and QA/Production environment parity

### [Back](../README.md)

## <i>Keep development, staging and production environment as similar as possible<i>

#### <i style="color:#4488ff">Situations when code `works for me!` on your workstation, but doesn’t start on your team mate’s without extra work has dramatic impact on team performance. The worst case scenario is that this code is deployed and doesn’t work in production, taking the service down. This friction can add up to significant time over the lifecycle of software. In the above scenario you are spending precious time futzing with your dev environment, and DevOps engineers are getting paged because the service is down.
</i>

Capable solutions:
- <p style="color:#f0584f">Stop using locally deployable infrastructure for development process. Use instead containers or services exposed from cloud. A lot of Kubernetes tools created to break the line between developer and cloud environment.</p>
- <p style="color:#f0584f">Use the same common deployment resources and strategies for Kubernetes in all environments.</p>
- <p style="color:#f0584f">Use image registries for development and CI/CD processes.</p>
- <p style="color:#f0584f">Use Helm charts for Kubernetes resource packaging and release versioning. Also Helm public repositories could help with fast and well-configured services and infrastructure setup.</p>
