# **Data Protection**

## Data Types

* [S3](https://aws.amazon.com/s3/)
    Customers of all sizes and industries can use it to store and protect any amount of data for a range of use cases, such as websites, mobile applications, backup and restore, archive, enterprise applications, IoT devices, and big data analytics

* [S3 Glacier](https://aws.amazon.com/glacier/ )
    Secure, durable, and extremely low-cost cloud storage service for data archiving and long-term backup. It is designed to deliver 99.999999999% durability, and provides comprehensive security and compliance capabilities that can help meet even the most stringent regulatory requirements

* [Amazon RDS](https://aws.amazon.com/rds/)

* [Amazon DynamoDB](https://aws.amazon.com/dynamodb/ )

* [Amazon Timestream](https://aws.amazon.com/timestream/ )
    Database service for IoT and operational applications that makes it easy to store and analyze trillions of events per day at 1/10th the cost of relational databases

* [Amazon Quantum Ledger Database (QLDB)](https://aws.amazon.com/qldb/)
    Amazon QLDB is a fully managed ledger database that provides a transparent, immutable, and cryptographically verifiable transaction log ‎owned by a central trusted authority. Amazon QLDB tracks each and every application data change and maintains a complete and verifiable history of changes over time.
    Amazon QLDB is a new class of database that eliminates the need to engage in the complex development effort of building your own ledger-like applications. With QLDB, your data’s change history is immutable – it cannot be altered or deleted – and using cryptography, you can easily verify that there have been no unintended modifications to your application’s data.

* [Amazon Elastic Block Store](https://aws.amazon.com/ebs/)
    Amazon Elastic Block Store (EBS) is an easy to use, high performance block storage service designed for use with Amazon Elastic Compute Cloud (EC2) for both throughput and transaction intensive workloads at any scale. A broad range of workloads, such as relational and non-relational databases, enterprise applications, containerized applications, big data analytics engines, file systems, and media workflows are widely deployed on Amazon EBS

* [Amazon Elastic File System](https://aws.amazon.com/efs/)
    Amazon Elastic File System (Amazon EFS) provides a simple, scalable, elastic file system for Linux-based workloads for use with AWS Cloud services and on-premises resources.  Amazon EFS is well suited to support a broad spectrum of use cases from highly parallelized, scale-out workloads that require the highest possible throughput to single-threaded, latency-sensitive workloads. Use cases such as lift-and-shift enterprise applications, big data analytics, web serving and content management, application development and testing, media and entertainment workflows, database backups, and container storage

* [Amazon Redshift](https://aws.amazon.com/redshift/ )    
    Amazon Redshift extends data warehouse queries to your data lake, with no loading required. You can run analytic queries against petabytes of data stored locally in Redshift, and directly against exabytes of data stored in Amazon S3. It is simple to set up, automates most of your administrative tasks, and delivers fast performance at any scale

* [Amazon Athena](https://aws.amazon.com/athena/ )    
    Amazon Athena is an interactive query service that makes it easy to analyze data in Amazon S3 using standard SQL. Athena is serverless, so there is no infrastructure to manage, and you pay only for the queries that you run.
    Athena is easy to use. Simply point to your data in Amazon S3, define the schema, and start querying using standard SQL. Most results are delivered within seconds. With Athena, there’s no need for complex ETL jobs to prepare your data for analysis. This makes it easy for anyone with SQL skills to quickly analyze large-scale datasets.

## Data Transfer

* [AWS Snowball](https://aws.amazon.com/snowball/ )
    Snowball is a petabyte-scale data transport solution that uses devices designed to be secure to transfer large amounts of data into and out of the AWS Cloud.   Snowball devices use tamper-resistant enclosures, 256-bit encryption, and an industry-standard Trusted Platform Module (TPM) designed to ensure both security and full chain-of-custody for your data

* [AWS Snowmobile](https://aws.amazon.com/snowmobile/ )    
    AWS Snowmobile is an Exabyte-scale data transfer service used to move extremely large amounts of data to AWS. You can transfer up to 100PB per Snowmobile, a 45-foot long ruggedized shipping container, pulled by a semi-trailer truck. Snowmobile makes it easy to move massive volumes of data to the cloud, including video libraries, image repositories, or even a complete data center migration. Transferring data with Snowmobile is more secure, fast and cost effective


## Encryption in Transit and at Rest
In this section, Rudy and Hong discussed data encryption in transit and at rest.

**Encryption of Data in Transit**

You can mount a file system so all NFS traffic is encrypted in transit using Transport Layer Security 1.2 (TLS, formerly called Secure Sockets Layer [SSL]) with an industry-standard AES-256 cipher. TLS is a set of industry-standard cryptographic protocols used for encrypting information that is exchanged over the wire. AES-256 is a 256-bit encryption cipher used for data transmission in TLS. If your organization is subject to corporate or regulatory policies that require encryption of data and metadata in transit, we recommend setting up encryption in transit on every client accessing the file system. More information on Encryption of data in transit can be found at: https://docs.aws.amazon.com/whitepapers/latest/efs-encrypted-file-systems/encryption-of-data-in-transit.html

**Encryption of Data at Rest**

You can create an encrypted file system so all your data and metadata is encrypted at rest using an industry-standard AES-256 encryption algorithm. Encryption and decryption is handled automatically and transparently, so you don’t have to modify your applications. If your organization is subject to corporate or regulatory policies that require encryption of data and metadata at rest, we recommend creating an encrypted file system.

**AWS Key Management Service (KMS)**

AWS Key Management Service (KMS) makes it easy for you to create and manage keys and control the use of encryption across a wide range of AWS services and in your applications. AWS KMS is a secure and resilient service that uses FIPS 140-2 validated hardware security modules to protect your keys. AWS KMS is integrated with AWS CloudTrail to provide you with logs of all key usage to help meet your regulatory and compliance needs. More details on AWS KMS can be found at: https://aws.amazon.com/kms/

* Customer master keys (CMKs)
Customer master keys are the primary resources in AWS KMS.
A customer master key (CMK) is a logical representation of a master key. The CMK includes metadata, such as the key ID, creation date, description, and key state. The CMK also contains the key material used to encrypt and decrypt data.

**AWS CloudHSM**

AWS CloudHSM is a cloud-based hardware security module (HSM) that enables you to easily generate and use your own encryption keys on the AWS Cloud. With CloudHSM, you can manage your own encryption keys using FIPS 140-2 Level 3 validated HSMs. CloudHSM offers you the flexibility to integrate with your applications using industry-standard APIs, such as PKCS#11, Java Cryptography Extensions (JCE), and Microsoft CryptoNG (CNG) libraries. CloudHSM is standards-compliant and enables you to export all of your keys to most other commercially-available HSMs, subject to your configurations. It is a fully-managed service that automates time-consuming administrative tasks for you, such as hardware provisioning, software patching, high-availability, and backups. CloudHSM also enables you to scale quickly by adding and removing HSM capacity on-demand, with no up-front costs. More information on AWS CloudHSM can be found at: https://aws.amazon.com/cloudhsm/


## Database Encryption
## Encryption at rest and in transit

**Amazon RDS** allows you to encrypt your databases using keys you manage through AWS Key Management Service (KMS). On a database instance running with Amazon RDS encryption, data stored at rest in the underlying storage is encrypted, as are its automated backups, read replicas, and snapshots.
Amazon RDS supports Transparent Data Encryption in SQL Server and Oracle. Transparent Data Encryption in Oracle is integrated with AWS CloudHSM, which allows you to securely generate, store, and manage your cryptographic keys in single-tenant Hardware Security Module (HSM) appliances within the AWS cloud.
Amazon RDS supports the use of SSL to secure data in transit.

**Network isolation**

AWS recommends that you run your database instances in Amazon VPC, which allows you isolate your database in your own virtual network and connect to your on-premises IT infrastructure using industry-standard encrypted IPsec VPNs. You can configure firewall settings and control network access to your database instances.

**Resource-level permissions**

Amazon RDS is integrated with AWS Identity and Access Management (IAM) and provides you the ability to control the actions that your AWS IAM users and groups can take on specific Amazon RDS resources, from database instances through snapshots, parameter groups, and option groups. You can also tag your Amazon RDS resources and control the actions that your IAM users and groups can take on groups of resources that have the same tag and associated value. For example, you can configure your IAM rules to ensure developers are able to modify "Development" database instances, but only Database Administrators can make changes to "Production" database 

Information on Amazon RDS Security can be found at​ https://aws.amazon.com/rds/features/#security

## Amazon S3 Default Encryption for S3 Buckets

**Amazon S3** default encryption provides a way to set the default encryption behavior for an S3 bucket. You can set default encryption on a bucket so that all objects are encrypted when they are stored in the bucket. The objects are encrypted using server-side encryption with either Amazon S3-managed keys (SSE-S3) or AWS KMS-managed keys (SSE-KMS).
When you use server-side encryption, Amazon S3 encrypts an object before saving it to disk in its data centers and decrypts it when you download the objects.  More details on using Encryption with Amazon S3 can be found at: https://docs.aws.amazon.com/AmazonS3/latest/dev/bucket-encryption.html

**Amazon Macie**


Amazon Macie is a security service that uses machine learning to automatically discover, classify, and protect sensitive data in AWS. Amazon Macie recognizes sensitive data such as personally identifiable information (PII) or intellectual property, and provides you with dashboards and alerts that give visibility into how this data is being accessed or moved. The fully managed service continuously monitors data access activity for anomalies, and generates detailed alerts when it detects risk of unauthorized access or inadvertent data leaks. Currently, Amazon Macie is available to protect data stored in Amazon S3.  More information about Amazon Macie is available at: https://aws.amazon.com/macie/


## EBS Encryption

Amazon EBS encryption offers seamless encryption of EBS data volumes, boot volumes and snapshots, eliminating the need to build and manage a secure key management infrastructure. EBS encryption enables data at rest security by encrypting your data volumes, boot volumes and snapshots using Amazon-managed keys or keys you create and manage using the AWS Key Management Service (KMS). In addition, the encryption occurs on the servers that host EC2 instances, providing encryption of data as it moves between EC2 instances and EBS data and boot volumes. For more information, see Amazon EBS encryption in the Amazon EC2 User Guide.

Access to Amazon EBS volumes is integrated with AWS Identity and Access Management (IAM). IAM enables access control to your Amazon EBS volumes. For more information, see AWS Identity and Access Management.  For more information about Amazon EBS encryption, see: https://aws.amazon.com/ebs/features/

## Cross Account Access to S3