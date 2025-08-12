---
title : "Create IAM User"
date: "2025-08-12"
weight : 1
chapter : false
pre : " <b> 2.1.2 </b> "
---


#### Create IAM **Lab IAM**
1. Go to [IAM service management console](https://console.aws.amazon.com/iam/home)
   + Click **User**.
   + Click **Create User**.

![IAM](datascienceplatformwtihjupyterandsagemaker/images/2.prerequisite/003-IAM.png)

2. At the **Specify user details** page.
   + In the **User name** field, type a user name for new user.
   + Click **Next**.

![IAM](datascienceplatformwtihjupyterandsagemaker/images/2.prerequisite/004-IAM.png)

3. At the **Set permissions** page
   + In the **Permissions options** field, choose **Attach policies directly**
   + Find and choose **AmazonSageMakerFullAccess**, **AmazonS3FullAccess**, **CloudWatchFullAccess**
4. At the **Review and create**, click **Submit**.