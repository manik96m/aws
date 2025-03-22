## ECR - Elastic Container Registry

- registry store, share and deploy container software
- ECS and EKS take container software from ECR to deploy applications to containers.
- Features ->
- Lifecycle Policies - To expire and remove unused images
- Image Scanning - Helps find vulnerabilities
  - Supports cross-region and cross-account sharing
  - Configured per repository and per region
- Cache Rules - caching public repos privately
- Tag Mutability - Prevents image tags from being overwritten

- Can use ECR images within your own container infra, ECS, ECR and Amazon Linux container locally

## ECS - Elastic Container Service

- ECS can manage containers
- fully managed and serverless using Fargate.
- supports Docker.

## EKS - Elastic Kubernetes Service

- fully managed open-source system
- supports Kubernetes

## EKS-D (Distro)

- Based on and used by EKS
- It is fully managed by you, unlike EKS
- Run anywhere

## EKS Anywhere

- way of running on-premise EKS
- Run clusters on prem
- Full lifecycle management of clusters
- Managed by customer

## ECS Anywhere

- Feature inside ECS
- Run and manage container applications on prem
- No orchestration needed
- COmpletely managed
- No ELB support
- There are some pre requirements to use ECS
- Auto Scaling Databases on Demand with Amazon Aurora Serverless
