# Cloud Watch

- Monitor aws infrastructure
- Works by tracking and monitoring metrics
- Track Metrics
  - variables tied to resources
  - derived from logs
- Cloud watch alarm - can be triggered based on a metric. It can perform actions if a metric is above or below a certain value.
- Can be integrated with SNS to send messages
- Aggregating metrics using dashboard
- Log Streams - Each separate source of logs makes up a separate log stream
- Log Group
  - It is group of log streams that share same retention, monitoring and access control settings.
  - By default, data in log groups is stored indefinitely and it can be expensive.

# Cloud trail

- API auditing tool
- Every request to AWS gets logged to cloud trail with senders info and some other info.
- Information includes the identity of the API caller, the time of the API call, the source IP address of the API caller, and more
- Complete history of user activity and API calls for your applications and resources.
- These information includes requests to provision, manage and configure aws resources.
- Cloud trail insights - can help detect unusual api activities in aws account.

# AWS trusted advisor

- Can help evaluate resources.
- Nd provide suggestions for best practices.
- Can help with
  - Cost optimization
  - Performance
  - Security
  - Fault Tolerance
  - Service limits

# Systems Manager

- Group resources on AWS, on prem or on other cloud platforms.
- Take automated actions on resources groups.

# AWS health dashboard

- helps track health of resources

# AWS config

- used for auditing data
- pre-defined recommendations or create custom rules
- can detect non-compliant resources

# Audit manager

- Centralize audit data from AWS config and security services
- find root cause of non compliance and generate reports
