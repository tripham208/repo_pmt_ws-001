---
title : "Step Function"
date :  "`r Sys.Date()`" 
weight : 2
chapter : false
pre : " <b> 2.4 </b> "
---
## Tạo Step Function

Chúng ta sẽ tạo hàm Step sử dụng Glue job ETL data từ Raw đến Staging sau đó dùng Crawler tạo Glue Table cho truy vấn Athena

### Tạo Step Function

1. Tạo luồng công việc:
    - Truy cập bảng điều khiển Step Function.
    - Chọn **Create state machine**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/070.png?featherlight=false&width=90pc)
    - Chọn trống.
    - Chọn **Select**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/071.png?featherlight=false&width=90pc)
    - Kéo **StartJobRun** vào luồng công việc.
    - Nhập "crawler"
    - Kéo **StartCrawler** vào luồng công việc sau **StartJobRun**.
    - Nhập “pass”
    - Kéo **Pass** vào luồng công việc sau **StartJobRun**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/072.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/073.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/2/076.png?featherlight=false&width=90pc)

2. Chạy công việc Setup Glue
    - Chọn **StartJobRun**.
    - Nhập tham số: lấy thông số từ đầu vào khi thực thi
```
{
   "JobName.$": "$.job_name"
}
```
-
    - Chọn **Wait for task complete** để chờ công việc dán keo hoàn tất trước khi bắt đầu nhiệm vụ tiếp theo
    - Chọn đầu ra

![Hình ảnh](/repo_pmt_ws-001/images/2/074.png?featherlight=false&width=90pc)
-
    - Chọn **Add original input**.
    - Chọn **Hủy kết quả và giữ nguyên dữ liệu đầu vào** để chuyển tiếp dữ liệu đầu vào của bạn sang tác vụ tiếp theo.

![Hình ảnh](/repo_pmt_ws-001/images/2/075.png?featherlight=false&width=90pc)

3. Cài đặt chạy trình thu thập keo
    - Chọn **StartCrawler**.
    - Nhập tham số: lấy thông số từ đầu vào khi thực thi
```
{
   "Name.$": "$.job_crawler"
}
```
-
![Hình ảnh](/repo_pmt_ws-001/images/2/077.png?featherlight=false&width=90pc)

3. Thuộc tính chức năng Bước thiết lập
    - Chọn chỉnh sửa trạng thái tên máy.
    - Nhập tên hàm Step
    - Chọn vai trò IAM của chức năng Step
    - Chọn **Create**.

   ![Hình ảnh](/repo_pmt_ws-001/images/2/078.png?featherlight=false&width=90pc)