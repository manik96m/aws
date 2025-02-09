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

## Pricing (4 Options)

- For Savings (1 year or 3 year commitment)

1. On-Demand

- No upfront payment
- useful for short term workloads

2. Reserved instances - for steady workflows (1 or 3 year commitment)

- Predictable usage
- Can make upfront payments
- Can save up to 72% off the on-demand price
- Operate at regional level

3. Spot instances - Get instance when available (can be reclaimed at any time by AWS)

- cheapest option (up to 90% discount)
- are instances running on the host (server)

4. Dedicated hosts

- are servers
- might be needed for compliance
- can be on-demand or reserved
- Solving Licensing Issues with dedicated hosts
  - Any question that talks about special licensing requirements.

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

## Load Balancer types (ToDo)

## Connecting to EC2

- AWS management console
- EC2 instance connect
- Secure Shell(Linux) and Remote desktop protocol(Windows)
- AWS systems manager

## Bootstrap Scripts

- Script that runs when the instance first runs.

## EC2 Metadata and User Data

- Metadata - Data about EC2 instance
- User Data is simply bootstrap scripts
- We can use bootstrap scripts (user data) to access metadata

## Networking with EC2

- Three different types of virtual networking cards can be attached to EC2 instance

1. ENI (Elastic Network Interface)

- basic day-to-day networking
- Private and Public IPv4 address
- Many IPv6 addresses
- MAC addresses
- 1 or more security groups

2. EN (Enhanced Networking)

- Uses single root I/O virtualization to provide high performance
- Networking between 10 Gbps - 100 Gbps
- Higher bandwidth
- High Packet Per Second
- Elastic Network Adapter for speeds up to 100 Gbps for supported instance types
- Intel Virtual Function Interface for speeds up to 10 Gbps for older instances

3. EFA (Elastic Fabric Adapter)

- Accelerates High Performance Computing and machine learning applications.
- EFA can use OS-BYPASS
  - Enables HPC and machine learning applications Bypass OS kernel and communicate directly with EFA device.
  - Makes it a lot faster with lower latency

## Placement Groups

- 3 types
- Cant merge Placement groups
- Existence instance can be moved to a placement group but it needs to be stopped first.

1. Cluster

- Grouping of instance within a single AZ.
- For applications that need low network latency, high network throughput or both
- Available for only certain instance types
- AWS recommends homogenous instances within a cluster

2. Spread

- Instances are placed on distinct underlying hardware.
- Used for individual instances.

3. Partition

- Each partition placement group has its own set of racks.
- Each rack has its own network and power source.
- No two partitions within a placement group share same racks, allowing to isolate impact of hardware failure within your application.
- Used for multiple instances.

## Timing workloads using Spot instances

- Used when application is stateless and fault tolerant.
- Need to decide the maximum spot price.
- Instance will be provisioned when Spot price is below your maximum Spot Price
- Hourly spot price varies based on capacity and region.
- If spot price goes above your maximum, then you have 2 minutes to decide whether to stop (can be resumed) or terminate.
- How to cancel spot instance under persistent spot request?

  - Cancel Spot request
  - Terminate instances

- Spot Fleet
  - Collection of spot instances and optionally On-demand instances

## Deploying vCenter in AWS with VMware Cloud

- VMware is used for private cloud deployments.
- Can be used for
  - Hybrid cloud
  - Cloud Migration
  - Disaster Recovery
  - Leverage AWS
- Deployment
  - Runs on dedicated hardware hosted in AWS
