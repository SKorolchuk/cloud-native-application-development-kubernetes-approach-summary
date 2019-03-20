# Application development, CI/CD and monitoring: Kubernetes approach
---------------
## Description
---------------
Summary notes about application and service development in Kubernetes: documentation, diagrams, guides, samples and bibliography

### `Note: Please, create issues or PR's with any copyright reference if I have missed links`

------------
## Contents
------------
    1. [Evolution of containers and orchestrators](docs/1-container-evolution.md)
    2. [Distributed complexity and isolation restrictions in containers](docs/2-distributed-complexity-in-containers.md)
    3. [Kubernetes goals and usage advantages](docs/3-kubernetes-goals.md)
    4. Common container patterns
    5. 12-Factor application principles
    6. Cloud Native application principles in Kubernetes
    7. Importance of development and QA/Production environment parity
    7. One-click start with Kubernetes dashboard as starting point
    8. Kubernetes architecture overview
       - Control plane definition
       - Simplified Kubernetes Application structure map
       - Kubectl, kube-proxy, kubeadm, kubelet, kubefed core utilities
       - Etcd High Available configuration store
       - API Server
       - Scheduler
       - Controller manager
       - cAdvisor, Heapster, metrics-server and state-metrics-server
       - Flannel, CNI and other Cluster network managers
       - Imperative vs. Declarative Kubernetes state management
       - Reconciliation Control Loop as core Kubernetes concept
       - Common workload resources
       - Common storage resources
       - RBAC and Access Control resources
       - Stateless vs. Stateful Kubernetes services
       - Kubernetes design patterns
       - Custom Resource Definition as extensibility point in Kubernetes
       - Operator SDK
    9. The hard choice: LoadBalancer Service or Ingress
       - LoadBalancer Service type
       - Nginx-Ingress, Ingress-Nginx
       - Traefik
       - Heptio Contour
       - HAProxy
    10. Kubernetes in Cloud
       - Landscape Overview
       - Cluster Federation and High Availability
    11. Kubernetes in development environment
        - Overview
        - Kubernetes as Docker Engine orchestrator
        - Minikube
        - Kubeadm multi-node cluster: Vagrant and DIND implementation
        - Kubespray
    12. Kubernetes On-Premise solutions
        - CoreOS Tectonic
        - OpenShift
        - Mesosphere DC/OS Kubernetes
    13. Simplifying k8s resource management
        - Helm
        - Draft
        - Skaffold
        - Kompose
    14. CI/CD pipeline setup in Cloud Native application development
        - Cloud-provided CI/CD overview
        - Spinnaker
        - GitLab CI/CD
    15. Improving cluster observability and resource provisioning
        - Cloud and paid solutions: Datadog, Sysdig, Azure Monitor, AWS CloudWatch, GKE Stackdriver
        - Application metrics and alerting with Prometheus and Grafana
        - Prometheus pull and push metrics collection strategies
        - Choice between classic Prometheus configuration and CRD resource controller
        - Service Mesh short overview
        - Service Tracing with Jaeger
    16. Cluster logs collection with EFK Stack(Fluentd, ElasticSearch, Kibana)
        - Log collection scheme
        - EFK stack deployment and integration
    17. Bibliography