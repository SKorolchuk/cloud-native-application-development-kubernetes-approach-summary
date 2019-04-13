# Application development, CI/CD, testing and monitoring: Kubernetes approach

## Description

Summary notes about application and service development in Kubernetes: documentation, diagrams, guides, samples and bibliography

```md
Warning: the docs materials are used references from 3rd party resources.
```

## `Note: Please, create issues or PR's with any copyright reference if I have missed links`

------------

## Contents

------------

1. [Evolution of containers and orchestrators](docs/1-container-evolution.md)
2. [Distributed complexity and isolation restrictions in containers](docs/2-distributed-complexity-in-containers.md)
3. [Kubernetes goals and usage advantages](docs/3-kubernetes-goals.md)
4. [Common container patterns](docs/4-common-patterns.md)
5. [12-Factor application principles](docs/5-12-factor-app-principles.md)
6. [Cloud Native application principles in Kubernetes](docs/6-cloud-native-principles-in-k8s.md)
7. [Importance of development and QA/Production environment parity](docs/7-qa-prod-env-parity.md)
8. [`One-click` start with Kubernetes dashboard as starting learning point](docs/8-k8s-dashboard-setup.md)
9. [Kubernetes architecture high level overview](docs/9-high-level-k8s-arch.md)
    - [Control plane definition](docs/9-1-control-plane-definition.md)
    - [Simplified Kubernetes Application structure map](docs/9-2-k8s-sample-application-arch.md)
    - [Kubectl, kube-proxy, kubeadm, kubelet, kubefed core utilities](docs/9-3-k8s-core-utilities.md)
    - [Etcd High Available configuration store](docs/9-4-k8s-etcd.md)
    - [API Server](docs/9-5-k8s-api-server.md)
    - [Scheduler](docs/9-6-k8s-scheduler.md)
    - [Controller manager](docs/9-7-k8s-controller-manager.md)
    - [Cloud Controller manager](docs/9-8-k8s-cloud-controller-manager.md)
    - [cAdvisor, Heapster, metrics-server and state-metrics-server](docs/9-9-k8s-metrics-sybsystem.md)
    - [Flannel, CNI and other Cluster network managers](docs/9-10-k8s-network-layer.md)
    - Imperative vs. Declarative Kubernetes state management
    - Reconciliation Control Loop as core Kubernetes concept
    - Common workload resources
    - Common storage resources
    - RBAC and Access Control resources
    - Stateless vs. Stateful Kubernetes services
    - Kubernetes design patterns
    - Custom Resource Definition as extensibility point in Kubernetes
    - Operator SDK
10. The hard choice: LoadBalancer Service or Ingress
    - LoadBalancer Service type
    - Nginx-Ingress, Ingress-Nginx
    - Traefik
    - Heptio Contour
    - HAProxy
11. Kubernetes in Cloud
     - Landscape Overview
     - Cluster Federation and High Availability
12. Kubernetes in development environment
      - Overview
      - Kubernetes as Docker Engine orchestrator
      - Minikube
      - Kubeadm multi-node cluster: Vagrant and DIND implementation
      - Kubespray
13. Kubernetes On-Premise solutions
      - CoreOS Tectonic
      - OpenShift
      - Mesosphere DC/OS Kubernetes
      - Rancher
14. Kubernetes management tools
      - kubectl utility
      - VS Code extension for Kubernetes
      - kube-shell 
      - Kubernetes Dashboard
15. Connect Kubernetes cluster with your local machine
      - kubectl `proxy` and `port-forward`
      - Datawire Ambassador and Telepresence
16. Simplifying k8s resource management
      - Helm
      - Draft
      - Skaffold
      - Kompose
17. CI/CD pipeline setup in Cloud Native application development
      - IaaS abd GitOps princeples  
      - Cloud-provided CI/CD overview
      - Azure DevOps
      - AWS CodeCommit, CodeBuild, CodeDeploy and CodePipeline
      - Google Cloud Build
      - WeaveWorks Weave Flux GitOps Operator
      - Jenkins X and Cloudbees
      - GoCD
      - Drone
      - Spinnaker
      - GitLab CI/CD
18. Improving cluster observability and resource provisioning by monitoring systems integration
      - Cloud and paid solutions: Datadog, Sysdig, Splunk, Azure Monitor, AWS CloudWatch, GKE Stackdriver
      - Application metrics and alerting with Prometheus and Grafana
      - Prometheus pull and push metrics collection strategies
      - Choice between classic Prometheus configuration and CRD resource controller
      - Service Mesh short overview
      - Service Tracing with Jaeger
19. Cluster logs collection
      - Elastic Stack(Fluentd/Logstash, ElasticSearch, Kibana)
      - Difference between logstash and fluentd
      - Log collection scheme
      - EFK stack deployment and integration
20. Integration, Acceptance, Conformance and Security testing in Kubernetes
      - Heptio `Sonobuoy` Diagnostic tool
      - `kube-monkey` Chaos testing tool
21. [Bibliography](docs/15-bibliography.md)
