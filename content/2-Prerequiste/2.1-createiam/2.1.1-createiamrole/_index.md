---
title : "Create IAM Role"
date: "2025-08-12"
weight : 1
chapter : false
pre : " <b> 2.1.1 </b> "
---


#### Create IAM **Lab IAM**
1. Go to [IAM service management console](https://console.aws.amazon.com/iam/home)
   + Click **Role**.
   + Click **Create Role**.

![IAM](/DataSciencePlatformWtihJupyterAndSageMaker/images/2.prerequisite/001-IAM.png)

2. At the **Create Role** page.
   + In the **Trusted entity type** field, click **AWS Service**.
   + In the **Use case** field, find and choose **SageMaker**.
   + Click **Next**.

![IAM](/DataSciencePlatformWtihJupyterAndSageMaker/images/2.prerequisite/002-IAM.png)

3. At the **Add Permissions** page, click **Next**. (we will modify it later)
4. At the **Name, review, and create**, name your role at **Role name** fleld and click **Submit**.