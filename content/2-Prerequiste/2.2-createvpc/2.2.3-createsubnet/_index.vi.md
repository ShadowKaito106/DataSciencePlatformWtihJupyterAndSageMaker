---
title : "Tạo subnet"
date: "2025-08-12"
weight : 1
chapter : false
pre : " <b> 2.2.3 </b> "
---


#### Tạo subnet
1. Truy cập [bảng điều khiển quản lý dịch vụ VPC](https://console.aws.amazon.com/vpc/home)
   + Nhấp vào **Subnets**.
   + Nhấp vào **Create subnet**.

![VPC](/images/2.prerequisite/012-VPC.png)

2. Tại trang **Create subnet**.
   + Trong trường **VPC ID**, chọn ID của VPC của bạn.
   + Trong trường **Subnet name**, đặt tên cho subnet của bạn.
{{% notice info %}}
Nên đặt tên là **"tên_subnet_của_bạn-a"** để phân biệt với 2 subnet khác là **"tên_subnet_của_bạn-b"** và **"tên_subnet_của_bạn-c"** mà bạn sẽ tạo sau này cho domain **SageMaker**.
{{% /notice %}}
   + Trong trường **Availability Zone**, chọn khu vực cho subnet của bạn.
{{% notice info %}}
Tôi chọn **us-east-1a** cho subnet này và chọn **us-east-1b** và **us-east-1c** cho 2 subnet khác trong dự án này. Nó có thể khác nhau tùy thuộc vào khu vực tài khoản của bạn.
{{% /notice %}}
   + Trong trường **IPv4 subnet CIDR block**, đặt IPv4 cho subnet của bạn là **10.0.1.0/24**. **10.0.2.0/24** và **10.0.3.0/24** sẽ được đặt cho 2 subnet khác.
   + Nhấp vào **Add new subnet** để tạo thêm 2 subnet nữa.
![VPC](/images/2.prerequisite/013-VPC.png)

   + Nhấp vào **Create subnet** sau khi bạn đã hoàn thành cả 3 subnet.

3. Để đặt nó thành public nhằm chạy mạng trên JupyterLab của bạn
   + Tại trang **Subnets**, nhấp vào subnet của bạn để đánh dấu chọn và nhấp vào **Actions**.
   + Trong menu thả xuống **Actions**, nhấp vào **Edit subnet settings**.
   + Tại **Edit subnet settings**, đánh dấu chọn **Enable auto-assign public IPv4 address** trong trường **Auto-assign IP settings**.
   + Nhấp vào **Save**.
   + Làm tương tự với cả 3 subnet.

![VPC](/images/2.prerequisite/014-VPC.png)