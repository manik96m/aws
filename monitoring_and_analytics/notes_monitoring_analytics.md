# Cloud Watch

- Monitor aws infrastructure
- Works by tracking and monitoring metrics
- Metrics - variables tied to resources
- Cloud watch alarm - can be triggered based on a metric. It can perform actions if a metric is above or below a certain value.
- Can be integrated with SNS to send messages
- Aggregating metrics using dashboard

# Cloud trail

- API auditing tool
- Every request to AWS gets logged to cloud trail with senders info and some other info.
- Information includes the identity of the API caller, the time of the API call, the source IP address of the API caller, and more
- Complete history of user activity and API calls for your applications and resources.
- These information includes requests to provision, manage and configure aws resources.
- Cloud trail insights - can help detect unusual api activities in aws account.

# AWS trusted advisor

- Can help evaluate resources.
- Can help with
  - Cost optimization
  - Performance
  - Security
  - Fault Tolerance
  - Service limits
