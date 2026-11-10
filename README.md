# CST8915 Lab 6: Deploy Algonquin Pet Store to Azure Kubernetes Service (AKS)

**Student Name**: Jane Akinyi Odhiambo<br/>
**Student ID**: 041268593<br/>
**Course**: CST8915 Full-stack Cloud-native Development<br/>
**Semester**: Fall 2026

---

## Demo Video

[Lab 6 Demo Video](https://youtu.be/SUg7qg22YCU)

---

## Overview

In this lab, I learned how to deploy and manage containerized microservices using Azure Kubernetes Service (AKS). The goal was to deploy the Algonquin Pet Store application to an AKS cluster, manage application resources using kubectl, expose services through an external IP address, and explore Kubernetes features such as scaling.

---

## Lab Objectives

- Understand the fundamentals of Azure Kubernetes Service (AKS).
- Install kubectl.
- Create an Azure Kubernetes Cluster (AKS).
- Deploy the Algonquin Pet Store Application using algonquin-pet-store-all-in-one.yaml file.

---

## Technologies Used

- Microsoft Azure
- Azure Kubernetes Service (AKS)
- Kubernetes
- kubectl
- Azure CLI
- RabbitMQ

---

## Reflection Questions

### 1. What is one advantage of using K8s over Docker Compose to manage microservices?

Kubernetes offers automated container orchestration, thus allowing applications to scale, recover from failures, and spread workloads across nodes.

---

### 2. How does NGINX reverse proxy routing allow services to use the same external IP address?

NGINX routes incoming requests to the appropriate backend service. For example, in this lab, `/products` sends requests to the Products service, `/orders` sends requests to the Orders service, and `/rabbitmq` sends requests to the RabbitMQ dashboard, thus allowing many services to share one external IP address.

---
