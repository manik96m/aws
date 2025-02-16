- AWS Supports different types of Relational database engines

## RDS

- Supports Multi-AZ

  - creates exact copy of your database in another AZ
  - Failover automatically done
  - Used for disaster recovery, not for improving performance

- OLTP (Online Transaction processing) vs OLAP (Online Analytical Processing)
  - OLTP - done using RDS
  - OLAP - done using Redshift or any other big data suitable database

## Read Replica

- Read-only copy of primary database.
- Used to boost performance
- Great for read-heavy workloads
- Requires automatic backup enabled
- upto 5 read replicas available

- Can be promoted to their own database.
  - this will break replication

## Relational Database Service

- Supports major database engines (ex - Oracle)
- Provides support for
  - Automated patching
  - Backups
  - Redundancy
  - Failover
  - Disaster recovery

## Amazon Aurora

- Managed database
- MySQL / PostgreSQL
- 5x better performance than MySQL
- 3x better performance than PostgreSQL
- Data replication (up to 15 replicas)
- Continuous backup to S3
- Point in time recovery
- Min 3 AZs
- 2 copies of data contained in each AZ

  - always have 6 copies minimum of your data

## Amazon Aurora Serverless

- On-demand auto-scaling config for MySQL and PostgreSQL compatibles editions of Amazon Aurora
- It starts-up, shuts down and scales capacity up/down based on application's needs
- for infrequent and cost effective access
- for variable workloads
- Aurora Capactity Units - Measurement on how your clusters scale
- Set Min and Max of ACUs for scaling requirements
- Allocated quickly by AWS-managed warm pools
