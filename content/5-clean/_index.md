---
title : "Resource Cleanup"
date: "2025-08-12"
weight : 5
chapter : false
pre : " <b> 5. </b> "
---

#### Resource Cleanup
After completing the project, you should clean up unused resources to avoid unnecessary costs.

---

### 1. Delete VPC Resources
1. Go to the **VPC Console** in AWS.
2. Locate and **delete the VPCs** created for the project (ensure no active resources are attached to them).
3. Inside each VPC:
   - **Subnet** → Delete all custom subnets.
   - **Route Tables** → Delete all custom route tables.

### 2. Delete SageMaker AI Resources
1. Go to the **SageMaker Console**.
2. Open **Domain**:
   - Select the created domain → **Delete**.
3. Open **User profiles**:
   - Delete all users within the domain.
4. Open **Spaces**:
   - Delete all spaces created for the project.

### 3. Delete IAM Roles and Users
1. Go to the **IAM Console**.
2. **Roles**:
   - Find the roles created for SageMaker, S3, or VPC in the project.
   - Delete these roles (only if they are not attached to any service).
3. **Users**:
   - Delete the users created specifically for the project.
   - If the user belongs to a group → remove permissions or delete the user.