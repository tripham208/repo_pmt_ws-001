---
title : "Clean up resources"
date : "`r Sys.Date()`"
weight : 6
chapter : false
pre : " <b> 6. </b> "
---
## Clean up resources

We will proceed to delete the resources in the following order:

### Delete Glue Job, Glue Crawler, Glue Database

1. Delete Glue Job:
    - Access the Glue console.
    - On the left navigation bar, select **ETL Jobs**
    - Select your glue job
    - Select **Action**
    - Select **Delete job**

   ![Image](/repo_pmt_ws-001/images/4/200.png?featherlight=false&width=90pc)

2. Delete Glue Crawler:
    - Access the Glue console.
    - On the left navigation bar, select **Crawler**
    - Select your Crawler
    - Select **Action**
    - Select **Delete Crawler**

   ![Image](/repo_pmt_ws-001/images/4/201.png?featherlight=false&width=90pc)
3. Delete Glue Database:
    - Access the Glue console.
    - On the left navigation bar, select **Database**
    - Select your Database
    - Select **Delete**

   ![Image](/repo_pmt_ws-001/images/4/202.png?featherlight=false&width=90pc)
    - When delete database you can't query this database in Athena
    ![Image](/repo_pmt_ws-001/images/4/203.png?featherlight=false&width=90pc)

### Delete Step Function

- Access the Step Function console.
- Select your step function 
- Select **Delete**

  ![Image](/repo_pmt_ws-001/images/4/204.png?featherlight=false&width=90pc)

### Delete S3 bucket

- Access the S3 console.
- Select your bucket
- Select **Delete**


![Image](/repo_pmt_ws-001/images/4/206.png?featherlight=false&width=90pc)

![Image](/repo_pmt_ws-001/images/4/210.png?featherlight=false&width=90pc)
- Select **Empty bucket**
- Enter **permanently delete**
- Select **Empty**


![Image](/repo_pmt_ws-001/images/4/205.png?featherlight=false&width=90pc)
- Select your bucket
- Select **Delete**
- Enter your bucket name
- Select **Delete bucket**

![Image](/repo_pmt_ws-001/images/4/207.png?featherlight=false&width=90pc)