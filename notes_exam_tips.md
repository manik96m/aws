# Learn the service categories

# Read AWS services whitepaper

# Topics

- Infrastructure
  - Regions, Availability zones, Local zones, Edge locations.
  - Management console - UI, CLI - Programmatic
- Migration
  - AWS cloud adoption framework, AWS well-architected architecture
- Compute technologies
  - EC2, instance types, pricing
  - Load balancer
  - Container Services (ECR, ECS, EKS)
  - Lambda
- Storage Technologies
  - EBS - Elastic Block Store (Individual storage for EC2 instance)
  - EFS - Elastic File System (Shared storage for multiple EC2 instances)
  - Instance Stores (Storage directly attached to EC2 instance)
  - S3
  - FSx
  - Elastic Disaster Recovery
- Content Delivery and Networking Services
  - CDN (Cloud front)
  - DNS (Amazon Route 53)
  - Cloud Accelerator
  - Amazon VPC (Virtual Private Cloud)
  - AWS Direct connect
  - AWS VPN
    - Site to Site VPN
    - Client VPN
- Database Services
  - Different Database Types
  - AWS Database Migration Service (DMS)
  - AWS Dynamo DB (NoSQL DB)
  - AWS MemoryDB for Redis (In-memory DB)
  - Neptune (Graph DB)

## AWS Global Accelerator

- Optimizes global application performance by routing user traffic through AWS's optimized network paths.
- Uses edge locations to find best pathway to regional endpoint.
- Provides consistent experience to global users.
