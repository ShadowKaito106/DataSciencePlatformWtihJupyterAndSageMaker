---
title : "Attach Policy to IAM Role"
date: "2025-08-12"
weight : 1
chapter : false
pre : " <b> 2.1.3 </b> "
---


#### Create IAM **Lab IAM**
1. Go to [IAM service management console](https://console.aws.amazon.com/iam/home)
   + Click **Role**.
   + Find your role and click on it.

![IAM](datascienceplatformwtihjupyterandsagemaker/images/2.prerequisite/005-IAM.png)

2. At your role page.
   + In the **Trust relationships** field, click **Edit trust policy**.

![IAM](datascienceplatformwtihjupyterandsagemaker/images/2.prerequisite/006-IAM.png)

3. At the **Edit trust policy** page
    + In the **Access level - read or write**, click **SetSourceIdentity**
    + Click **Update policy**

![IAM](datascienceplatformwtihjupyterandsagemaker/images/2.prerequisite/007-IAM.png)
