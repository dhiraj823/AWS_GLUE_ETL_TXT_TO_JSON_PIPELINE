# AWS_GLUE_ETL_TXT_TO_JSON_PIPELINE
# i attached all screenshots of  my project workflow and txt file and the updated file named run... typ .. for understanding.

AWS Glue ETL Pipeline: TXT to JSON Conversion

📌 Project Overview

This project demonstrates the implementation of an ETL (Extract, Transform, Load) pipeline using AWS Glue and Amazon S3.

The main objective is to convert raw sales data stored in TXT format into structured JSON format using AWS Glue and store the transformed data in an S3 bucket.

🎯 Business Requirements

1. Raw sales data is received in TXT format and stored in Amazon S3.
2. The data needs to be converted into JSON format.
3. An ETL pipeline must be created to automate the transformation process.

🏗️ Architecture

The pipeline follows this workflow:

Amazon S3 (TXT) → AWS Glue Crawler → AWS Glue Data Catalog → AWS Glue ETL Job → Amazon S3 (JSON)

🛠️ AWS Services Used

- Amazon S3: Stores raw input data and transformed output data.
- AWS Glue Crawler: Discovers the schema of the source data.
- AWS Glue Data Catalog: Stores metadata and table definitions.
- AWS Glue ETL Job: Processes and transforms the input data.
- Python / PySpark: Used for data transformation.

⚙️ Project Workflow

Step 1: Upload Raw Data

Uploaded the sales.txt file into the source Amazon S3 bucket.

Step 2: Create AWS Glue Crawler

Configured a Glue Crawler to identify the source data structure and discover its schema.

Step 3: Data Catalog

The crawler creates or updates the corresponding table metadata in the AWS Glue Data Catalog.

Step 4: ETL Transformation

Created an AWS Glue ETL job to read the source data, process it, and convert it into JSON format.

Step 5: Store Transformed Data

The final JSON output is stored in the destination Amazon S3 bucket.

📂 Repository Structure

aws-glue-etl-txt-to-json-pipeline/
│
├── data/
├── scripts/
├── architecture/
├── screenshots/
└── README.md

📸 Project Screenshots

Screenshots of the AWS implementation, including S3 buckets, Glue Crawler, Data Catalog, ETL Job, and transformed JSON output, are available in the screenshots folder.

📚 Key Learnings

- Understanding ETL pipeline architecture.
- Working with Amazon S3.
- Creating and configuring AWS Glue Crawlers.
- Understanding AWS Glue Data Catalog.
- Data format conversion (TXT to JSON).
- Working with cloud-based data processing.

🚀 Future Improvements

- Automate pipeline execution using AWS Glue Triggers.
- Add error handling and logging.
- Implement data quality checks.
- Explore workflow orchestration using AWS Glue Workflows.

👨‍💻 Author

Dhiraj Kumar

B.Tech CSE | IoT Specialization

Interested in Data Engineering, AWS Cloud, Python, SQL, and ETL Pipelines.
