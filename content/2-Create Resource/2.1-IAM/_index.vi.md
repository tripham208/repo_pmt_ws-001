---
title : "Create IAM Role"
date :  "`r Sys.Date()`"
weight : 1
chapter : false
pre : " <b> 2.1 </b> "
---

## Tạo vai trò IAM

Chúng ta sẽ tạo vai trò IAM cho Glue, Step Function:

### Tạo vai trò IAM cho Glue

1. Truy cập bảng điều khiển IAM:
  - Truy cập bảng điều khiển IAM.
  - Trên thanh điều hướng bên trái chọn **Vai trò**
  - Chọn **Tạo vai trò**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/001.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/006.png?featherlight=false&width=90pc)

2. Tạo vai trò cho Glue.
  - Chọn **Dịch vụ AWS**.
  - Nhập **Glue** vào "Ca sử dụng".
  - Chọn **Tiếp theo**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/007.png?featherlight=false&width=90pc)

  - Nhập **keo**
  - Chọn **AWSGlueServiceRole**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/008.png?featherlight=false&width=90pc)
  - Nhập tên vai trò
  - Chọn **Tạo vai trò**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/009.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/010.png?featherlight=false&width=90pc)
### Tạo vai trò IAM cho Step Function
1. Truy cập bảng điều khiển IAM:
  - Truy cập bảng điều khiển IAM.
  - Trên thanh điều hướng bên trái chọn **Vai trò**
  - Chọn **Tạo vai trò**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/011.png?featherlight=false&width=90pc)

2. Tạo vai trò cho Step Function.
  - Chọn **Dịch vụ AWS**.
  - Nhập **Step Function** vào "Ca sử dụng".
  - Chọn **Tiếp theo**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/012.png?featherlight=false&width=90pc)

  - Chọn **Tiếp theo**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/013.png?featherlight=false&width=90pc)
  - Nhập tên vai trò
  - Chọn **Tạo vai trò**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/014.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/015.png?featherlight=false&width=90pc)

3. Cập nhật quyền.
  - Chọn vai trò chức năng bước của bạn.
  - Chọn **Thêm quyền**.
  - Chọn **Truy cập quản trị**.
  - Chọn **Thêm quyền**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/016.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/017.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/018.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/019.png?featherlight=false&width=90pc)