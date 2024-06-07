## Capital Expenditure (CapEx)

- Upfront purchases toward fixed assets.

## Operational Expenses (OpEx)

- funds used to run day-to-day operations.

## AWS regions

- AWS provides high availability using multiple AWS regions.
- Each region is isolated from each other.
- Unless specified data from one AWS region will not move to another AWS region.
- Some services like elastic load balancing are regionally scoped.
- Considerations before choosing an AWS region
  - Compliance
  - User proximity
  - Available features in that region
  - Pricing

## Availability zones

- One AWS region can have multiple availability zones that are isolated.
- AZ is made of multiple data centers
- Allow for high availability
  - by replicating service across AZs

## Latency

- Latency is amount of time a request takes to respond.
  - Low latency is good

## Local Zones

- Local zones place AWS services closer to end-users.
- These are extensions of AWS regions.

## Edge locations

- can help reduce latency.
- They don't launch resources but help cache content for faster delivery to users.
- Used for -
  - CDN - Amazon cloud front
  - DNS - amazon route 53

## CDN (Cloud Front)

- Caching copies of data closer to customers
- For speed, reliability, global reach
- Cloud Front caches content in edge locations
- Uses AWS Shield for Ddos attacks
- Used for streaming videos, traffic spikes, detailed analytics

## DNS (Amazon Route 53)

- Human readable name to IP address.
- Helps with traffic routing.
- Can perform health checks as well.
  - and redirect requests accordingly.

## Aws Outposts - isolated data centre

- Installing mini AWS region inside your own data centre.

## Lightsail

- used to quickly launch small projects.

## Batch

- Process large workload in small batches

## Wavelength

- Allows users to reach application servers without leaving 5G mobile network.

## Provisioning resources

- Management console
- CLI - calling apis to provision
  - Programmatic access
- SDK
- Cloud formation - IAS
  - provision using template
  - Cloud provision calls requires apis
