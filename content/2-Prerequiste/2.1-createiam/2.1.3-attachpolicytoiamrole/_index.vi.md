---
title : "Gán Policy cho IAM Role"
date: "2025-08-12"
weight : 1
chapter : false
pre : " <b> 2.1.3 </b> "
---


#### Gán Policy cho IAM Role 
1. Vào [bảng điều khiển quản lý dịch vụ IAM](https://console.aws.amazon.com/iam/home)
   + Nhấp vào **Role**.
   + Tìm role của bạn và nhấp vào nó.

![IAM](datascienceplatformwtihjupyterandsagemaker/images/2.prerequisite/005-IAM.png)

2. Tại trang role của bạn.
   + Trong trường **Trust relationships** (Mối quan hệ tin cậy), nhấp vào **Edit trust policy** (Chỉnh sửa chính sách tin cậy).

![IAM](datascienceplatformwtihjupyterandsagemaker/images/2.prerequisite/006-IAM.png)

3. Tại trang **Edit trust policy**
   + Trong trường **Access level - read or write** (Cấp độ truy cập - đọc hoặc ghi), nhấp vào **SetSourceIdentity**.
   + Nhấp vào **Update policy** (Cập nhật chính sách).

![IAM](datascienceplatformwtihjupyterandsagemaker/images/2.prerequisite/007-IAM.png)