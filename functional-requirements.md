# Functional Requirements

## **Functional Requirements**

This feature will make available entire customer historical billing data \(GCP and AWS\) to support the use cases defined above. 

In addition, this infrastructure will enable us, in the future, to import additional types of data if the need arises in future.

High-level example of a use case 1:

1. Users land into a registration web page and registers with CMP
2. Users log in to CMP and goes to the Setting page
3. Users upload a SA for Google or provide ARN to AWS which will allow us to backfill their billing data. Following this, the backfill process will start and will backfill client information

* For BigQuery the data is in a BQ billing table which we need to identify and extend the Moshe’s process. 
* For AWS the data will be in a CUR file in S3 bucket which we need to identify and extend Tomer process

   4.There will be a hourly process of fetching incremental billing data

