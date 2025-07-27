---
title : "Create CloudWatch"
date :  "2025-07-10" 
weight : 1
chapter : false
pre : " <b> 3.1. </b> "
---

1. Go to [**Amazon CloudWatch**](https://ap-southeast-1.console.aws.amazon.com/cloudwatch/home?khuo=ap-southeast-1#home:/)
+ Find **CloudWatch**
+ Select **CloudWatch**
![CloudWatch](/images/3.awscloudwatch/1.png)

2. CloudWatch Interface
+ Find **Log Group** on the left sidebar
+ Select the resources related to the previous lambda configuration 
![CloudWatch](/images/3.awscloudwatch/2.png)

2.1 In the log stream of **Log Group**
+ Select the first item
![CloudWatch](/images/3.awscloudwatch/3.png)

2.2 Open reports and errors to view details
+ You will see the error reports and reports report
![CloudWatch](/images/3.awscloudwatch/4.png)

3. Continue to select **Lambda Insights** on the left sidebar of the screen
- Open and select the Performance Monitoring item **Single Function**
- Then, wait a few minutes for lambda Insights to work.
![CloudWatch](/images/3.awscloudwatch/5.png)

3.1 Then, the lambda details will be displayed as the result below

+ **Lambda Details** will display the previous successful and failed tests
![CloudWatch](/images/3.awscloudwatch/6.png)

4. Create a dashboard for more detailed monitoring.
+ Select the dashboard on the left side of the screen

+ Then select **Create Dashboard**
![CloudWatch](/images/3.awscloudwatch/7.png)

4.1 Name the dashboard
+ Create a new dashboard **`LambdaMonitoring`**
+ Click **Create Dashboard**
![CloudWatch](/images/3.awscloudwatch/8.png)

4.2 In the **Utility Configuration** section
+ Select **Line**
+ Select **Next**
![CloudWatch](/images/3.awscloudwatch/9.png)

4.3 In the **Add Metric Chart** section
+ Select **Lambda**
![CloudWatch](/images/3.awscloudwatch/10.png)

4.4 Find the important Lambda monitoring item
+ Then select **Invitation**, **Duration**, **Error** of **MonitorDemoFuncton**
![CloudWatch](/images/3.awscloudwatch/11.png)

4.5 Same steps as above to add coldstar and error to dashboard
+ Select **CustomLambdaMetrics**
+ Click **Create Extension**
![CloudWatch](/images/3.awscloudwatch/12.png)

4.6 In CustomLambdaMetrics
+ Check **ColdstarCount** and **ErrorCount**

![CloudWatch](/images/3.awscloudwatch/13.png)

5 When created successfully
+ Number of Invocations, Duration and Number of errors will appear
+ Then click **Save**
![CloudWatch](/images/3.awscloudwatch/14.png)