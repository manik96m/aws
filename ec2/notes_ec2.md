## EC2 - Elastic Compute Cloud

- Server
- Provides access to virtual servers
- (Multitenancy) - Underlying hardware is shared between virtual machines(EC2s).
- Use when access to underlying OS is required

## Instance Type

- Varies by CPU, memory, ...
- Choose based on the need.
- General, Compute optimized, memory optimized, accelerated computing, storage optimized

## Pricing

- On-Demand
- Savings (1 year or 3 year commitment)
- Reserved instances - for steady workflows (1 or 3 year commitment)
- Spot instances - Get instance when available (can be reclaimed at any time by AWS)
- Dedicated hosts

## Scale on demand

- Start with only resources you need and design your architecture to respond to changing demand by scaling out or in.
- Using Auto Scaler

## Elastic Load balancer

- Even load distribution across different EC2 instances
- Runs on region level
- Automatically scales in/out on demand.
- New instances informs ELB when they are available to take requests.

## Messaging and Queueing

- Amazon SQS - Simple Queue Service
  - Send/Store/Receive messages between software components at any volume.
- Amazon SNS - Simple Notification Service
  - Send/Store/Receive messages between software components or end users at any volume.
  - Uses pub/sub model
- Message Queue
  - Application don't need to directly communicate with each other.
  - Helps decouple the architecture/applications.
