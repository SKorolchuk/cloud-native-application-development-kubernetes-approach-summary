# Application development, CI/CD, testing and monitoring: Kubernetes approach

## Description

Summary notes about application and service development in Kubernetes: documentation, diagrams, guides, samples and bibliography

```md
Warning: the docs materials are used references from 3rd party resources.
```

## `Note: Please, create issues or PR's with any copyright reference if I have missed links`

---

## [Bibliography and Reference list](docs/15-bibliography.md)

---

---

## Contents

---

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
10. The hard choice: LoadBalancer Service or Ingress(or both)
    - LoadBalancer Service type
    - Nginx-Ingress, Ingress-Nginx
    - Traefik
    - Heptio Contour
    - Kong
    - HAProxy
    - Heptio Gimbal
    - MetalLB
11. CSI providers. Distributed persistent storage options in Kubernetes:
    - Rook
    - Ceph
    - Gluster
    - Minio
12. Kubernetes in Cloud
    - Landscape Overview
    - Cluster Federation and High Availability
13. Kubernetes in development environment
    - Overview
    - Kubernetes as Docker Engine orchestrator
    - Garden
    - Minikube
    - Kubeadm Vagrant cluster
    - Kubeadm dind cluster
    - kind
    - Kubespray
14. Kubernetes On-Premise solutions
    - CoreOS Tectonic
    - OpenShift
    - Mirantis
    - Mesosphere DC/OS Kubernetes
    - Rancher
    - kubevirt
    - Kubernetes CDK
15. Kubernetes management tools
    - kubectl utility
    - VS Code extension for Kubernetes
    - kube-shell
    - kube-prompt
    - kubebox
    - kubefuse
    - Kubernetes Dashboard
    - Kubernetic
    - kubesec
    - skopeo
    - Heptio Velero
    - kubespy
    - helm-monitor
16. Connect Kubernetes cluster with your local machine
    - kubectl `proxy` and `port-forward`
    - Datawire Ambassador, Forge and Telepresence
    - kubefwd
    - Azure Dev Spaces
17. Simplifying k8s resource management
    - Helm
    - Ksonnet
    - Terraform
    - Pulumi
    - Kustomize
    - Skaffold
    - Kaniko, Makisu, buildah and buildkit
    - Gitkube
    - Kompose
    - Draft
    - Kubeapps
18. Serverless technologies compatible with Kubernetes
    - Kubeless
    - OpenFaaS
    - virtual-kubelet
19. Improve application management and delivery speed with Service Mesh
    - Service Mesh concepts
    - Istio
    - Istion namespace injection
    - Network configuration
    - Istio CRD overview
    - Security
    - Built-in netrics, distributed request tracing and mesh visualization
20. Extend Kubernetes cluster functionality with operators
    - Prometheus operator
    - Vault operator
    - Etcd operator
    - cert operator
    - DB operator
    - shell operator
    - flagger operator
21. CI/CD pipeline setup in Cloud Native application development
    - [Release strategies](https://github.com/ContainerSolutions/k8s-deployment-strategies)
    - IaaS abd GitOps princeples
    - Cloud-provided CI/CD overview
    - Azure DevOps
    - AWS CodeCommit, CodeBuild, CodeDeploy and CodePipeline
    - Google Cloud Build
    - WeaveWorks Weave Flux GitOps Operator
    - Jenkins X and Cloudbees
    - GoCD
    - Drone
    - Argo
    - Spinnaker
    - GitLab CI/CD
22. Improving cluster observability and resource provisioning by monitoring systems integration
    - Cloud and paid solutions: Datadog, Sysdig, Splunk, Azure Monitor, AWS CloudWatch, GKE Stackdriver
    - Application metrics and alerting with Prometheus and Grafana
    - Prometheus pull and push metrics collection strategies
    - Choice between classic Prometheus configuration and CRD resource controller
    - Service Tracing with Jaeger
23. Cluster logs collection
    - Elastic Stack(Fluentd/Logstash, ElasticSearch, Kibana)
    - Difference between logstash and fluentd
    - Log collection scheme
    - EFK stack deployment and integration
24. Integration, Acceptance, Conformance and Security testing in Kubernetes
    - Heptio `Sonobuoy` Diagnostic tool
    - `kube-monkey` Chaos testing tool
    - Brigade and Kashti
    - kube-bench
    - kube-hunter
    - PowerfulSeal
    - popeye
    - chaosblade
    - kube-score
