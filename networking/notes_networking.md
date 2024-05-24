# Amazon Virtual private cloud

- isolated resources
- Public or private (subnets)
- Assign private ips to resources
- For public, assign Internet gateway
- For private, virtual private gateway

# Aws direct connect

- dedicated fiber connection from your data centre to aws

# Network Access Control List(ACL)

- Each packet sent (both inbound and outbound) to VPC is checked by Network access control list(ACL) for permissions.
- Default acl allow all inbound and outbound traffic.
- Network ACLs are stateless

# Security Groups

- Ec2 instance are assigned with security groups.
- Security group checks inbound traffic only.
- Security groups are stateful.
