---
title : "Lambda Configuration"
date : "2024-12-05"
weight : 2
chapter : false
pre : " <b> 2.2 </b> "
---

### Configuration Lambda.
1. Go to [AWS Management Console](https://aws.amazon.com/console/)
+ Select **Code**.
+ Delete the old code and paste this code into **Code source**.
+ Click **Deploy**.
![Lambda](/images/2.prerequisite/05-test.png)

2. In the Lambda interface
+ Then select **Configuraion**
+ Select **General Configuration**
+ Click **Edit**
![Lambda](/images/2.prerequisite/06-config.png)

2.1 In the Create a function section
+ In the **Memory** section
+ Set to **256**
+ Click **Save**
![Lambda](/images/2.prerequisite/07-edit.png)

2.2 The creation success message is shown below.
![Lambda](/images/2.prerequisite/08-updatesuccess.png)

3. Then select **Test**
+ Select create new event
+ Event name **`NormalEvent`**
+ Event json to default
+ Click **Test** 5 - 7 times and then **Save**
![Lambda](/images/2.prerequisite/09-test.png)

3.1 Similarly, create another error test to check
+ Select create new event
+ Event name **`ErorrEvent`**
+ Event json **`{"cause_erorr": true}`**
+ Click **Test** 2 times and then **Save**
![Lambda](/images/2.prerequisite/10-test.png)

3.2 Continue to configuration
+ Select **Monitoring and openings tools**
+ Select **Edit**
![Lambda](/images/2.prerequisite/11-edit2.png)

3.3 In the Edit monitoring tools section
+ Check **Enable** for application Signals
+ Check **Enable** for Lambda service traces
+ Check **Enhanced monitoring** for CloudWatch Insights
+ Then click **Save**
![Lambda](/images/2.prerequisite/12-edit3.png)

3.4 Successful update notification as shown above
+ And then wait 10 minutes for lambda insight to work dynamic
![Lambda](/images/2.prerequisite/13-editsuccess.png)