## EC2 - Elastic Compute Cloud

- Server
- Provides access to virtual servers
- Manually manage the memory, CPU, hardware, processor for your instance.
- (Multitenancy) - Underlying hardware is shared between virtual machines(EC2s).
- Use when access to underlying OS is required

## Instance Type

- Varies by CPU, memory, ...
- Choose based on the need.
- 6 types
  - General, Compute optimized, memory optimized, accelerated computing, storage optimized, High performance computing(HPC) optimized

## Pricing

- On-Demand
- Savings (1 year or 3 year commitment)
- Reserved instances - for steady workflows (1 or 3 year commitment)
- Spot instances - Get instance when available (can be reclaimed at any time by AWS)
  - cheapest option
  - are instances running on the host (server)
- Dedicated hosts
  - are servers

## Scale on demand

- Start with only resources you need and design your architecture to respond to changing demand by scaling out or in.
  - Horizontal - add/removes EC2 instances
  - Vertical scaling - Upgrade EC2 instances
- Using Auto Scaler

## Elastic Load balancer

- Even load distribution across different EC2 instances
- Runs on region level
- Automatically scales in/out on demand.
- New instances informs ELB when they are available to take requests.
- ## Load Balancer types

## Connecting to EC2

- AWS management console
- EC2 instance connect
- Secure Shell(Linux) and Remote desktop protocol(Windows)
- AWS systems manager
