## ECR - Elastic Container Registry

- store registry store, share and deploy container software
- ECS and EKS take container software from ECR to deploy applications in containers.

## ECS - Elastic Container Service

- fully managed and serverless using fargate
- supports docker

## EKS - Elastic Kubernetes Service

- fully managed open-source system
- supports kubernetes

# Fargate

- is used for workloads running for more than minutes. Otherwise, Lambda can be used.
- can only choose CPU size and memory size of your container,
  but not the processor or hardware
