---
title : "Preparing Lambda"
date :  "2025-07-10" 
weight : 1
chapter : false
pre : " <b> 2.1 </b> "
---

### Introduction
**AWS Lambda** is a serverless computing service that lets you run code without provisioning or managing servers. You just write code, and Lambda automatically takes care of scaling, availability, and failure handling.

### Why AWS Lambda?

**AWS Lambda** lets you run code for almost any type of application or backend service without provisioning or managing servers. Simply upload your code as a Lambda function, and the service automatically takes care of the rest. Lambda supports a variety of programming languages, including Python, Node.js, Java, Go, and more.
Lambda integrates tightly with other AWS services like Amazon S3, DynamoDB, API Gateway, and CloudWatch so you can build complete, scalable, and cost-effective applications. With its time-of-execution and request-based pricing model, Lambda is ideal for volatile, volatile workloads.

### Benefits of AWS Lambda
- **No Server Management**: Automatically deploy and scale functions based on request volume. You don't need to worry about configuring, patching, or maintaining servers.

- **Low Cost, Resource-Optimized**: Pay only for the actual time your code runs and the number of function calls. No cost when not in use.

- **Elastic Scalability**: Automatically scale based on request volume, from a few requests/second to thousands without intervention.
- **Easy integration with other AWS services**: Easily build event-driven applications, handle real-time, automate workflows with services such as S3, DynamoDB, SNS, API Gateway...

{{% notice note %}}
To learn more about AWS Lambda, you can refer to the website below described
{{% /notice %}}

- [About AWS Lambda](https://aws.amazon.com/lambda/)

### Contents
- [Create Amazon Lambda](2.1.1-createlambda/)
- [Install Amazon Lambda ](2.2-testlambda/)

