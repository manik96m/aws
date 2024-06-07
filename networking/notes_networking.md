## Amazon Virtual private cloud

- isolated resources
- Public or private (subnets)
- Assign private ips to resources
- For public, assign Internet gateway
- For private, virtual private gateway

## Internet Gateway

- Responsible for routing outgoing requests and incoming traffic
- It is attached to VPC

## Route Table

- Have entries(routes) that determine where network traffic from your subnets should go.
- Each subnet must be associated with a route table

## Aws direct connect

- dedicated fiber connection from your data centre to aws
- used for
  - large scale data transfer
  - Consistent performance
  - Sensitive data

## AWS VPN

- Site to Site VPN
  - For Data center
  - Between your data center and AWS
- Client VPN
  - For individual access
  - Secure access to AWS resources or your private network from any location.

## Network Access Control List(ACL)

- Each packet sent (both inbound and outbound) to VPC is checked by Network access control list(ACL) for permissions.
- Default ACL ALLOW all inbound and outbound traffic.
- Network ACLs are stateless
- Operate at subnet level.

## Security Groups

- Instance are assigned with security groups (Ex - EC2 instance)
- Security group checks inbound traffic only.
  - Security groups are stateful.

VPC -> Subnets -> Route Tables -> Internet Gateway
