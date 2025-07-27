---
title : "Cấu hình Lambda"
date : "2024-12-05"
weight : 2
chapter : false
pre : " <b> 2.2 </b> "
---

### Cấu hình Lambda.

1. Truy cập [AWS Management Console](https://aws.amazon.com/console/) 
   + Chọn **Code**.
   + Xóa đoạn code cũ và dán đoạn code này vào **Code source**.
   + Ấn vào **Deploy**.
![Lambda](/images/2.prerequisite/05-test.png)


2. Trong giao diện Lambda
   + Sau đó chọn **Configuraion**
   + Chọn **General Configuration**
   + Ấn **Edit**
![Lambda](/images/2.prerequisite/06-config.png)

2.1 Trong phần Create a function
   + Ở phần **Memory**
   + Đặt thành **256** 
   + Ấn **Save**
![Lambda](/images/2.prerequisite/07-edit.png)

2.2 Thông báo tạo thành công như hình bên dưới.
![Lambda](/images/2.prerequisite/08-updatesuccess.png)

3. Sau đó chọn **Test**
   + Chọn **create new event**
   + Event name **`NormalEvent`**
   + Event json để mặt định 
   + Ấn vào **Test** 5 - 7 lần và sau đó **Save**
![Lambda](/images/2.prerequisite/09-test.png)

3.1 Tương tự vậy tạo thêm một cái test lỗi để kiểm tra
   + Chọn create new event
   + Event name **`ErorrEvent`**
   + Event json **`{"cause_erorr": true}`**
   + Ấn vào **Test** 2 lần và sau đó **Save**
![Lambda](/images/2.prerequisite/10-test.png)

{{% notice note %}}
Ở bước này chúng ta sẽ tạo ra một lỗi nhỏ để thuận tiện cho việc theo dõi.
{{% /notice %}}

3.2 Tiếp tục vào phần configuration
   + Chọn **Monitoring and openrations tools**
   + Chọn **Edit**
![Lambda](/images/2.prerequisite/11-edit2.png)

3.3 Trong phần Edit monitoring tools 
   + Tích chọn **Enable** cho phần application Signals
   + Tích chọn **Enable** cho Lambda service traces
   + Tích chọn **Enhanced monitoring** cho CloudWatch Insights 
   + Sau đó ấn **Save**
![Lambda](/images/2.prerequisite/12-edit3.png)

3.4 Thông báo cập nhật thành công như ảnh trên
   + Và sau đó chờ 10 phút để lambda insight hoạt động
![Lambda](/images/2.prerequisite/13-editsuccess.png)