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
  - Trên thanh điều hướng bên trái chọn **Roles**
  - Chọn **Create role**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/001.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/006.png?featherlight=false&width=90pc)

2. Tạo vai trò cho Glue.
  - Chọn **AWS Service**.
  - Nhập **Glue** vào "Use case".
  - Chọn **Next**.

![Image](/repo_pmt_ws-001/images/2/007.png?featherlight=false&width=90pc)

- Nhập **glue**
- Chọn **AWSGlueServiceRole**.
- Nhập **s3**
- Chọn **AmazonS3FullAccess**.

![Image](/repo_pmt_ws-001/images/2/008.png?featherlight=false&width=90pc)

![Image](/repo_pmt_ws-001/images/2/061.png?featherlight=false&width=90pc)
- Nhập Role name
- Chọn **Create role**.

![Image](/repo_pmt_ws-001/images/2/009.png?featherlight=false&width=90pc)

![Image](/repo_pmt_ws-001/images/2/062.png?featherlight=false&width=90pc)
### Tạo vai trò IAM cho Step Function
1. Truy cập bảng điều khiển IAM:
  - Truy cập bảng điều khiển IAM.
  - Trên thanh điều hướng bên trái chọn **Roles**
  - Chọn **Create role**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/011.png?featherlight=false&width=90pc)

2. Tạo vai trò cho Step Function.
  - Chọn **AWS Service**.
  - Nhập **Step Function** vào "Use case".
  - Chọn **Next**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/012.png?featherlight=false&width=90pc)

  - Chọn **Next**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/013.png?featherlight=false&width=90pc)
  - Nhập tên vai trò
  - Chọn **Create role**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/014.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/015.png?featherlight=false&width=90pc)

3. Cập nhật quyền.
  - Chọn vai trò chức năng bước của bạn.
  - Chọn **Add permissions**.
  - Chọn **AdministrationAccess**.
  - Chọn **Add permissions**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/016.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/017.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/018.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/019.png?featherlight=false&width=90pc)