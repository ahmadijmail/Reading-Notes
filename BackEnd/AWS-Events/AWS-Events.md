# AWS: Events

### What is the difference betweeen SQS and SNS? 

SNS is a distributed publish-subscribe service.

SQS is distributed queuing service.

### What are some use cases for both SNS and SQS?


## Choose SNS if:

You would like to be able to publish and consume batches of messages. 

You would like to allow same message to be processed in multiple ways.

Multiple subscribers are needed.

## Choose SQS if:

You need a simple queue with no particular additional requirements.
Decoupling two applications and allowing parallel asynchronous processing.
Only one subscriber is needed.

Describe how to use SQS and SNS in a “fanout” pattern.

The Fanout scenario is when a message published to an SNS topic is replicated and pushed to multiple endpoints, such as Kinesis Data Firehose delivery

Explain how “push notifications” work, using SNS.

Amazon SNS uses the device token to create a mobile endpoint, to which it can send direct push notification messages.
