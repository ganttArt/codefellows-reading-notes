# Readings: AWS: API, Dynamo and Lambda

## Review, Research, and Discussion

1. What are serverless functions?
    - AWS Lambdas are an example
    - They are "single-purpose, programmatic functions that are hosted on managed infrastructure. These functions, which are invoked through the Internet, are hosted and maintained by cloud computing companies."[src](https://www.pubnub.com/blog/what-is-a-serverless-function/#:~:text=Conventionally%2C%20serverless%20functions%20are%20single,maintained%20by%20cloud%20computing%20companies.&text=Software%20developers%20are%20moving%20their%20product%20code%20to%20serverless%20functions.)
1. If you were to create a system that emulated Lambda functions, how would you do it?
    - I could use events or socket.io to listen for an event, and then have some functionality trigger on that event happening.
1. Describe how a CDN works
    - In order to improve speed and connectivity, a CDN will place servers at the exchange points between different networks. These Internet exchange points (IXPs) are the primary locations where different Internet providers connect in order to provide each other access to traffic originating on their different networks. By having a connection to these high speed and highly interconnected locations, a CDN provider is able to reduce costs and transit times in high speed data delivery. [src](https://www.cloudflare.com/learning/cdn/what-is-a-cdn/)

## Document the following Vocabulary Terms

- **Serverless Functions** - single-purpose, programmatic functions that are hosted on managed infrastructure. These functions, which are invoked through the Internet, are hosted and maintained by cloud computing companies.[src](https://www.pubnub.com/blog/what-is-a-serverless-function/#:~:text=Conventionally%2C%20serverless%20functions%20are%20single,maintained%20by%20cloud%20computing%20companies.&text=Software%20developers%20are%20moving%20their%20product%20code%20to%20serverless%20functions.)
- **Cloud Storage** - a cloud computing model that stores data on the Internet through a cloud computing provider who manages and operates data storage as a service. It’s delivered on demand with just-in-time capacity and costs, and eliminates buying and managing your own data storage infrastructure. This gives you agility, global scale and durability, with “anytime, anywhere” data access. [src](https://aws.amazon.com/what-is-cloud-storage/)
- **CDN** - (Content Delivery Network) is a highly-distributed platform of servers that helps minimize delays in loading web page content by reducing the physical distance between the server and the user. This helps users around the world view the same high-quality content without slow loading times. [src](https://www.akamai.com/us/en/cdn/what-is-a-cdn.jsp)

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
    - AWS Lambdas are an example of a serverless function.
    - AWS Lambdas are so much like listening for events in socket.io. When an event is triggered that a client is listening for than some functions will happen.
    - There are services that handle CDN setup for you. Now that there are so many cloud computing solutions companies, it makes sense that there would be companies that would provide the service of taking care of the CDN.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    - Deploying a lambda to aws using the cli
    - Working with permissions in API gateway. Using middleware or something else that would only allow some people the ability to delete or update something for instance.
    - Working with EC2, seems like it was brought up briefly but we haven't done anything with it.
1. What are you most excited about trying to implement or see how it works?
    - Using s3 to store image files that is hooked up to a rest api that we create locally.

## Preparation Materials

- [AWS API Gateway Overview](https://www.serverless.com/amazon-api-gateway)
- [AWS API Gateway](https://aws.amazon.com/api-gateway/)
- [AWS DynamoDB Guide](https://www.dynamodbguide.com/what-is-dynamo-db/)
- [AWS DynamoDB](https://aws.amazon.com/dynamodb/)
- [Dynamoose](https://dynamoosejs.com/getting_started/Introduction)
