## Lambda

- Serverless
- Management of server is taken care of
- run code without needing to provision or manage servers.
- Uses triggers to execute lambda functions
- Each invocation run time < 15 mins

## New Lambda function

- When a new lambda function is created, it also creates an execution role for your function.
- An execution role is an AWS Identity and Access Management (IAM) role that grants a Lambda function permission to access AWS services and resources.
- For your function, the role that Lambda creates grants basic permissions to write to CloudWatch Logs.

## Lambda Function execution

- Handler function is the entry point of lambda function.

## Function Params

- Event

  - contains JSON formatted data.
  - If your function is invoked by another AWS service, the event object contains information about the event that caused the invocation.

- Context
  - context object contains information about the function invocation and execution environment.

## Lambda Function Cleanup

- Delete Lambda Function
- Delete log group
- Delete execution role
- This can automated using CloudFormation and CLI

## Logging

- [Nodejs Logging](https://docs.aws.amazon.com/lambda/latest/dg/nodejs-logging.html)
