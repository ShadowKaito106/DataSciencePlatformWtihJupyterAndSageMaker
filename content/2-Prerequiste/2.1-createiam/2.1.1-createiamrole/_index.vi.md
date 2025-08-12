---
title : "Tạo IAM Role"
date: "2025-08-12"
weight : 1
chapter : false
pre : " <b> 2.1.1 </b> "
---


#### Tạo IAM **Lab IAM**
1. Vào [bảng điều khiển quản lý dịch vụ IAM](https://console.aws.amazon.com/iam/home)
   + Nhấp vào **Role**.
   + Nhấp vào **Create Role**.

![VPC](datascienceplatformwtihjupyterandsagemaker/images/2.prerequisite/001-IAM.png)

2. Tại trang **Create Role**.
   + Trong trường **Trusted entity type**, nhấp vào **AWS Service**.
   + Trong trường **Use case**, tìm và chọn **SageMaker**.
   + Nhấp vào **Next** .

![VPC](datascienceplatformwtihjupyterandsagemaker/images/2.prerequisite/002-IAM.png)

3. Tại trang **Add Permissions** , nhấp vào **Next** . (chúng ta sẽ chỉnh sửa sau)
4. Tại phần **Name, review, and create** (Đặt tên, xem lại và tạo), đặt tên cho role của bạn tại trường **Role name** và nhấp vào **Submit** .