- Web API with an HTTP endpoint can be created for lambda function using Amazon API gateway.
- Web APIs can route HTTP requests to lambda functions.
- Authentication and authorization controls can be added to API.
- Resources define methods like GET or POST, these methods are integrated to a lambda function.
- To add an HTTP method to your API, you first need to create a resource for that method to operate on.??
- A proxy resource catches all paths beneath a resource.

[Adding API Gateway/endpoint to Lambda](https://docs.aws.amazon.com/lambda/latest/dg/services-apigateway.html#apigateway-add)

## Proxy Integration

- API Gateway APIs are comprised of stages, resources, methods and integrations.
- Stage and resource determine path of the endpoint.
- /prod/user
  /{STAGE}/{RESOURCE}
- /dev/{proxy+}
  - Any route with dev stage
- Path and HTTP method combination is mapped to a lambda function.

## Event format

- API Gateway invokes lambda synchronously with an event that contains JSON representation of HTTP request.
- For a custom integration, the event is the body of the request. ??
- For a proxy integration, the event has a defined structure. ??

## Response format

- API Gateway waits for a response from your function and relays the result to the caller.
- For a custom integration, you define an integration response and a method response to convert the output from the function to an HTTP response.??
- For a proxy integration, the function must respond with a representation of the response in a specific format. ??

## Permissions

- to access lambda form API gateway (TBD)

## Handling error with an API Gateway API

- API Gateway treats all invocation and function errors as internal errors.
- If the Lambda API rejects the invocation request,
  API Gateway returns a 500 error code.
- If the function runs but returns an error, or
  returns a response in the wrong format,
  API Gateway returns a 502.
- In both cases, the body of the response from API Gateway is {"message": "Internal server error"}.
- To customize the error response, you must catch errors in your code and format a response in the required format.

## API Types

- HTTP, REST, Websocket
- REST API
  - supports custom Lambda integrations
- Websocket API
  - Use a WebSocket API for applications that benefit from a persistent connection between the client and API.
  - Provides full-duplex communication, which means that both the client and the API can send messages continuously without waiting for a response.
