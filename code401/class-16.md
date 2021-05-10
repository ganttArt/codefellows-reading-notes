# Readings: AWS: Cloud Servers

## Review, Research, and Discussion

1. Describe the Web-Request-Response-Cycle
    - A computer makes a request to another computer that takes that request, does something to it, and then sends a response with some data to the first computer.
1. Explain what a “server” is, as it relates to the WRRC
    - Servers will be running the applications that are on both sides of the WRRC, making requests and sending responses to other servers.
1. What does it mean to “deploy” an application?
    - It means you are creating your application in a server that lives in the cloud, ie. a data center somewhere.

## Document the following Vocabulary Terms

- **Server** - a computer that provides data to other computers. It may serve data to systems on a local area network (LAN) or a wide area network (WAN) over the Internet. Many types of servers exist, including web servers, mail servers, and file servers. Each type runs software specific to the purpose of the server. [src](https://techterms.com/definition/server#:~:text=A%20server%20is%20a%20computer,the%20purpose%20of%20the%20server.)
- **Pub/Sub** - publish–subscribe is a messaging pattern where senders of messages, called publishers, do not program the messages to be sent directly to specific receivers, called subscribers, but instead categorize published messages into classes without knowledge of which subscribers [src](https://en.wikipedia.org/wiki/Publish%E2%80%93subscribe_pattern)
- **WRRC** - a cycle of requests and responses that flow between clients and servers. [src](https://medium.com/@jen_strong/the-request-response-cycle-of-the-web-1b7e206e9047)

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
    - Elastic Beanstalk (EBS) is the AWS solution for deploying and scaling web applications that you've built.
    - EC2 = Elastic Compute Cloud - & It is running new instances of your servers built in VMs/containers.
    - zip -rp server.zip *
      - to zip a folder and retain all permissions etc.. We will send this zip file up to aws.
    - `aws configure` in your terminal to setup the aws cli to your account.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    - Deploying a RESTful API to AWS
    - Spinning up multiple servers that are using socket.io and are able to talk to eachother to AWS.
    - How to hookup a nosql database to an aws deployment.
1. What are you most excited about trying to implement or see how it works?
    - How to setup scaling on your cloud deployment so that it will continue working with a high volume of traffic.

## Preparation Materials

- [Virtual Machines](https://www.youtube.com/watch?v=yIVXjl4SwVo) (Bookmark This)
- [VMS and the Cloud](https://www.youtube.com/watch?v=l0DfHUWMjsU) (Bookmark This)
- [AWS EC2](https://aws.amazon.com/ec2/)
- [EC2 For Humans](https://www.youtube.com/watch?v=lZMkgOMYYIg)
- [Elastic Beanstalk](https://www.youtube.com/watch?v=SrwxAScdyT0)
