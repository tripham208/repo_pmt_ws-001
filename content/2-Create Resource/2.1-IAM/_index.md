---
title : "Create IAM Role"
date :  "`r Sys.Date()`" 
weight : 1
chapter : false
pre : " <b> 2.1 </b> "
---

## Create IAM Role

We will create IAM role for Glue, Step Function:

### Create IAM role for Glue

1. Access the IAM console:
    - Access the IAM console.
    - On the left navigation bar, select **Roles**
    - Select **Create role**.

   ![Image](/repo_pmt_ws-001/images/2/001.png?featherlight=false&width=90pc)
   
   ![Image](/repo_pmt_ws-001/images/2/006.png?featherlight=false&width=90pc)

2. Create role for Glue.
   - Select **AWS Service**.
   - Enter **Glue** in "Use case".
   - Select **Next**.

   ![Image](/repo_pmt_ws-001/images/2/007.png?featherlight=false&width=90pc)

   - Enter **glue** 
   - Select **AWSGlueServiceRole**.
   - Enter **s3**
   - Select **AmazonS3FullAccess**.

   ![Image](/repo_pmt_ws-001/images/2/008.png?featherlight=false&width=90pc)

   ![Image](/repo_pmt_ws-001/images/2/061.png?featherlight=false&width=90pc)
   - Enter Role name
   - Select **Create role**.

   ![Image](/repo_pmt_ws-001/images/2/009.png?featherlight=false&width=90pc)

   ![Image](/repo_pmt_ws-001/images/2/062.png?featherlight=false&width=90pc)

### Create IAM role for Step Function
1. Access the IAM console:
   - Access the IAM console.
   - On the left navigation bar, select **Roles**
   - Select **Create role**.

   ![Image](/repo_pmt_ws-001/images/2/011.png?featherlight=false&width=90pc)

2. Create role for Step Function.
   - Select **AWS Service**.
   - Enter **Step Function** in "Use case".
   - Select **Next**.

   ![Image](/repo_pmt_ws-001/images/2/012.png?featherlight=false&width=90pc)

   - Select **Next**.

   ![Image](/repo_pmt_ws-001/images/2/013.png?featherlight=false&width=90pc)
   - Enter Role name
   - Select **Create role**.

   ![Image](/repo_pmt_ws-001/images/2/014.png?featherlight=false&width=90pc)

   ![Image](/repo_pmt_ws-001/images/2/015.png?featherlight=false&width=90pc)

3. Update Permission.
   - Select your step function role.
   - Select **Add permissions**.
   - Select **AdministrationAccess**.
   - Select **Add permissions**.

   ![Image](/repo_pmt_ws-001/images/2/016.png?featherlight=false&width=90pc)

   ![Image](/repo_pmt_ws-001/images/2/017.png?featherlight=false&width=90pc)

   ![Image](/repo_pmt_ws-001/images/2/018.png?featherlight=false&width=90pc)

   ![Image](/repo_pmt_ws-001/images/2/019.png?featherlight=false&width=90pc)

{{% notice info %}}
You should specify permissions when using different services in the step function
{{% /notice %}}