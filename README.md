# Foyer Projet Infrastructure Provisionning & Application Deployment Deployment

This repository contains Terraform configurations for deploying and managing a robust infrastructure for the **Foyer Project**. Additionally, it includes Kubernetes manifests for deploying the application to an Azure Kubernetes Service (AKS) cluster.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Architecture](#architecture)
- [Prerequisites](#Prerequisites)

---

## Overview

This project automates the provisioning of cloud infrastructure using **Terraform**, focusing on scalability, security, and maintainability. It also includes the deployment of the **Foyer application**, which is built with separate backend and frontend components.

- **Backend**: [Foyer Backend Repository](https://github.com/OnsHanafi/Foyer) (Spring Boot API)
- **Frontend**: [Foyer Frontend Repository](https://github.com/OnsHanafi/frontFoyer) (Angular Application)

---

## Features

- **Azure Kubernetes Service (AKS)**: A managed Kubernetes cluster for deploying containerized applications.
- **Networking**: Secure virtual network (vNet) and subnets for isolating resources.
- **RBAC**: Secure authentication for Kubernetes workloads using Role Base Access.
- **Ingress Controller**: External ingress with TLS/SSL certificates managed by Cert-Manager.
- **Storage**: Persistent storage for applications deployed in the AKS cluster.
- **Application Deployment**: Kubernetes manifests for deploying the Foyer application, including services and ingress configurations.

---

## Architecture

The infrastructure and application deployment are designed with the following components:

1. **Resource Group**: Centralized resource management for Azure resources.
2. **Virtual Network (vNet) and Subnets**: Isolated network architecture.
3. **AKS Cluster**: Configured with workload identity and spot node pools for cost optimization.
4. **Ingress Controller**: Deployed with Cert-Manager for managing TLS certificates.
5. **Application**: Deployed using Kubernetes manifests & RBAC to the AKS cluster.

---

### Prerequisites

- Terraform v1.5 or later
- Azure CLI authenticated to your Azure subscription
- kubectl configured for your AKS cluster
- Git installed on your local machine


