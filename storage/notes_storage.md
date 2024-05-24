# Instance store

- can provide storage for an EC2 instance. This is a physical storage attached to the host computer.
- Data on this storage is destroyed once an Ec2 instance is stopped.

# Amazon elastic Block store (ebs)

- Virtual hard drive can be created
- These can be attached to an EC2 instance
- The data on EBS can be persisted beyond the life cycle of EC2 instance
- This is done by taking incremental snapshots of the data.
- Block storage Ex- video is broken down and stored in multiple blocks.

# Amazon simple storage Service (S3)

- Data is stored as objects.
- Each object consists of metadata, data and a key (unique identifier)
- Objects are stored in buckets
- Versioning of object is possible
- Can be used for static website hosting
- Different storage classes of S3 are available
- Life cycle policies can be created to move data from one tier another.
- Regionally distributed
