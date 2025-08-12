---
title : "Tạo IAM User"
date: "2025-08-12"
weight : 1
chapter : false
pre : " <b> 2.1.2 </b> "
---


#### Tạo IAM User **Lab IAM User**
1. Vào [bảng điều khiển quản lý dịch vụ IAM](https://console.aws.amazon.com/iam/home)
   + Nhấp vào **User**.
   + Nhấp vào **Create User**.

![VPC](/DataSciencePlatformWtihJupyterAndSageMaker/images/2.prerequisite/003-IAM.png)

2. Tại trang **Specify user details**.
   + Trong trường **User name**, nhập tên người dùng cho người dùng mới.
   + Nhấp vào **Next**.

![VPC](/DataSciencePlatformWtihJupyterAndSageMaker/images/2.prerequisite/004-IAM.png)

3. Tại trang **Set permissions** 
   + Trong trường **Permissions options**, chọn **Attach policies directly**
   + Tìm và chọn **AmazonSageMakerFullAccess**, **AmazonS3FullAccess**, **CloudWatchFullAccess**
4. Tại phần **Review and create**, nhấp vào **Submit**.