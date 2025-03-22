# Fargate

- is used for workloads running for more than 15 minutes. Otherwise, Lambda can be used.
- can only choose CPU size and memory size of your container,
  but not the processor or hardware
- Requires use of ECS or EKS
- Choose fargate for consistent workloads

## EC2 vs Fargate

- EC2 - Customer is responsible for underlying OS
- EC2 pricing model
- For long running containers
- Multiple containers can share same host
- Capable of mounting EFS file system for persistent, shared storage

- Fargate - No OS access
- Pay based on resources allocated and time ran
- Short running tasks
- Isolated environments per container
- Also capable of mounting EFS file system for persistent, shared storage
