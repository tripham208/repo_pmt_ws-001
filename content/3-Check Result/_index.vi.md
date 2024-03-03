---
title : "Check result"
date :  "`r Sys.Date()`" 
weight : 3
chapter : false
pre : " <b> 3. </b> "
---
## Kiểm tra kết quả


### Thực thi Step Function

1. Thực thi Step Function:
   - Truy cập bảng điều khiển Step Function.
   - Chọn chức năng bước của bạn.
   - Chọn **Start execution**.
   - Nhập "job_name", "job_crawler" của bạn
   - Chọn **Start execution**.

   ![Hình ảnh](/repo_pmt_ws-001/images/3/088.png?featherlight=false&width=90pc)

2. Kiểm tra thực hiện.
   - Chọn nhiệm vụ công việc dán keo.
   - Chọn **Glue job**
   - Bạn có thể thấy công việc dán keo của mình đang chạy

   ![Hình ảnh](/repo_pmt_ws-001/images/3/087.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/3/091.png?featherlight=false&width=90pc)

   - Sau khi dán thành công trình thu thập thông tin sẽ bắt đầu

   ![Hình ảnh](/repo_pmt_ws-001/images/3/096.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/3/091.png?featherlight=false&width=90pc)

   - Sau khi trình thu thập keo hoàn tất: một bảng được tạo

   ![Hình ảnh](/repo_pmt_ws-001/images/3/100.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/3/101.png?featherlight=false&width=90pc)

### Truy vấn trong Athena
1. Thiết lập vị trí kết quả truy vấn:
   - Truy cập bảng điều khiển Athena.
   - Đặt vị trí kết quả truy vấn
      - Chọn vị trí kết quả truy vấn
      - Chọn **Save**

   ![Hình ảnh](/repo_pmt_ws-001/images/3/102.png?featherlight=false&width=90pc)

   ![Hình ảnh](/repo_pmt_ws-001/images/3/103.png?featherlight=false&width=90pc)
2. Truy vấn trong Athena
   - Chọn cơ sở dữ liệu dàn dựng của bạn.
   - Nhập truy vấn của bạn.
   - Chọn **Run**
   - Bạn có thể xem kết quả truy vấn sql từ tệp trong S3

   ![Hình ảnh](/repo_pmt_ws-001/images/3/104.png?featherlight=false&width=90pc)