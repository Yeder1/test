---
title : "Create cost alert"
date :  "2025-07-10" 
weight : 4
chapter : false
pre : " <b> 4. </b> "
---

1. In [**All alarms**](https://ap-southeast-1.console.aws.amazon.com/cloudwatch/home?region=ap-southeast-1#alarmsV2:/)
+ Select **Create alarm**
![CloudWatch](/images/4.alarm/1.png)

1.1 In the Specify metric and conditions section
+ Select **Select Metric**
+ Select Create alarm
![CloudWatch](/images/4.alarm/2.png)

1.2 In the **Add Metric graph** section
+ Select **Lambda**
![CloudWatch](/images/4.alarm/3-11.png)

1.3 Find important monitoring metrics of Lambda
+ Then check **Duration** of **MonitoringDemoFuncton**
+ Click **Select metric**
![CloudWatch](/images/4.alarm/4.png)

1.4 Specify metrics and conditions
+ Set Metric name as **`Duration`**
+ Statistic as **Average**
+ Period as **1 minute**
+ Conditions -> than... as 500
+ Then select **Next**
![CloudWatch](/images/4.alarm/5.png)

1.5 Configure actions
+ Alarm state trigger select **In alarm**
+ Send a notification to the following SNS topic select **Create new topic**
+ Create a new topic named **`LambdaAlerts`**
+ Enter your email in **(eg: abcxyz@gmail.com)**
+ Then select **Create topic**
![CloudWatch](/images/4.alarm/6.png)

{{% notice info %}}
You need to confirm in the gmail you registered.
{{% /notice %}}

1.6 Select **Next**
![CloudWatch](/images/4.alarm/7.png)

1.7 Add alarm details
+ Alarm name **`HighDurationAlarm`**
+ Select **Next**
![CloudWatch](/images/4.alarm/8.png)

1.8 Preview and create
+ Click **Create alarm**
![CloudWatch](/images/4.alarm/9.png)

2. Create successfully and continue to create similarly
![CloudWatch](/images/4.alarm/10.png)

2.1 In the **Add Metric graph** section
+ Select **Lambda**
![CloudWatch](/images/4.alarm/3-11.png)

2.2 Find important monitoring indicators of Lambda
+ Then check **Errors** of **MonitoringDemoFuncton**
+ Click **Select metric**
![CloudWatch](/images/4.alarm/12.png)

2.3 Specify metrics and conditions
+ Set Metric name as **`Errors`**
+ Statistic as **Average**
+ Period as **1 minute**
+ Conditions -> than... as 5
+ Then select **Next**
![CloudWatch](/images/4.alarm/13.png)

2.4 Configure actions
+ Alarm state trigger select **In alarm**
+ Send a notification to the following SNS topic select **Select an existing SNS topic**
+ Send a notification to **LambdaAlerts**
+ Then select **Create topic**
![CloudWatch](/images/4.alarm/14.png)

2.5 Select **Next**
![CloudWatch](/images/4.alarm/15.png)

2.6 Add alarm details
+ Alarm name **`HighErrorAlarm`**
+ Select **Next**
![CloudWatch](/images/4.alarm/16.png)

2.7 Preview and create
+ Click **Create alarm**
![CloudWatch](/images/4.alarm/17.png)

2.8 Created successfully
![CloudWatch](/images/4.alarm/18.png)
- **Go back to Lambda and click test many times, when the number of calls, execution time, and errors are exceeded, an email will be sent to you.**