# Evoli

Lulu Dans Ma Rue technical test that a candidate need to do for the DevOps / Fullstack developer position

## Goal

### 1st part (est. half a day ~ day)

The goal of this technical is divided in two parts:

1st part is to deploy a Kubernetes cluster from scratch with *Terraform* to Google Cloud Platform. The Kubernetes cluster should at least have these third parties services deployed with the tool of your choice .e.g: Helm, Kustomize. 

To deploy the Kubernetes cluster you can use the IaC tool of your choice .e.g: Terraform, Ansible, Pulumi etc...

- ArgoCD
- Prometheus
- Grafana

Tips:

- Use preemptible nodes to reduce the cost
- Namespace could be useful
- Use the machine type n2d-standard-2 

### 2nd part (est. 1 day)

The 2nd part of this test required you to configure a small app to deploy it in the Kubernetes cluster by using a CI/CD pipeline in combination of using the ArgoCD tool to implement a GitOps deployment process.

- To create the pipeline, please *fork* this repository
- Create your CI/CD pipeline by following this diagram

Below is the description of the pipeline

### Dev branch

The dev branch represent the `preproduction` environment

When a developer is merging a PR to the Dev branch. The dev branch should:
- Run unit test
- Build a docker image
- Deploy the **pre-production app** in the Kubernetes cluster by using ArgoCD

### Main branch

The main branch represent the `production` environment

When a developer is merging a PR to the Dev branch. The dev branch should:
- Run unit test
- Build a docker image
- Deploy the **production app** in the Kubernetes cluster by using ArgoCD
