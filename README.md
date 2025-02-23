# aws-s3-datalake

## Steps

---

### 1) Create IAM Role for EC2 to Access S3
- Create a role in IAM for EC2 with S3 access (full, read, or write based on use case).

### 2) Create EC2 Instance with SSH
- Launch an EC2 instance and attach the IAM role created in step 1.

### 3) SSH into EC2 and Install Spark, Hadoop, and OpenJDK
- SSH into the EC2 instance and install Spark, Hadoop, and OpenJDK.
- Set the necessary environment variables.

### 4) Create VPC Endpoint for EC2 to Access S3
- Create a VPC endpoint for secure, private network access to the S3 service.

### 5) Install Jupyter Notebook
- Install Jupyter Notebook on the EC2 instance.
- Run Jupyter Notebook without the browser option.

### 6) Tunnel Jupyter Server to Local Machine and Read S3 Objects using Spark
- Use SSH tunneling to access Jupyter Notebook on your local machine.
- Read data from S3 using Spark.

---

**Dataset Source**: [TLC Trip Record Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.pages)
