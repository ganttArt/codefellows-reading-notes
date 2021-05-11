# Readings: AWS: S3 and Lambda

## Review, Research, and Discussion

1. Describe “The Cloud”
    - The cloud is a way for people have their computing needs met non-locally.
1. What is a container (as it relates to computers and servers)?
    - A container is a way to wrap up an application and all of its dependencies, so that you can reliably run the application no matter what your underlying operating system is.
1. What is auto-scaling?
    - When you deploy an application to a cloud service like AWS, you can set up your application to scale when your site traffic increases. This means that AWS will be doing work behind the scenes to create more instances of your application that can handle the load of increased user traffic. When the site traffic goes back down, AWS will scale back down too by removing those added instances.
1. What is bandwidth?
    - the maximum rate of data transfer across a given path [src](https://en.wikipedia.org/wiki/Bandwidth_(computing))
1. How do cloud providers compute service costs?
    - When setting price, cloud providers determine the expense to maintaining the network. They start by calculating costs for network hardware, network infrastructure maintenance, and labor. These expenses are added together and then divided by the number of rack units a business will need for its IaaS cloud. [src](https://expedient.com/knowledgebase/blog/2015-05-01-how-the-cost-of-cloud-computing-is-calculated/#:~:text=When%20setting%20price%2C%20cloud%20providers,need%20for%20its%20IaaS%20cloud.)

## Document the following Vocabulary

- **Server Instances** - Instances in AWS are basically virtual environments. These virtual environments are isolated from the underlying base OS. It's an On-demand service, i.e. a user can rent the virtual server(instances) on an hourly base and deploy their applications on it. [src](https://www.edureka.co/blog/ec2-instances-in-aws/)
- **Containers** - A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another.
- **Cloud Services** - refers to a wide range of services delivered on demand to companies and customers over the internet. These services are designed to provide easy, affordable access to applications and resources, without the need for internal infrastructure or hardware. [src](https://www.citrix.com/glossary/what-is-a-cloud-service.html#:~:text=The%20term%20%22cloud%20services%22%20refers,for%20internal%20infrastructure%20or%20hardware.)
- **Cloud Architecture** - refers to the various components in terms of databases, software capabilities, applications, etc. engineered to leverage the power of cloud resources to solve business problems. Cloud architecture defines the components as well as the relationships between them. [src](https://www.hcltech.com/technology-qa/what-is-cloud-architecture#:~:text=Cloud%20Architecture%20refers%20to%20the,as%20the%20relationships%20between%20them.&text=Cloud%20resources,-Software%20components%20and)
- **AWS** - a secure cloud services platform, offering compute power, database storage, content delivery and other functionality to help businesses scale and grow. [src](https://blog.usejournal.com/what-is-aws-and-what-can-you-do-with-it-395b585b03c)
- **EC2/Beanstalk vs Heroku** - EC2 and Elastic Beanstalk are AWS solutions for deploying software solutions. Heroku is actually built on top of these services offered by AWS and provides an arguably more user/developer friendly experience for deploying and managing applications.

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
    - How lambdas are used within the context of AWS. My understanding now is that lambdas are used to be able to have multiple AWS services that you are using work together and do work upon certain actions being triggered.
    - S3 is not just a good storage solution for images, it will also be used for things like audio or video files.
    - A CDN is a way that services can be distributed such that people in different places around the world are accessing the information they need from a server that is closest to them.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    - The different ways we can deploy a API to AWS. Either using their builtin API solution or working with something like EB where we deploy a node/express server with routes.
    - How we can write code that will add files to S3 buckets.
    - How to scale your application in AWS such that it is using a CDN where people on the other side of the world would have faster access to my application.
1. What are you most excited about trying to implement or see how it works?
    - Adding files to s3 programmatically in JS.

## Preparation Materials

[AWS S3](https://aws.amazon.com/s3/)
[AWS Lambda Basics](https://www.serverless.com/aws-lambda)
[AWS Lambda Functions](https://aws.amazon.com/lambda/)
[CDN](https://cyberhoot.com/cybrary/content-delivery-network-cdn/)
