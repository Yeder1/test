---
title : "Tạo cảnh báo chi phí"
date :  "2025-07-10" 
weight : 4
chapter : false
pre : " <b> 4. </b> "
---

1. Trong [**All alarms**](https://ap-southeast-1.console.aws.amazon.com/cloudwatch/home?region=ap-southeast-1#alarmsV2:/)
  + Chọn **Create alarm**
![CloudWatch](/images/4.alarm/1.png)

1.1 Trong phần Specify metric and conditions
+ Chọn **Select Metric**
+ Chọn **Create alarm**
![CloudWatch](/images/4.alarm/2.png)

1.2 Trong phần **Add Metric graph** 
  + Chọn **Lambda**
![CloudWatch](/images/4.alarm/3-11.png)

1.3 Tìm các chỉ số giám sát quan trọng của Lambda
+ Sau đó tích vào **Duration** của **MonitoringDemoFuncton**
+ Ấn vào **Select metric**
![CloudWatch](/images/4.alarm/4.png)

1.4 Chỉ định số liệu và điều kiện
+ Đặt Metric name là **`Duration`**
+ Statistic là **Average**
+ Period là **1 minute**
+ Conditions -> **than...** **là 500**
+ Sau đó chọn **Next**
![CloudWatch](/images/4.alarm/5.png)

1.5 Cấu hình hành động
+ Alarm state trigger chọn **In alarm**
+ Send a notification to the following SNS topic chọn **Create new topic**
+ Create a new topic đặt tên là **`LambdaAlerts`**
+ Nhập mail của bạn vào **(vd: abcxyz@gmail.com)**
+ Sau đó chọn **Create topic**
![CloudWatch](/images/4.alarm/6.png)

{{% notice info %}}
Bạn cần xác ở trong gmail mà bạn đã đăng ký.
{{% /notice %}}

1.6 Chọn **Next**
![CloudWatch](/images/4.alarm/7.png)

1.7 Thêm chi tiết báo động
+ Alarm name **`HighDurationAlarm`**
+ Chọn **Next**
![CloudWatch](/images/4.alarm/8.png)

1.8 Xem trước và tạo
+ Ấn **Create alarm**
![CloudWatch](/images/4.alarm/9.png)

2. Tạo thành công và tiếp tục tạo tương tự
![CloudWatch](/images/4.alarm/10.png)

2.1 Trong phần **Add Metric graph** 
  + Chọn **Lambda**
![CloudWatch](/images/4.alarm/3-11.png)

2.2 Tìm các chỉ số giám sát quan trọng của Lambda
+ Sau đó tích vào **Errors** của **MonitoringDemoFuncton**
+ Ấn vào **Select metric**
![CloudWatch](/images/4.alarm/12.png)

2.3 Chỉ định số liệu và điều kiện
+ Đặt Metric name là **`Errors`**
+ Statistic là **Average**
+ Period là **1 minute**
+ Conditions -> **than... là 5**
+ Sau đó chọn **Next**
![CloudWatch](/images/4.alarm/13.png)

2.4 Cấu hình hành động
+ Alarm state trigger chọn **In alarm**
+ Send a notification to the following SNS topic chọn **Select an existing SNS topic**
+ Send a notification to **LambdaAlerts**
+ Sau đó chọn **Create topic**
![CloudWatch](/images/4.alarm/14.png)

2.5 Chọn **Next**
![CloudWatch](/images/4.alarm/15.png)

2.6 Thêm chi tiết báo động
+ Alarm name **`HighErrorAlarm`**
+ Chọn **Next**
![CloudWatch](/images/4.alarm/16.png)

2.7 Xem trước và tạo
+ Ấn **Create alarm**
![CloudWatch](/images/4.alarm/17.png)

2.8 Tạo thành công 
![CloudWatch](/images/4.alarm/18.png)
- **Bạn hãy trở lại Lambda và bấm test nhiều lần thì khi vượt quá số lần gọi, thời gian thực thi, và lỗi thì sẽ gửi mail về cho bạn.**

