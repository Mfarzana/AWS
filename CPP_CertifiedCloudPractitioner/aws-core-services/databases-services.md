# Database Services and Utilites

## Amazon RDS 
**Amazon Relational Database Service** makes it easy to set up, operate, and scale a relational database in the cloud. **Launches into a VPC**. Provide both general purpose SSD and provisioned IOPS SSD drive options.
You can use the **AWS Database Migration Service to easily migrate or replicate your existing databases to Amazon RDS**.
### Amazon RDS Platforms
**Amazon Aurora, PostgreSQL, MySQL, MariaDB, Oracle Database, and SQL Server**.
* **Amazon Aurora** is a **MySQL and PostgreSQL-compatible relational database built for the cloud**, that combines the performance and availability of traditional enterprise databases with the simplicity and cost-effectiveness of open source databases.
### Amazon Database Migration Service (DMS)
* Enables you to move data into AWS from existing databases.
* Support both one time and continual migration of data.
* Support many popular commercial and open source databases.
* Only pay for compute leverage in the migration process. 

## Amazon DynamoDB
* Fully managed **NoSQL database service** 
* Provides both **key-value and document database** 
* Enables extremely low latency at virtually any scale
* Support automated scaling based on configuaration 
* Offers in memory cache with DynamoDB Acceleration (DAX)
```diff
! DynamoDB can handle more than 10 trillion request per day and can support peaks of more than 20 million request per second .
```
### Use Cases
* Scale without excesssive maintenace
* Serverless application
* Implementatins where low latency is key
* Data models without BLOB storage

## Reference
* https://aws.amazon.com/rds/
* https://aws.amazon.com/dynamodb/
