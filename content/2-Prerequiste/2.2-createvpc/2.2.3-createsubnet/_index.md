---
title : "Create subnet"
date: "2025-08-12"
weight : 1
chapter : false
pre : " <b> 2.2.3 </b> "
---


#### Create subnet
1. Go to [VPC service management console](https://console.aws.amazon.com/vpc/home)
   + Click **Subnets**.
   + Click **Create subnet**.

![VPC](/images/2.prerequisite/012-VPC.png)

2. At the **Create subnet** page.
   + In the **VPC ID** field, choose the id of your VPC.
   + In the **Subnet name** field, name your subnet.
{{% notice info %}}
Recommend name it with **"yoursubnetname-a"** to seperate with 2 more subnet **"yoursubnetname-b"** and **"yoursubnetname-c"** you will create later for **SageMaker** domain.
{{% /notice %}}
   + In the **Availability Zone** field, choose the zone for your subnet.
{{% notice info %}}
I choose **us-east-1a** for this subnet and choose **us-east-1b** and **us-east-1c** for 2 others subnet in this project.It maybe different depend on your account region.
{{% /notice %}}
   + In the **IPv4 subnet CIDR block** field, set your subnet IPv4 to **10.0.1.0/24**. **10.0.2.0/24** and **10.0.3.0/24** will be set into 2 others subnet. 
   + Click **Add new subnet** to create 2 more subnet.
![VPC](/images/2.prerequisite/013-VPC.png)

   + Click **Create subnet** after you done all 3 subnets.

3. To set it to public in order to run network on your JupyterLab
   + At the **Subnets** page, click your subnet to tick it and click **Actions**.
   + In the **Actions** dropdown, click **Edit subnet settings**.
   + At the **Edit subnet settings**, tick on the **Enable auto-assign public IPv4 address** in the **Auto-assign IP settings** field.
   + Click **Save**
   + Do the same with all 3 subnets.
   
![VPC](/images/2.prerequisite/014-VPC.png)