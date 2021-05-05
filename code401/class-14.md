# Readings: Event Driven Architecture

## Review, Research, and Discussion

1. What’s the difference between a FIFO and a standard queue?
    - FIFO queues have essentially the same features as standard queues, but provide the added benefits of supporting ordering and exactly-once processing. FIFO queues provide additional features that help prevent unintentional duplicates from being sent by message producers or from being received by message consumers. [src](https://aws.amazon.com/about-aws/whats-new/2016/11/amazon-sqs-introduces-fifo-queues-with-exactly-once-processing-and-lower-prices-for-standard-queues/#:~:text=FIFO%20queues%20have%20essentially%20the,being%20received%20by%20message%20consumers.)
1. How can the server be assured a message was properly received?
    - Sometimes, you might want to get a callback when the client confirmed the message reception. To do this, simply pass a function as the last parameter of .send or .emit. What's more, when you use .emit, the acknowledgement is done by you, which means you can also pass data along. [src](https://www.semicolonworld.com/question/47982/how-to-be-sure-that-message-via-socket-io-has-been-received-to-the-client)
1. What classic design pattern is best represented by event driven programming?
    - The Observer Pattern [src](https://www.sitepoint.com/javascript-design-patterns-observer-pattern/)
1. How do you test an event driven system?
    - Service tests for event-driven systems operate on events for inputs and events for outputs. More on testing strategy here [src](https://medium.com/dan-on-coding/testing-event-driven-systems-63c6b0c57517)

## Document the following Vocabulary Terms

- **FIFO Queue** - Amazon SQS FIFO (First-In-First-Out) queues are designed to enhance messaging between applications when the order of operations and events is critical, or where duplicates can't be tolerated. Examples of situations where you might use FIFO queues include the following:
  - To make sure that user-entered commands are run in the right order.
  - To display the correct product price by sending price modifications in the right order.
  - To prevent a student from enrolling in a course before registering for an account.
- **Pub/Sub** - publish–subscribe is a messaging pattern where senders of messages, called publishers, do not program the messages to be sent directly to specific receivers, called subscribers, but instead categorize published messages into classes without knowledge of which subscribers, if any, there may be. Similarly, subscribers express interest in one or more classes and only receive messages that are of interest, without knowledge of which publishers, if any, there are. [src](https://en.wikipedia.org/wiki/Publish%E2%80%93subscribe_pattern)

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
    - Simple Notification Service - AWS's pub/sub system
    - Simple Queue Service - queueing service for message processing. SQS could subscribe to SNS.
    - That a 'FIFO queue' at least as AWS has co-opted it, is more than just a queue that works in the way of first in first out.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    - The difference in deploying our projects to Heroku and AWS and when should we choose one or the other, in this case maybe we lean towards AWS because they have a product offering that is geared around what exactly it is that we are building?
    - Pub/sub for the layman. Meaning, can I set myself up to subscribe to things being published from certain servers or companies, or even something like news?
    - The Observer Pattern
1. What are you most excited about trying to implement or see how it works?
    - Implementing something like what we've been building using one of AWS's solutions.

## Preparation Materials

[AWS SNS and SQS](https://www.youtube.com/watch?v=mXk0MNjlO7A)
