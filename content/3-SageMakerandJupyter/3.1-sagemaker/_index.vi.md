---
title : "Kết nối đến SageMaker"
date: "2025-08-12"
weight : 1
chapter : false
pre : " <b> 3.1. </b> "
---


#### Tạo SageMaker Unified studio domain
1. Truy cập [bảng điều khiển quản lý dịch vụ SageMaker](https://console.aws.amazon.com/datazone/home)
   + Nhấp vào **Create a Unified studio domain**.

![SM](datascienceplatformwtihjupyterandsagemaker/images/3.connect/001-SageMaker.png)

2. Tại trang **Create an Amazon SageMaker Unified Studio domain**.
   + Trong trường **How do you want to set up your domain?**, chọn **Quick setup**.
   + Nhấp vào **Choose VPC**.

![SM](datascienceplatformwtihjupyterandsagemaker/images/3.connect/002-SageMaker.png)

3. Sau khi nhấp **Choose VPC**
   + Trong trường **Virtual private cloud (VPC)**, chọn VPC của bạn.
   + Trong **Subnets**, chọn cả 3 subnet bạn đã tạo.

![SM](datascienceplatformwtihjupyterandsagemaker/images/3.connect/003-SageMaker.png)

4. Nhấp vào **Create domain**.

5. Truy cập [bảng điều khiển quản lý dịch vụ SageMaker AI](https://console.aws.amazon.com/sagemaker/home)
   + Nhấp vào **Domains**.

6. Tại trang **Domains**
   + Nhấp vào domain SageMaker của bạn.
{{% notice info %}}
Nếu bạn có nhiều hơn 1 domain trên trang **Domains**, bạn có thể xem thời gian tạo của nó để biết đâu là domain SageMaker.
{{% /notice %}}

![SM](datascienceplatformwtihjupyterandsagemaker/images/3.connect/008-SageMaker.png)

7. Tại trang domain SageMaker của bạn
   + Trong phần **Authentication and permissions**, nhấp vào **Edit**.

![SM](datascienceplatformwtihjupyterandsagemaker/images/3.connect/009-SageMaker.png)
   + Trong **Permissions**, tìm và chọn IAM role của bạn tại cả hai trường **Default execution role** và **Space default execution role**.
{{% notice info %}}
Đảm bảo rằng bạn đã chọn IAM role đã tạo trước đó có **SetSourceIdentity**, nếu không SageMaker sẽ không thể tạo không gian cho Jupyter notebook.
{{% /notice %}}

![SM](datascienceplatformwtihjupyterandsagemaker/images/3.connect/010-SageMaker.png)
   + Nhấp vào **Submit**.
8. Tại trang domain SageMaker của bạn
   + Trong **Network** , nhấp vào **Edit**.

![SM](datascienceplatformwtihjupyterandsagemaker/images/3.connect/011-SageMaker.png)
 + Trong **How do you want to connect to other AWS services?**, chọn **Public internet access** và nhấp vào **Submit**.

![SM](datascienceplatformwtihjupyterandsagemaker/images/3.connect/012-SageMaker.png)