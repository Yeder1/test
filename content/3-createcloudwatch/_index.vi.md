---
title : "Tạo CloudWatch"
date :  "2025-07-10" 
weight : 3
chapter : false
pre : " <b> 3. </b> "
---
### Giới thiệu về CloudWatch
- **Amazon CloudWatch** là một dịch vụ giám sát hiệu suất và thu thập log do AWS cung cấp
- Theo dõi tài nguyên như EC2, Lambda, RDS, DynamoDB, v.v.
- Thu thập và phân tích log, metrics (chỉ số), và sự kiện.
- Cảnh báo (alarm) khi có vấn đề xảy ra (ví dụ như CPU cao bất thường).
- Xây dashboard trực quan để theo dõi hệ thống theo thời gian thực.

### Ứng dụng thực tế
- Giám sát lỗi hệ thống.
- Đo hiệu suất hàm Lambda.
- Cảnh báo sớm khi có sự cố.
- Phân tích log truy cập, lỗi hệ thống.

{{% notice note %}}
Ở bước này, chúng ta sẽ tạo Amazon CloudWatch để theo dõi tài nguyên Lambda.
{{% /notice %}}

### Nội dung
3.1. [Tạo CloudWatch](3.1-create)

