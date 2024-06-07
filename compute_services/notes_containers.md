## ECR - Elastic Container Registry

- registry store, share and deploy container software
- ECS and EKS take container software from ECR to deploy applications to containers.

## ECS - Elastic Container Service

- fully managed and serverless using Fargate.
- supports Docker.

## EKS - Elastic Kubernetes Service

- fully managed open-source system
- supports Kubernetes

# Fargate

- is used for workloads running for more than 15 minutes. Otherwise, Lambda can be used.
- can only choose CPU size and memory size of your container,
  but not the processor or hardware
