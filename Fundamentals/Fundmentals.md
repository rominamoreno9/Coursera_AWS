# AWS Fundamentals 

## What is the AWS term for physically distinct groups of data centers?

Availability Zone

## AMI (Amazon Machine Image)

Is a template that contains a software configuration such as an operating system, application server and applications

## Amazon EC2 (Elastic Compute Cloud)

Web service that provides secure and resizable compute capacity in the cloud

* [EC2](https://aws.amazon.com/ec2/)

* [Instance-types](https://aws.amazon.com/ec2/instance-types/)

## Amazon Lightsail

Use compute capacity without worrying about provisioning or managing underlying hardware

* [Lightsail](https://aws.amazon.com/lightsail/)
* https://www.youtube.com/watch?v=29_LqYnomdg


## **Network**

## Amazon VPC (Amazon Virtual Private Cloud)

Amazon Virtual Private Cloud (Amazon VPC) lets you provision a logically isolated section of the AWS Cloud where you can launch AWS resources in a virtual network that you define. You have complete control over your virtual networking environment, including the selection of your own IP address range, the creation of subnets, and the configuration of route tables and network gateways. You can use both IPv4 and IPv6 in your VPC for secure and easy access to resources and applications. You could create up to five non-default VPCs per AWS account per Region. (See below for information about default VPCs.)

* https://aws.amazon.com/vpc
* https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html
* https://docs.aws.amazon.com/vpc/latest/userguide/default-vpc.html

## **Storage**

## Amazon EBS (Elastic Block Storage) 

Provides persistent block storage volumes for use with Amazon EC2 instances in the AWS Cloud

* [EBS](https://aws.amazon.com/ebs)

## Amazon S3 (Amazon Simple Storage Service)

Stores data as objects within resources that are called buckets

* [S3](https://aws.amazon.com/s3)

## Amazon EFS (Elastic File System)

* [EFS](https://aws.amazon.com/efs/)

## Advantages of Amazon EFS (Elastic File System) over Amazon EBS (Elastic Block Storage)

EFS can be attached to multiple EC2 instances simultaneously

## **Databases**

## Amazon RDS (Cloud Relational Database)

A database engine that can be used with MySQL server, Oracle, Microsoft SQL server, PostgreSQL and Amazon Aurora

* [AWS Database Migration Service (AWS DMS)](https://aws.amazon.com/dms)
* https://aws.amazon.com/rds/pricing/

## Amazon DynamoDB

A fast and flexible NoSQL database service for applications that need consistent, single-digit millisecond latency at any scale
You don't need to define the underlying hardware you're running your database on

* https://aws.amazon.com/dynamodb

* Databases and EC2 instances are most performant using block-level storage

## **Monitoring**

## Amazon CloudWatch

A monitoring service for AWS Cloud resources and the applications that you run on AWS. You can use Amazon CloudWatch to collect and track metrics, collect and monitor log files, set alarms, and automatically react to changes in your AWS resources.

* [CLoudWatch](https://aws.amazon.com/cloudwatch/)
* [Events](https://docs.aws.amazon.com/AmazonCloudWatch/latest/events/WhatIsCloudWatchEvents.html)
* [Logs](https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/WhatIsCloudWatchLogs.html)
* [Metris](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CW_Support_For_AWS.html)


## **Scaling**

## Amazon ELB (Elastic Load Balancing)

Automatically distributes incoming application traffic across multiple targets, such as Amazon EC2 instances, containers, and IP addresses. It can handle the varying load of your application traffic in a single Availability Zone or across multiple Availability Zones.

* [ELB](https://aws.amazon.com/elasticloadbalancing/)

## Auto Scaling

Helps you maintain application availability, and it allows you to dynamically scale your Amazon EC2 capacity up or down automatically according to conditions that you define

* [Auto Scaling](https://aws.amazon.com/ec2/autoscaling)

* Increases or decreases compute resources on demand to meet your deployment needs and minimize costs

## **Security**

## Amazon Shared Responsibility Model
Security in the Cloud: Customer responsibility will be determined by the AWS Cloud services that a customer selects. This determines the amount of configuration work the customer must perform as part of their security responsibilities.

* [Shared Responsibility Model](https://aws.amazon.com/compliance/shared-responsibility-model/)


## **Cost Management**

## AWS Pricing Calculator

Can be used to calculate Amazon EC2 and Amazon EBS pricing

* [AWS Pricing Calculator](https://calculator.aws/#/)

## AWS Cost Explorer

Lets you visualize, understand, and manage your AWS costs and usage over time. You can create custom reports (including charts and tabular data) that analyze cost and usage data, both at a high level (e.g., total costs and usage across all accounts) and for highly specific requests (e.g., m2.2xlarge costs within account Y that are tagged project: secretProject).

* [AWS Cost Explorer](https://aws.amazon.com/aws-cost-management/aws-cost-explorer/)

## AWS Trusted Advisor

Online tool that helps you configure resources to follow best practices

* [AWS Trusted Advisor](https://aws.amazon.com/premiumsupport/trustedadvisor/)
