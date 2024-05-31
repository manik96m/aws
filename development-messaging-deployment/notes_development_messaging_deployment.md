## CI/CD

## AWS Development Tools

- CodeCommit - Central Code Repository
- CodeBuild - Build and Test Service
- CodeDeploy - Automated deployment
- CodePipeline - Automated CI/CD Pipeline

## AWS CloudShell

- Interact with AWS account using CLI from browser based shell.
- AWS CLI is already installed.

## AWS Cloud9

- It is IDE in browser.
- Comes pre-installed with AWS CLI, programming languages and commonly used tools.

## AWS CodeArtifact

- Artifact repository (Maven, npm, ...)

# Decoupling Application Components

# Messaging and Queueing

## Amazon SQS - Simple Queue Service

- Send/Store/Receive messages between software components at any volume.
- SQS is pull based, consumer pulls message when they are ready to process.
- Processing is async
- Queue Types
  - Standard Queues
    - Default Queue
    - Messages are delivered at least once
    - Best-effort ordering - messages are generally delivered in the same order they are sent.
  - FIFO Queues
    - Order is strictly preserved
    - Messages delivered once
    - No duplicate messages
- Polling Types - How frequently consumers poll
  - Short Polling - returns response immediately on poll even if message queue being polled is empty
  - Long Polling - queue doesn't respond until a message arrives or long poll times out

## Amazon SNS - Simple Notification Service

- Send/Store/Receive messages between software components or end users at any volume.
- Uses pub/sub model
- SMS text message or email (plain text)

## Message Queue

- Application don't need to directly communicate with each other.
- Helps decouple the architecture/applications.

## Simple Email Service (SES)

- Enable application richly formatted HTML emails

## Amazon Event Bridge

- Easily configure event driven systems
- Event are state changes
- Event bridge has rules and target
- Rules match the events
- Nd then route them to correct targets.
- Targets can be services like EC2, Lambda, SNS, ...
- Targets can take actions

- It can also help schedule events

## Step Functions

- Helps understand and visualize your serverless application.
- Can automatically trigger and track each step of a process (ex - checkout process of a product)
- Can log state of each step

## AWS Elastic Beanstalk

- Helps focus only on code and not on infrastructure
- Upload code and enable Elastic beanstalk
- It will automatically provision resources required
- Takes care of monitoring and auto scaling.

## X-Ray

- tool that helps developers analyze and debug distributed applications.
- it is part of Cloud Watch
- Analyze performance and health of distributed applications.
  -X-ray service map provides end-to-end view of service requests.
