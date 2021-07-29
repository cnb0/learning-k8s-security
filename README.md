# learning-k8s-security

```
Overview of the Kubernetes API and Security Features

      Access to HTTPS endpoints, Kubernetes API, nodes, and containers
      Kubernetes Authentication and Authorization features
      How Hackers Attack Your Cluster

How hackers find your etcd port, Kubernetes API, and other services
      How hackers execute code inside your container
      How hackers escalate their privileges
      Case study: How Tesla exposed its Kubernetes cluster
      Setting up Kubernetes

Choosing a distribution
Installing Kubernetes
Using Credentials and Secrets
      The credentials life cycle
      Understanding secrets
      Distributing credentials
      Controlling Access to the Kubernetes API

Encrypting API traffic with TLS
      Implementing authentication for API servers
      Implementing authorization for different roles
      Controlling User and Workload Capabilities

Understanding Kubernetes policies
      Limiting resource usage
      Limiting container privileges
      Limiting network access
      Controlling access to nodes

Separating workload access

Protecting Cluster Components
      Restricting access to etcd
      Disabling features
      Changing, removing and revoking credentials and tokens
      Securing Container Image

Managing Docker and Kubernetes images
      Building secure images
      Controlling Access to Cloud Resources

Understanding cloud platform metadata
Limiting permissions to cloud resources

Evaluating Third Party Integrations
    Minimizing the permissions granted to third party software
    Evaluating components that can create pods
    Establishing a Security Policy

Reviewing the existing security profile
    Creating a security model
    Cloud native security considerations
    Other best practices
    Encrypting Inactive Data

Encrypting backups
    Encrypting the entire disk
    Encrypting secret resources in etcd
    Monitoring Activity

Enabling audit logging
    Auditing and governing the software supply chain
    Subscribing to security alerts and updates
