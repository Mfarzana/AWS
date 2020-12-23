# AWS File Storage Services

## Amazon S3
**Amazon Simple Storage Service** (Amazon S3) is an **object storage** service that offers industry-leading scalability, data availability, security, and performance.
This means customers of **all sizes and industries can use** it to **store and protect any amount of data** for a range of use cases, such as data lakes, websites, 
mobile applications, **backup and restore, archive**, enterprise applications, IoT devices, and big data analytics.

* **Stores files as objects in buckets**
* Provides **different storage classes** for different use cases
* **Stores data** across **multiple availability zones**
* Unables **URL access for files**
* Offers configuration rules for data lifecyle
* **Can Serve as a static website host**

* ### Amazon S3 Non Archival Storage Classes
  * **S3 Standard**: is the **default storage** class and is **for frequently access data**
  * **S3 Intelligent-Tiering**: will move your data to the correct storage class based on usage
    * Automatically moves files based on access
    * Moves between frequent and infrequent access
    * Same performance as S3-Standard   
    > **S3 Intelligent-Tiering is the only cloud storage class that delivers automatic cost savings by moving objects between four access tiers when access patterns change**. 
    The S3 Intelligent-Tiering storage class is designed to optimize costs by automatically moving data to the most cost-effective access tier, without operational overhead.
  * **S3 Standard-IA**: is for **infrequently accessed data** with the standard resilience(/rəˈzilyəns/)
  * **S3 One Zone-IA**: is for **infrequently access data** that is **only one stored in one AZ**
* ### Amazon S3 Archival Storage Classes
  * **Amazon S3 Glacier**
    * S3 Galcier
    * S3 Glacier Deep Archive
    
    ```
              S3 Galcier                          |         S3 Glacier Deep Archive
     ---------------------------------------------| -------------------------------------
     Desinged for archival data                   | Desinged for archival data 
     90 day minimum storage duration change       | 180 day minimum storage duration change
     Can be retrieved either minutes or hours     | Can be retrieved either hours
     You pay a retrieval fee per GB per retrieved | You pay a retrieval fee per GB per retrieved
     Over 5 times less expensive than S3          | Over 23 times less expensive than S3 
      Standard storage class                      |       Standard storage class   
     
     ```
    

### S3 Lifecyle Policies
* Object in a bucket can transition or expire based on your criteria
* Transition can enable objects to move to another storage class based on time
* Expiratino can delete objects based on age
* Policies can also factor in versions of a specific object in the bucket
### S3 Transfer Acceleration 
Feature that can be enabled per bucket that allows for **optimized uploading of data using the AWS edge locations as part of Amazon CluudFront**.
```diff
S3 Transer Acceleratin upload data in your buckets much faster
! if you need upload data fast and efficient way in your S3 bujects you can consider utilizing S3 Transfer Acceleration
```
## Amazon Elastic Block Store( Amazon EBS )
  **Persistent block storage for use with Amazon EC2**.
  Persistent desinged to be connected to a single EC2 instance that can be scale to support petabytes of data and supports multiple volume types based on need.
  * Enable redundancy within an AZ
  * Allow users to take snapshots of its data
  * Offers encryption of its volumes
  * **Provides multiple volume types**
    * **General purpose SSD**: is a cost effective type designed for general workloads 
    * **Provisional IOPS SSD**: High performace volume for low latency application
    * **Throughput optimized HDD**: is designed for frequently access data
    * **Cold HDD**: is desinged for less frequently accessed workloads. 
  
## Amazon Elastic File System (Amazon EFS)
 * **Fully Managed NFS file system**
 * **Designed for Linux workloads**
 * Suport up to petabtye scale
 * Store data across multiple AZ's
 * Provide two different storage classes
   *  Standard
   * Infrequent Access
 * Provides configurable lifecycle data rules
 ```
 NFS: Network File System. It is protocal which allows user to access data and files remotely over the internet.
  It uses the Transmission Control Protocol (TCP) and User Datagram Protocol (UDP) for accessing and delivering the data and files.
 ```
## Amazon FSx for Windows File Server 
 * **Fully managed native windows file system**
 * Includes native windows features including
   * SMB Support 
   * Active Directory integration 
   * Windows NTFS
 * Utilize SSD drives for low latency
## AWS Snowball & AWS Snowmobile 
**Large Scale of Data Transfer into AWS**

```
              AWS Snowball                          |           AWS Snowmobile  
     ---------------------------------------------  | -------------------------------------
     Desinged for large-scale data transfer         | Desinged for large-scale data transfer 
     Supports petabyte scale transfer               |  Supports exrabyte scale transfer
     Physical device is delivered by AWS            | Ruggedized shipping container is delivered to your location
     You connect the Snowball to your network       | AWS sets up a connection to your network
                             and upload your data   | 
     AWS receives device and loads your data into S3| AWS will load data into S3 when the container is received at an AWS location                        
     
   
 ```
     
  > To migrate large datasets of 10PB or more in a single location, you should use Snowmobile. 
  For datasets less than 10PB or distributed in multiple locations, you should use Snowball
  
## References
* https://aws.amazon.com/s3/
* https://www.javatpoint.com/nfs
* https://aws.amazon.com/snowmobile/faqs/#:~:text=Q%3A%20How%20should%20I%20choose,locations%2C%20you%20should%20use%20Snowball.
