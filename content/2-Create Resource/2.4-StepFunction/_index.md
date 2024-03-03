**---
title : "Step Function"
date :  "`r Sys.Date()`"
weight : 1
chapter : false
pre : " <b> 2.1 </b> "
---

## Create Step Function

We will create Step function use Glue job ETL data from Raw to Staging then use Crawler create Glue Table for Athena query

### Create Step Function

1. Create work flow:
    - Access the Step Function console.
    - Select **Create state machine**.

   ![Image](/repo_pmt_ws-001/images/2/070.png?featherlight=false&width=90pc)
    - Select blank.
    - Select **Select**.

   ![Image](/repo_pmt_ws-001/images/2/071.png?featherlight=false&width=90pc)
    - Drag **StartJobRun** to work flow.
    - Enter "crawler"
    - Drag **StartCrawler** to work flow after **StartJobRun**. 
    - Enter "pass"
    - Drag **Pass** to work flow after **StartJobRun**.

   ![Image](/repo_pmt_ws-001/images/2/072.png?featherlight=false&width=90pc)

   ![Image](/repo_pmt_ws-001/images/2/073.png?featherlight=false&width=90pc)

   ![Image](/repo_pmt_ws-001/images/2/076.png?featherlight=false&width=90pc)

2. Setup Glue job run
    - Select **StartJobRun**.
    - Enter Parameters: get param from your input when you execute
```
{
  "JobName.$": "$.job_name"
}
```
- 
    - Select **Wait for task complete** to wait glue job run complete before start next task
    - Select Output

    ![Image](/repo_pmt_ws-001/images/2/074.png?featherlight=false&width=90pc)
- 
    - Select **Add original input**.
    - Select **Discard result and keep original input** to forward your input to next task.
  
    ![Image](/repo_pmt_ws-001/images/2/075.png?featherlight=false&width=90pc)

3. Setup Glue crawler run
    - Select **StartCrawler**.
    - Enter Parameters: get param from your input when you execute
```
{
  "Name.$": "$.job_crawler"
}
```
-
    ![Image](/repo_pmt_ws-001/images/2/077.png?featherlight=false&width=90pc)

3. Setup Step function properties
    - Select edit name state machine.
    - Enter Step function's name
    - Select IAM role of Step function
    - Select **Create**.
   
    ![Image](/repo_pmt_ws-001/images/2/078.png?featherlight=false&width=90pc)
