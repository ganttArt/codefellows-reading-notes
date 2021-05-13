# Readings: AWS: Events

## Review, Research, and Discussion

1. Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server
    - With an express server you can write RESTful API routes, like those that you can make in API Gateway, and have all of the functionality of those routes within them, which would be the Lambda function piece.
1. List the AWS Database offerings and talk about the pros and cons of each
    - S3
      - Pros: Free file storage for smaller amounts of data.
      - Cons: Limited number of changes per month before pay structure begins
    - Lambda
      - Pros: Integration with other AWS services
      - Cons: Cost, can get into infinite loops of being triggered if not careful.
    - DynamoDB
      - Pros: Interface for putting in new data.
      - Cons: Need integrations with other services to have non-gui crud or REST actions done.
    - API Gateway
      - Pros: Easily setup routes for your api
      - Cons: Need integration with other services for api actions
    - Elastic Beanstalk
      - Pros: Easily setup an application
      - Cons: Resource heavy
    - SNS
      - Pros: Easily setup email or sms notifications that can be subscribed to.
      - Cons: Not sure, it could be hard to add a lot of subscribers.
    - SQS
      - Pros: Standard or FIFO queue.
      - Cons: Not straight forward setup for just peeking at items in the queue.
    - Overall con: you're funneling more money to one of the top richest people on the planet.
1. What’s the difference between a FIFO and a standard queue?
    - In a FIFO queue, the subscriber will get the first item put in the queue first, where in the standard queue, messages will be received by the subscriber in a seemingly random order.
1. How can the server be assured a message was properly received?
    - If the server is using TCP as opposed to UDP, a response from the receiver is necessary.

## Document the following Vocabulary Terms

- **Serverless API** - a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers. A serverless application runs in stateless compute containers that are event-triggered, ephemeral (may last for one invocation), and fully managed by the cloud provider. [src](https://hackernoon.com/what-is-serverless-architecture-what-are-its-pros-and-cons-cc4b804022e9)
- **Triggers** - a Lambda resource or a resource in another service that you configure to invoke your function in response to lifecycle events, external requests, or on a schedule. [src](https://docs.aws.amazon.com/lambda/latest/dg/lambda-invocation.html)
- **Dynamo vs Mongo** - Dynamo and Mongo are both NoSQL databases. They are formatted in similar ways, they just come from different companies: Dynamo from AWS and MongoDB from Mongo
- **Dynamoose vs Mongoose** - These are solutions to modeling data and performing crud actions for NoSQL databases. The first being for DynamoDB and the second being for MongoDB.

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
    - That SNS is an easy way to create a text message notification service.
    - How FIFO queues and standard queues differentiate on AWS.
    - A little bit more about what Serverless means in the context of cloud services. I've always thought of serverless as being a microservices architecture, but here I see it more in the way that in AWS you can setup different services that interact with each other.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    - Going deeper into building React front ends.
    - Using Redux for state management
    - Discussing more applications of using sqs and/or sns.
1. What are you most excited about trying to implement or see how it works?
    - An SNS service that will send me email notifications.

## Preparation Materials

- [SQS and SNS Basics](https://www.youtube.com/watch?v=UesxWuZMZqI)
- [AWS SQS vs SNS](https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5)

## Bookmark

- [SNS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SNS.html)
- [SQS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SQS.html)
