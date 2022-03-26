# Kubernetes training

[![CI](https://github.com/devpro/kubernetes-training/actions/workflows/ci.yml/badge.svg)](https://github.com/devpro/kubernetes-training/actions/workflows/ci.yml)

Welcome to this learning space!

## Introduction

You'll find here training exercises to **learn and practice Kubernetes from Zero**.

:bulb: Feel free to contribute, by sharing it, creating Issues and submitting Pull Requests!

## Requirements

### Terminal

We'll mainly execute commands from a terminal window. Make sure you chose one you are familiar with.

### kubectl

[`kubectl`](https://kubernetes.io/docs/reference/kubectl/) is the Kubernetes Command Line Interface tool.
It must be installed prior to any other action.

Follow the procedure from the [official documentation](https://kubernetes.io/docs/tasks/tools/#kubectl).

Example: [Install kubectl on Ubuntu](./samples/ubuntu-based-configuration.md#kubectl)

### (Optional) IDE

We are going to create and update YAML files. Some people may be confortable in using IDE, like Visual Studio Code, to do so.

## Learning paths

### Discovery tour

* [1. Components](./docs/1-components/components.md)
* [2. Setup](./docs/2-setup/setup.md)
* [3. Dashboard](./docs/3-dashboard/dashboard.md)
* [4. Deployments](./docs/4-deployments/deployments.md)
* [5. Services](./docs/5-services/services.md)
* Ingresses
* Operators

### Administration tour

* Statefull with MongoDB operator
* Installation with kubeadm
* Managed instances with Azure Kubernetes Service (AKS)
* Package management with Helm
* Secret management with Bitnami Sealed Secrets
* Certificate automated creation with cert-manager and Let's Encrypt
* GitOps with ArgoCD
* Observability with OpenTelemetry, Prometheus and Grafana
