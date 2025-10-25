# AWS-DATA-PIPELINE-PROJECT-EC2-EMR-S3-GLUE-ATHENA-PYSPARK
In this project, we are designing and implementing a batch data processing pipeline using AWS and PySpark.


Data Ingestion: The source data, initially available as CSV files in the local environment, is migrated into an Amazon S3 bucket under the raw/ directory. Data security is ensured by configuring appropriate IAM roles and key pairs on the EC2 instance for encryption and controlled access.

Data Transformation: Using PySpark on an Amazon EMR cluster, we perform required transformations such as record counts, string replacements (e.g., handling delimiters), and schema adjustments. The transformed data is then written back into the S3 bucket under the transformed/ directory in an optimized format.

Data Consumption: Once available in the transformed/ folder, the data is exposed via Amazon Athena, enabling downstream teams to query the data directly. These curated tables then serve as the foundation for business dashboards and reporting, providing insights to end customers.

## Use Case
Monthly sales data is delivered as CSV files into an Amazon S3 bucket, but the raw data is not ready for analysis. We need an automated pipeline that processes this data using Amazon EMR (Spark), applies required transformations, and stores the cleaned output in a curated S3 bucket. The processed data should then be made queryable through AWS Glue Data Catalog and Amazon Athena for analysts and data scientists to use.

### What you will learn

- How to create and setup an Amazon EMR cluster
- How to submit a PySpark job on EMR
- How to integrate EMR with Amazon S3
- How to integrate S3 bucket with Amazon Athena

# STEP 1
- Open EC2 instance and create key pair by giving name.
  
choose private key file format .pem or .ppk based on your usage.

