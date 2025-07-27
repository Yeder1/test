---
title : "Chuẩn bị AWS Lambda"
date :  "2025-07-10" 
weight : 1
chapter : false
pre : " <b> 2.1 </b> "
---

### Giới Thiệu
**AWS Lambda** là dịch vụ điện toán không máy chủ (serverless), cho phép bạn chạy mã mà không cần cung cấp hoặc quản lý máy chủ. Bạn chỉ cần viết mã và Lambda sẽ tự động lo việc mở rộng quy mô, quản lý tính sẵn sàng và xử lý lỗi.

### Tại sao lại là AWS Lambda?

**AWS Lambda** cho phép bạn chạy mã cho hầu hết mọi loại ứng dụng hoặc dịch vụ backend mà không cần cung cấp hoặc quản lý máy chủ. Chỉ cần tải mã của bạn lên dưới dạng hàm Lambda và dịch vụ sẽ tự động đảm nhận mọi việc còn lại. Lambda hỗ trợ nhiều ngôn ngữ lập trình như Python, Node.js, Java, Go, v.v.
Lambda tích hợp chặt chẽ với các dịch vụ khác của AWS như Amazon S3, DynamoDB, API Gateway và CloudWatch để bạn có thể xây dựng các ứng dụng hoàn chỉnh, dễ dàng mở rộng và tiết kiệm chi phí. Với mô hình tính phí theo thời gian thực thi và số lượng request, Lambda là lựa chọn lý tưởng cho những khối lượng công việc không ổn định, biến động.

### Lợi ích của AWS Lambda
- **Không cần quản lý máy chủ**: Tự động triển khai và mở rộng hàm theo lượng request. Bạn không cần lo lắng về việc cấu hình, vá lỗi hay bảo trì máy chủ.
- **Chi phí thấp, tối ưu tài nguyên**: Chỉ thanh toán cho thời gian thực tế mà mã của bạn chạy và số lần gọi hàm. Không tốn chi phí khi không sử dụng.
- **Khả năng mở rộng linh hoạt**: Tự động mở rộng theo số lượng request, từ vài request/giây đến hàng ngàn mà không cần can thiệp.
- **Tích hợp dễ dàng với các dịch vụ AWS khác**:  Dễ dàng xây dựng ứng dụng event-driven, xử lý real-time, tự động hóa workflows với các dịch vụ như S3, DynamoDB, SNS, API Gateway...

{{% notice note %}}
Để tìm hiểu thêm về AWS Lambda, bạn có thể tham khảo trang web bên dưới được mô tả
{{% /notice %}}

- **[About AWS Lambda](https://aws.amazon.com/lambda/)**

### Nội dung
  - [Tạo Amazon Lambda](2.1.1-createlambda/)
  - [Cài đặt Amazon Lambda  ](2.2-testlambda/)

