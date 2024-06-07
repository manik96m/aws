## AWS Identity and Access Management (IAM)

- Used for Access Control
- IAM user
  - Explicitly allow access to resources.
  - New IAM users come with 0 permissions.
  - IAM user is an identity that you create in AWS.
  - consists of name and credentials.
- IAM policy
  - describes the permissions granted to a user / group.
- IAM group
  - can be created to share permissions across multiple users.
  - easier to manage same permissions that are required for multiple users.
- IAM roles
  - Using roles, permissions can be assumed for temporary amounts of time.
  - Roles can be granted to
    - AWS resources
    - Users
    - External identities
    - Applications
    - AWS services

## AWS Organizations

- Used to consolidate and manage multiple AWS accounts. (common for organizations)
- Centralized management of AWS accounts.
- Service Control Policies - Permissions are controlled using Service Control Policies (SCPs).
  - these can be applied to individual member account or an organizational unit.
  - it impacts all the IAM users, groups, and roles within an account (including root user).
- Organizational units - Accounts can be grouped into organizational units (OUs)
  - makes it easier to manage accounts with similar business or security requirements
  - easily grant access to the services and resources required by an Organization unit.
- Consolidated billing
- Hierarchical grouping of account

## IAM Identity Center

- Using federated entity
- Using 3rd party identity provider to provide access

## System Manager Parameter Store

- Secrets like username, password, ...
- it can be accessed using IAM roles

## Secrets Manager

- Ability to rotate secrets

## AWS Network Firewall

- Filter based on origin
- can define rules to inspect traffic within VPCs

## AWS WAF (Web Application Firewall)

- protects against common exploits
- like SQL injection or cross-site scripting

## AWS Shield

- Protects from DDoS (Denial of Service)

## Amazon GuardDuty

- checks logs across application and detect threats

## Amazon Detective

- Helps investigate security events that have already happened

## Amazon Inspector

- Scans for software vulnerabilities and network exposure
