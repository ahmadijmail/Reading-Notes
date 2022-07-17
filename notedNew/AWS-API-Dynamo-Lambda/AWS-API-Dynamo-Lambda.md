# AWS: API, Dynamo and Lambda

## AWS API Gateway Overview
<br>

What is Amazon API Gateway?

iT's a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. 

Why is Amazon API Gateway an important part of the Serverless ecosystem?

API Gateway allows you to implement a fully managed authentication and authorization layer by using Amazon Cognito and Lambda custom authorizers without running your own auth systems.


How does API Gateway integrate with other AWS services?

This type of integration lets an API expose AWS service actions. In AWS integration, you must configure both the integration request and integration response and set up necessary data mappings from the method request to the integration request, and from the integration response to the method response.


## AWS API Gateway

What are the some benefits of using Amazon API Gateway?

Efficient API development

Performance at any scale


Cost savings at scale

What two API types might you choose from?

1. RESTful APIs

2. WEBSOCKET APIs


## AWS DynamoDB Guide

What is DynamoDB?

 a hosted NoSQL database offered by Amazon Web Services (AWS).

What is Dynamoose?

 a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose


 What are some key features of Dynamoose?

Type safety

High level API

Easy to use syntax

Ability to transform data before saving or retrieving documents

Strict data modeling (validation, required attributes, and more)

Support for DynamoDB Transactions

Powerful Conditional/Filtering Support

Callback & Promise support

