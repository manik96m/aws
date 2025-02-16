## Event Bridge

- Serverless event bus
- Allows to pass events from a source to an endpoint.
- Events - Recorded change in an AWS environment.
- Rules - Criteria to match incoming events and send them to appropriate targets.
- Event Bus - Router that receives events and delivers them to targets. Every account has a default bus and you can create other custom buses.
- Rule triggers

  - Event Pattern - define event source and event pattern that will trigger the rule. Ex - EC2 terminated
  - Scheduled - Can set up recurring schedule for triggering a rule. Rate based or cron based

- EventBridge Architecture Example
  - User action
  - Event matches rule
  - EventBridge triggers lambda function
  - EventBridge publishes SNS message
