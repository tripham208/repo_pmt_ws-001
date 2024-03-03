---
title : "Create S3 Bucket"
date :  "`r Sys.Date()`" 
weight : 1
chapter : false
pre : " <b> 2.2 </b> "
---
## Tạo S3 bucket

Chúng tôi sẽ tạo nhóm S3 cho dữ liệu thô, theo giai đoạn:

### Tạo S3 raw bucket

1. Truy cập bảng điều khiển S3.:
    - Truy cập bảng điều khiển S3.
    - Chọn **Create Bucket**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/002.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/020.png?featherlight=false&width=90pc)
    - Chọn vùng của bạn
    - Nhập tên nhóm của bạn
    - Chọn **Create Bucket**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/021.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/022.png?featherlight=false&width=90pc)
2. Tải file thô lên
    -  [Financial Sample](/repo_pmt_ws-001/Financial_Sample.csv)
    - Truy cập nhóm thô của bạn.
    - Chọn **Create Folder**.
    - Nhập tên thư mục của bạn
    - Chọn **Create Folder**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/028.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/029.png?featherlight=false&width=90pc)

    - Truy cập thư mục của bạn
    - Chọn **Upload**.
    - Tải tập tin của bạn lên
    - Chọn **Upload**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/030.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/031.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/032.png?featherlight=false&width=90pc)

### Tạo S3 staging bucket

1. Truy cập bảng điều khiển S3.:
    - Truy cập bảng điều khiển S3.
    - Chọn **Create Bucket**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/023.png?featherlight=false&width=90pc)
    - Chọn vùng của bạn
    - Nhập tên nhóm của bạn
    - Chọn **Create Bucket**.
    -
   ![Hình ảnh](/repo_pmt_ws-001/images/2/024.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/025.png?featherlight=false&width=90pc)
### Tạo nhóm nội dung S3 Glue

1. Truy cập bảng điều khiển S3.:
    - Truy cập bảng điều khiển S3.
    - Chọn **Create Bucket**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/023.png?featherlight=false&width=90pc)
    - Chọn vùng của bạn
    - Nhập tên nhóm của bạn
    - Chọn **Create Bucket**.
    -
   ![Hình ảnh](/repo_pmt_ws-001/images/2/026.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/025.png?featherlight=false&width=90pc)