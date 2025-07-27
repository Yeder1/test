---
title : "Clean up resources"
date :  "2025-07-10" 
weight : 5 
chapter : false
pre : " <b> 5. </b> "
---

We will take the following steps to delete the resources we created in this exercise.

#### Delete AWS Lambda 
1. Go to [Lambda console](https://ap-southeast-1.console.aws.amazon.com/lambda/home?region=ap-southeast-1#/begin)
- Click **Functions**.
- Tick the data related to the lab.
- On the right corner, click Action.
- Select **delete**.

#### Delete AWS CloudWatch.
1. Go to [Amazon CloudWatch](https://ap-southeast-1.console.aws.amazon.com/cloudwatch/home?region=ap-southeast-1)
- Click **Dashboards**.
- Select the data related to the lab.
- Select **delete**.

1.1 Then go to **All alarms** on the left sidebar.
- Select the data related to the lab.
- On the right corner, click Action then select **delete**.

1.2 Continue to select **Log groups** on the left sidebar.
- Select all data related to the lab.
- On the right corner, click Action then select **delete**.

#### Delete AWS SNS
1. Go to [Amazon SNS](https://ap-southeast-1.console.aws.amazon.com/sns/v3/home?region=ap-southeast-1#/topics)
- Select **Topic**.
- Select the topics created in the lab.
- Select **delete**
- Then select **subscriptions**.
- Select the subscriptions created in the lab.
- Select **delete**

#### Delete IAM Policy
1. Go to [IAM](https://us-east-1.console.aws.amazon.com/iam/home?region=ap-southeast-1#/policies)
- Select **Policies**.
- Tick the data related to the lab.
- Then select **delete**



