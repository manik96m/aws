## Instance store

- can provide storage for an EC2 instance. This is a physical storage attached to the host computer.
- Data on this storage is destroyed once an EC2 instance is stopped.
- comes free with the instance.

## Amazon Elastic Block Store (EBS)

- Block storage Ex- video is broken down and stored in multiple blocks.
- Virtual hard drive can be created
- These can be attached to an EC2 instance
- The data on EBS can be persisted beyond the life cycle of EC2 instance
- This is done by taking incremental snapshots of the data.
- Encrypted at rest and in transit.
- EBS Volumes
  - SSD-backed
    - General Purpose
    - Provisioned IOPS
  - HDD-backed
    - Throughput Optimized HDD
    - Cold HDD

## Elastic File System

- Managed shared file system
- No need to worry about storage and backups
- Can scale up and down as needed
- Can be attached to an EC2 instance (need to in the same region)
- Multiple EC2 can read/write simultaneously

## Amazon simple storage Service (S3)

- Data is stored as objects.
- Each object consists of metadata, data and a key (unique identifier)
- Objects are stored in buckets
- Versioning of object is possible
- Can be used for static website hosting
- Life cycle policies can be created to move data from one tier another.
- Regionally distributed
- S3 buckets are encrypted by default.
- Security using bucket policies (User access) and Access Control List (ACL).
- Different storage classes of S3 are available
  - Standard
  - Intelligent Tiering
    - Automatically moves data between 2 access tiers based on access patterns.
  - Standard Infrequent Access
    - Data accessed less frequently but needs RAPID access.
  - One Zone-Infrequent Access
    - Stored in one Availability zone and is cost-effective
    - can be used for backups
  - Glacier Instant Retrieval
    - Archive storage for data not frequently accessed
    - But provides INSTANT retrieval
  - Glacier Flexible Retrieval
    - Archive Storage
    - Access is not immediate and can take some time
  - Glacier Deep Archive
    - Archive Storage
    - Used for compliance
    - Slow access, can take up to 12 hours

## FSx

- fully managed
- Windows File System

## Elastic Disaster Recovery

- Minimize downtime and data loss.
- Quick Recovery Times
- Cost Effective

## AWS Storage Gateway

- Connect onsite data storage to AWS cloud services.
- Cost efficient
- Encrypted data transfer
- can be used for
  - for offsite backup
  - Disaster recovery
- Types
  - S3 File Gateway
  - Volume Gateway - Block Storage volumes
  - Tape Gateway - For archiving data
  - FSx File Gateway - Extends on-premises file systems

## AWS backup

- Manage backups across services
- Automatic backup scheduling
- Encrypted
- Cross region account backup
