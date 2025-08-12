---
title : "Connect to SageMaker"
date: "2025-08-12"
weight : 1
chapter : false
pre : " <b> 3.1. </b> "
---


#### Create SageMaker Unified studio domain
1. Go to [SageMaker service management console](https://console.aws.amazon.com/datazone/home)
    + Click **Create a Unified studio domain**.

![SM](datascienceplatformwtihjupyterandsagemaker/images/3.connect/001-SageMaker.png)

2. At **Create an Amazon SageMaker Unified Studio domain** page.
    + In the **How do you want to set up your domain?** field, choose **Quick setup**.
    + Click **Choose VPC**.

![SM](datascienceplatformwtihjupyterandsagemaker/images/3.connect/002-SageMaker.png)

3. After Click **Choose VPC**
    + In the **Virtual private cloud (VPC)** field, choose your VPC.
    + In the **Subnets**, choose all 3 subnets you create.

![SM](datascienceplatformwtihjupyterandsagemaker/images/3.connect/003-SageMaker.png)

4. Click **Create domain**.

5. Go to [SageMaker AI service management console](https://console.aws.amazon.com/sagemaker/home)
    + Click **Domains**.

6. At **Domains** page
    + Click on your SageMaker domain. 
{{% notice info %}}
If you have more than 1 domain on **Domains** page, you can look at it's created time to know which one is SageMaker domain. 
{{% /notice %}}

![SM](datascienceplatformwtihjupyterandsagemaker/images/3.connect/008-SageMaker.png)

7. At your SageMaker domain page
    + In the **Authentication and permissions**, click **Edit**.

![SM](datascienceplatformwtihjupyterandsagemaker/images/3.connect/009-SageMaker.png)
    + In the **Permissions**, find and choose your IAM role at both **Default execution role** and **Space default execution role** field.
{{% notice info %}}
Make sure that you choose the IAM role that you create before that have **SetSourceIdentity** if don't SageMaker will unable to create space for Jupyter notebook
{{% /notice %}}

![SM](datascienceplatformwtihjupyterandsagemaker/images/3.connect/010-SageMaker.png)
    + Click **Submit**
8. At your SageMaker domain page
    + In the **Network**, click **Edit**.

![SM](datascienceplatformwtihjupyterandsagemaker/images/3.connect/011-SageMaker.png)
    + In the **How do you want to connect to other AWS services?**, choose **Public internet access** and click **Submit**

![SM](datascienceplatformwtihjupyterandsagemaker/images/3.connect/012-SageMaker.png)