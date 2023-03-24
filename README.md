# Youtube-data-Analysis-using-AWS-and-Qlik

## Overview
This project is aimed at creating a centralized repository of structured and unstructured data using AWS S3 buckets and performing data warehousing and business intelligence tasks on the stored data. We have used AWS Lambda for data transformation, 
AWS Glue for crawling and cataloging the data, and AWS QuickSight to help companies effectively advertise their product in youtube to reach target audience based on regional and channel popularity.

## Project Steps
### Loading Data: 
We loaded the source data (JSON and CSV) into the first S3 bucket using the Extract, Load, and Transformation process.
### Creating a Data Lake: 
We transformed the JSON data to the Parquet file format using AWS Lambda and moved the transformed data to the second S3 bucket using AWS Glue crawler. We then transformed the CSV data to Parquet format and added it to the second S3 bucket as well.
### Data Cleaning: 
The second S3 bucket contains the cleaned and transformed data in the Parquet format.
### Automation: 
We plan to automate the loading of future incoming data using triggers.
### Data Catalog:
We used AWS Glue Studio catalog to join required tables and added it to the reporting bucket for further querying and business intelligence tasks.
### Machine Learning:
We plan to use AWS SageMaker to deploy an ML model for categorization of YouTube videos based on description and AWS Comprehend to implement sentiment analysis.
### Business Intelligence:
We plan to use AWS QuickSight to perform business intelligence tasks such as creating word clouds, bar charts, line charts, and bubble charts to count number of likes, count number of likes by snippet title, sum of views by snippet title, sum of views by region, and checking which category of videos had the most number of likes and views.
## Installation
Clone the repository
Install the required dependencies
Run the Python scripts in the 'scripts' folder to extract, transform, and load the data.
Run the AWS Glue crawler to move the transformed data to the second S3 bucket.
Use AWS Glue Studio to create a data catalog and join required tables.
Use AWS QuickSight to perform business intelligence tasks.
# Conclusion
This project successfully demonstrates the use of AWS services to create a centralized repository of data and perform data warehousing and business intelligence tasks on it. The use of AWS Lambda, AWS Glue, and AWS QuickSight has made the process of data transformation, data cleaning, and reporting much easier and efficient.
