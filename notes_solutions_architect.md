## S3

- Object based storage
- up to 5TB file size
- Server side encryption
- Object level ACLs
- Bucket policies to define actions allowed or denied
- Strong read-after-write consistency
  - Immediately receive latest version of an object
- Strong consistency for listing operation as well.

- URL for an object - https://{{BUCKET_NAME}}.s3.{{REGION}}.amazonaws.com/{{KEY-NAME}}

- Buckets are private by default

- Securing Bucket using Bucket Policies and ACLs

  - Change Block Public Access to control level of access to public
  - Edit Object ownership and enable ACLs for adding object level permissions
  - Then select an object, click Actions and click Make public using ACL to make that object publically accessible

- Static website hosting

  - Disable Block public access
  - Enable static website hosting for the bucket
  - Upload files
  - Permission -> Edit Bucket Policy -> Upload policy
  - Scales automatically with demand

- Versioning
  - Versioning cannot be disabled for a bucket but only suspended
  - Support MFA
  - can be integrated with lifecycle rules
  - Previous version are not public
  - Once an object is deleted, we can delete the Delete Marker to restore the
- Storage classes

  - S3 standard
    - High availability and durability
    - Data stored redundantly across multiple devices in multiple facilities (>= 3 AZs)
  - S3 standard infrequent access
    - rapid access
  - S3 one zone-infrequent access
    - long lived data
    - 20% lower cost
    - 99.5% availability
  - S3 intelligent tiering

    - automatically move data between frequent and infrequent types based on usage

  - Glacier options

    - pay when you access
    - used for archiving data
    - cheap
    - infrequently accessed data

  - Glacier instant retrieval
    - instant retrieval of data
  - Glacier flexible retrieval
    - can be min or up to 12 hours to access data
  - Glacier deep archive
    - Standard retrieval time 12 hours
    - Bulk retrieval up to 48 hours
    - cheapest

- Lifecycle Management

  - Automates moving of objects between different storage tiers, to maximize cost effectiveness.
  - Ex - moving from S3 standard, to IA, to Glacier
  - It can be combined with versioning, to move different versions to different tiers.

- S3 object lock
  - used to store object using a write once, read many (WORM) model.
  - Governance mode
    - users cant override or delete an object version or alter its lock settings unless they have special permissions.
  - Compliance mode
    - Protected object version cant be overwritten or deleted by ANY user.
    - Retention mode and period set cannot be changed.
  - Retention period
    - protects an object version for a fixed amount of time.
    - after the retention period expires the object version can be overwritten or deleted unless a legal hold is placed.
  - Legal hold
    - prevents overriding and deletion of an object version.
  - Glacier Vault Lock
    - easily deploy and enforce compliance controls for individual S3 vaults with a vault lock policy.

## EC2

- Pricing Options
- Security Groups
- AWS Command Line
  - aws configure to configure user credentials
  - used to access other resources from EC2
  - Use secret access key (password to access CLI) to assign access to CLI for a user
- Bootstrap Scripts
- EC2 Metadata and User Data
- Networking with EC2
- Placement Groups
- Dedicated Hosts
- Spot instances
- vCenter with VMware
- AWS Outposts

## IAM

- User
- Group
- Roles

## Database

- RDS
  - OLTP vs OLAP
  - RDS Multi AZ
  - usecase of Multi AZ
  - Read Replica
- Amazon Aurora
- DynamoDB
  - ACID with DynamoDB
- ACID Properties

- MongoDB / Amazon DocumentDB
  - Operating MongoDB Compatible databases in AmazonDB
- Apache Cassandra workloads with Amazon Keyspaces
- Graph databases using Amazon Neptune
- Leveraging Amazon Quantum Ledger Database (QLDB) for Ledger Databases
- Analyzing time-series data with Amazon TimeStream

## Serverless Computing

- Lambda
- AWS Serverless Application Repository
- Container
- ECS
- EKS
- Fargate
- Amazon EventBridge or CloudWatch Events
- Docker images in ECR (Elastic Container Registry)
- Using Open Source Kubernetes in Amazon EKS Distro
- Orchestrating Containers outside AWS using EKS Anywhere and ECS Anywhere
- AWS X-ray for application insights
- Deploying GraphQL Interfaces in AWS AppSync

## Route 53
