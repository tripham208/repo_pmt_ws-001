---
title : "Glue"
date :  "`r Sys.Date()`" 
weight : 2
chapter : false
pre : " <b> 2.3 </b> "
---
## Tạo Glue

Chúng tôi sẽ tạo Glue Jobs, Glue Crawler, Glue Database

### Tạo Glue Database

1. Truy cập bảng điều khiển Glue.:
    - Truy cập bảng điều khiển Keo.
    - Chọn **Database**.
    - Chọn **Add Database**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/027.png?featherlight=false&width=90pc)

    - Nhập tên cơ sở dữ liệu của bạn
    - Nhập URI nhóm dàn dựng của bạn
    - Chọn **Add Database**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/033.png?featherlight=false&width=90pc)

### Tạo Glue Crawler

1. Đặt thuộc tính trình thu thập thông tin, nguồn dữ liệu:
    - Truy cập bảng điều khiển Keo.
    - Chọn **Crawler**.
    - Chọn **Create crawler**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/034.png?featherlight=false&width=90pc)

    - Nhập tên trình thu thập thông tin của bạn
    - Chọn **Next**.
    - Chọn **Add a data source**.
    - Chọn thư mục đích của bạn trong nhóm dàn dựng.
    - Chọn **Add an S3 data source**.
      ![Hình ảnh](/repo_pmt_ws-001/images/2/046.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/047.png?featherlight=false&width=90pc)

2. Đặt bảo mật:
    - Chọn vai trò keo IAM của bạn.
    - Chọn **Next**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/048.png?featherlight=false&width=90pc)
3. Đặt đầu ra:
    - Chọn cơ sở dữ liệu dàn dựng của bạn.
    - Chọn **Next**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/049.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/050.png?featherlight=false&width=90pc)

### Tạo Glue Jobs

1. Tạo công việc dán keo.:
    - Truy cập bảng điều khiển Keo.
    - Chọn **ETL Jobs**.
    - Chọn **Visual ETL**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/051.png?featherlight=false&width=90pc)
2. Thiết lập biến đổi trong Công việc Keo
    - Chọn **Source**.
    - Chọn **Amazon S3**.
    - Nhập thư mục của bạn vào thùng thô
    - Chọn định dạng dữ liệu đầu vào của bạn.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/052.png?featherlight=false&width=90pc)
    - Chọn nguồn của bạn.
    - Chọn **Target**.
    - Chọn **Amazon S3**.
    - Nhập thư mục của bạn vào thùng thô
    - Chọn định dạng dữ liệu đầu ra của bạn.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/053.png?featherlight=false&width=90pc)
3. Thiết lập chi tiết công việc dán keo
    - Nhập tên công việc keo của bạn
    - Chọn vai trò keo IAM của bạn.
    - Nhập số lượng công nhân
    - Chọn nội dung keo đường dẫn tập lệnh của bạn.
    - Chọn nội dung keo đường dẫn tạm thời của bạn.
    - Chọn **Save**

   ![Hình ảnh](/repo_pmt_ws-001/images/2/054.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/055.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/056.png?featherlight=false&width=90pc)
4. Chạy thử keo
    - Chọn **Run**

   ![Hình ảnh](/repo_pmt_ws-001/images/2/064.png?featherlight=false&width=90pc)