---
title : "Dọn dẹp tài nguyên"
date: "2025-08-12"
weight : 5
chapter : false
pre : " <b> 5. </b> "
---

#### Dọn dẹp tài nguyên
Sau khi hoàn thành dự án, cần dọn dẹp các tài nguyên để tránh phát sinh chi phí.

---

### 1. Xóa tài nguyên VPC
1. Truy cập **VPC Console** trên AWS.
2. Tìm và **xóa các VPC** đã tạo cho dự án (đảm bảo không còn tài nguyên nào đang gắn với VPC này).
3. Trong từng VPC:
   - **Subnet** → Xóa tất cả subnet tùy chỉnh.
   - **Route Tables** → Xóa bảng định tuyến tùy chỉnh.

### 2. Xóa tài nguyên SageMaker AI
1. Truy cập **SageMaker Console**.
2. Vào **Domain**:
   - Chọn Domain đã tạo → **Delete**.
3. Vào **User profiles**:
   - Xóa tất cả user trong domain.
4. Vào **Spaces**:
   - Xóa các space đã tạo cho dự án.

### 3. Xóa IAM Role và User
1. Truy cập **IAM Console**.
2. **Roles**:
   - Tìm các role được tạo cho SageMaker, VPC trong dự án.
   - Xóa các role này (chỉ khi không còn gắn với dịch vụ nào).
3. **Users**:
   - Xóa user được tạo riêng cho dự án.
   - Nếu user nằm trong group → xóa quyền hoặc xóa user luôn.