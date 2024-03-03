---
title : "Glue"
date :  "`r Sys.Date()`" 
weight : 2
chapter : false
pre : " <b> 2.2 </b> "
---

## Create Glue 

We will create Glue Jobs, Glue Crawler, Glue Database

### Create Glue Database

1. Access the Glue console.:
    - Access the Glue console.
    - Select **Database**.
    - Select **Add Database**.

   ![Image](/repo_pmt_ws-001/images/2/027.png?featherlight=false&width=90pc)

    - Enter your database name
    - Enter your staging bucket URI
    - Select **Create Database**.
   
   ![Image](/repo_pmt_ws-001/images/2/033.png?featherlight=false&width=90pc)

### Create Glue Crawler

1. Set crawler properties, data source:
    - Access the Glue console. 
    - Select **Crawler**.
    - Select **Create crawler**.

   ![Image](/repo_pmt_ws-001/images/2/034.png?featherlight=false&width=90pc)

    - Enter your crawler name
    - Select **Next**.
    - Select **Add a data source**.
    - Select your destination folder in staging bucket. 
    - Select **Add an S3 data source**.
   ![Image](/repo_pmt_ws-001/images/2/046.png?featherlight=false&width=90pc)

   ![Image](/repo_pmt_ws-001/images/2/047.png?featherlight=false&width=90pc)

2. Set security:
   - Select your IAM glue role.
   - Select **Next**.
   
   ![Image](/repo_pmt_ws-001/images/2/048.png?featherlight=false&width=90pc)
3. Set output:
    - Select your staging database.
    - Select **Next**.

   ![Image](/repo_pmt_ws-001/images/2/049.png?featherlight=false&width=90pc)

   ![Image](/repo_pmt_ws-001/images/2/050.png?featherlight=false&width=90pc)

### Create Glue Jobs

1. Create Glue Jobs.:
    - Access the Glue console.
    - Select **ETL Jobs**.
    - Select **Visual ETL**.

   ![Image](/repo_pmt_ws-001/images/2/051.png?featherlight=false&width=90pc)
2.  Setup transform in Glue Jobs
    - Select **Source**.
    - Select **Amazon S3**.
    - Enter your folder in raw bucket 
    - Select your input data format.
    
    ![Image](/repo_pmt_ws-001/images/2/052.png?featherlight=false&width=90pc)
    - Select your source.
    - Select **Target**. 
    - Select **Amazon S3**. 
    - Enter your folder in raw bucket 
    - Select your output data format.
    
    ![Image](/repo_pmt_ws-001/images/2/053.png?featherlight=false&width=90pc)
3.  Setup detail of Glue Jobs
    - Enter your glue job name
    - Select your IAM glue role.
    - Enter number of worker
    - Select your Script path glue assets.
    - Select your Temporary path glue assets.
    - Select **Save**

    ![Image](/repo_pmt_ws-001/images/2/054.png?featherlight=false&width=90pc)

    ![Image](/repo_pmt_ws-001/images/2/055.png?featherlight=false&width=90pc)

    ![Image](/repo_pmt_ws-001/images/2/056.png?featherlight=false&width=90pc)
4. Test Glue Job run
    - Select **Run**

    ![Image](/repo_pmt_ws-001/images/2/064.png?featherlight=false&width=90pc)