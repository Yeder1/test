---
title : "Tạo CloudWatch"
date :  "2025-07-10" 
weight : 1
chapter : false
pre : " <b> 3.1.</b> "
---

1. Truy cập [**Amazon CloudWatch**](https://ap-southeast-1.console.aws.amazon.com/cloudwatch/home?region=ap-southeast-1#home:/)
  + Tìm **CloudWatch**
  + Chọn **CloudWatch**
![CloudWatch](/images/3.awscloudwatch/1.png)

2. Trong giao diện CloudWatch
  + Tìm **Log group** ở thanh bên trái màn hình
  + Chọn những tài nguyên có liên quan tới những lambda cấu hình trước đó
![CloudWatch](/images/3.awscloudwatch/2.png)

2.1 Trong phần log streams của **Log group**
  + Chọn cái đầu tiên
![CloudWatch](/images/3.awscloudwatch/3.png)

2.2 Mở các report và error ra để xem chi tiết
  + Sẽ thấy error và report
![CloudWatch](/images/3.awscloudwatch/4.png)

3. Tiếp tục chọn **Lambda Insights** ở thanh bên trái màn hình
- Mở phần Performance monitoring ra và chọn **Single function**
- Sau đó đợi một vài phút để lambda insights hoạt động.
![CloudWatch](/images/3.awscloudwatch/5.png)

3.1 Sau đó lambda insights sẽ hiện như kết quả bên dưới
  + **Lambda insights** sẽ hiện ra số lần test thành công và thất bại trước đó 
![CloudWatch](/images/3.awscloudwatch/6.png)


4. Tạo ra một dashboard để theo dõi chi tiết hơn.
  + Chọn bảng điều khiển ở thanh bên trái màn hình 
  + Sau đó chọn **Create dashboard**
![CloudWatch](/images/3.awscloudwatch/7.png)

4.1 Đặt tên cho bảng điều khiển
  + Create new dashboard **`LambdaMonitoring`**
  + Ấn **Create dashboard**
![CloudWatch](/images/3.awscloudwatch/8.png)

4.2 Trong phần **Widget Configuration** 
  + Chọn **Line**
  + Chọn **Next**
![CloudWatch](/images/3.awscloudwatch/9.png)

4.3 Trong phần **Add Metric graph** 
  + Chọn **Lambda**
![CloudWatch](/images/3.awscloudwatch/10.png)

4.4 Tìm các chỉ số giám sát quan trọng của Lambda
  + Sau đó tích vào **Invocations**, **Duration**, **Errors** của **MonitoringDemoFuncton**
![CloudWatch](/images/3.awscloudwatch/11.png)

4.5 Tương tự các bước trên thêm coldstar và error cho dashboard
  + Chọn **CustomLambdaMetrics**
  + Ấn **Create widget**
![CloudWatch](/images/3.awscloudwatch/12.png)

4.6 Trong CustomLambdaMetrics
  + Tích vào **coldstarCount** và **ErrorCount**
![CloudWatch](/images/3.awscloudwatch/13.png)

5 Khi tạo thành công 
  + Sẽ hiện ra số lần gọi (Invocations),Thời gian thực thi (Duration) và error (Số lỗi)
  + Sau đó ấn **Save**
![CloudWatch](/images/3.awscloudwatch/14.png)



