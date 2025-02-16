## AWS DynamoDB

- Serverless Database
- Table
- Data are stored as items
- Item has attributes
- Data is stored redundantly
- Rigid schema (Relational DB) can have
- Non-relational NoSQL database
- Spread across 3 geographically distinct data centres
- Items can be added and removed at any time
- Each item (Key) can have different attributes (values)
- Highly scalable
- Strongly consistent reads
- Stored on SSD storage

- Eventually consistent vs Strongly consistent reads
- Eventually consistent reads
  - Consistency across of all copies of data is usually reached within a second.
  - Repeating a read after a short time should return the updated data.
- Strongly consistent read
  - returns a result that reflects all writes that received a successful response prior to the read.

## DynamoDB Accelerator (DAX)

- Fully managed, highly scalable in-memory cache
- 10x performance improvement
- Reduces request time from ms to microseconds-even under load
- Compatible with DynamoDB API calls

## Acid with Dynamo DB

- Transactions can be enabled

## DynamoDB backups

- Full backups any time
- Zero impact on table performance
- Backup in same region

## Point in time recovery

- Protects against accidental writes or deletes
- Restores to any point in the last 35 days.
- Incremental backups
- Not enabled by default
- Latest restorable - 5 minutes in the past

## Streams??

- FIFO ordered, shard (stream of records)
- Time-ordered sequences of item-level changes in a table

## Global Tables

- Globally distributed applications
- Multi region redundancy for disaster recovery and high availability
- Done by creating replicas
- Uses DynamoDB streams, it needs to be enabled
  - by default enabled when needed
- Replication latency under 1 second
