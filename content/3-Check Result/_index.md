---
title : "Check result"
date : "`r Sys.Date()`"
weight : 3
chapter : false
pre : " <b> 3. </b> "
---
## Check result


### Execute Step Function

1. Execute Step Function:
    - Access the Step Function console.
    - Select your Step Function.
    - Select **Start execution**.
    - Enter your "job_name", "job_crawler"
    - Select **Start execution**.
   
    ![Image](/repo_pmt_ws-001/images/3/088.png?featherlight=false&width=90pc)

2. Check execute.
    - Select glue job task.
    - Select **Glue job**
    - You can see your glue job is running

   ![Image](/repo_pmt_ws-001/images/3/087.png?featherlight=false&width=90pc)

   ![Image](/repo_pmt_ws-001/images/3/091.png?featherlight=false&width=90pc)

    - After glue job succeed crawler will start
   
    ![Image](/repo_pmt_ws-001/images/3/096.png?featherlight=false&width=90pc)

    ![Image](/repo_pmt_ws-001/images/3/091.png?featherlight=false&width=90pc)

    - After glue crawler complete: a table created

    ![Image](/repo_pmt_ws-001/images/3/100.png?featherlight=false&width=90pc)

    ![Image](/repo_pmt_ws-001/images/3/101.png?featherlight=false&width=90pc)

### Query in Athena
1. Setting query result location:
    - Access the Athena console.
    - Setting query result location
      - Select query result location
      - Select **Save**
   
    ![Image](/repo_pmt_ws-001/images/3/102.png?featherlight=false&width=90pc)

    ![Image](/repo_pmt_ws-001/images/3/103.png?featherlight=false&width=90pc)
2. Query in Athena
    - Select your staging database.
    - Input your query.
    - Select **Run**
    - You can see sql query result from file in S3
   
   ![Image](/repo_pmt_ws-001/images/3/104.png?featherlight=false&width=90pc)