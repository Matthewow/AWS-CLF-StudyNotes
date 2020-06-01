# Overview of AWS Web Services

Hi there! 

This is a self optimized personal study notes for AWS Certificated Cloud Practitioner training whitepaper summarized by Matthew WANG. 

The contents are mostly noted down from the source pages as below. Should you have any enquires, please get in touch with me at ***matthewwang dot my at gmail dot com.***

[https://www.youtube.com/watch?v=3hLmDS179YE&t=26s](https://www.youtube.com/watch?v=3hLmDS179YE&t=26s)

Online course online 

[https://www.youtube.com/watch?v=3hLmDS179YE&t=26s](https://www.youtube.com/watch?v=3hLmDS179YE&t=26s)

Official Whitepaper

[https://d0.awsstatic.com/whitepapers/aws-overview.pdf](https://d0.awsstatic.com/whitepapers/aws-overview.pdf)

Other website(s):

[https://digitalcloud.training/certification-training/aws-certified-cloud-practitioner/](https://digitalcloud.training/certification-training/aws-certified-cloud-practitioner/)

# 1. Cloud Concepts

## 1.1 What is Cloud Computing?

Cloud computing is the **on-demand delivery** of **computing power**, **database storage**, **applications**, and **other IT resources** through a cloud services platform via the Internet with pay-as-you-go pricing.

On premise (私有部署):

- Users own the servers
- Users hire the IT people
- Users pay or rent the real estate
- Users take all the risk

With Cloud Provider:

- Users are only responsible for configuring the cloud services and code.

## 1.2 Six Advantages of Cloud Computing

1. Trade capital expense for variable expense. No upfront cost
2. Benefit from massive economies of scale.
3. Stop guessing capacity.
4. Increase speed and agility.
5. Stop spending money running and maintaining data centers.
6. Go global in minutes.

## 1.3 Types of Cloud Computing

### 1.3.1 Cloud Computing Models

- **Infrastructure as a Service (IaaS),** For Admins
- **Platform as a Service (PaaS)**, For developer
- **Software as a Servcie (SaaS),** For users

### 1.3.2 Cloud Computing Deployment Models

- **Cloud** A cloud-based application is fully deployed in the cloud and all parts of the application run in the cloud. 
**Fully utilize cloud computing.**
For Start-Ups, offering SaaS
- **Hybrid** A hybrid deployment is a way to connect infrastructure and applications between cloud-based resources and existing resources that are not located in the cloud.
Banks, Fintechs
- **On-premises:** The deployment of resources on-premises, using virtualization and resource management tools, is sometimes called the “private cloud.”
Public sectors, like Gov
Sensitive Data, like hospital 
A large enterprise with regulations

# 2. Global Infrastructure

AWS Cloud operates in over 60 Availability Zones within over 20 geographic Regions around the world.

## 2.1 Region:

- A physical location in the world where we have multiple Availability Zones.
- **Geographically distinct.**
- **US-EAST: edging one**

## 2.2 Availability Zones:

- One or more physically discrete data centers, each with redundant power, networking, and connectivity, housed in separate facilities.
- **Each Availability Zone is designed as an independent failure zone.**
- ****Availability Zones are all **redundantly** connected to multiple tier-1 transit providers.
- letter identifier like us-east-1a (a refers to AZ number)
- <10ms latency between AZs

## 2.3 Edge location:

- Data centers owned by AWS trusted partners.
- Direct connection to AWS network
- Low latency

# 3. Hands on concepts

## 3.1 Amazon EC2 (Elastic Compute Cloud)

- A web service that provides secure, resizable compute capacity in the cloud.
- quickly scale capacity, both up and down, as your computing requirements change.
- Instance types:
**On-Demand Instances**
**Reserved Instances**
**Spot Instances**, bid on spare Amazon EC2 computing capacity.
- **Session manager**: Provides a browser-based interactive shell and CLI for managing Windows and Linux EC2 instances, without the need to open inbound ports, manage SSH keys, or use bastion hosts.

## 3.2 Auto Scaling

Maintain application availability and allows you to automatically add or remove EC2 instances according to conditions you define.

## 3.3 Elastic Load Balancing

Automatically distributes incoming application traffic across multiple targets, such as Amazon EC2 instances, containers, and IP addresses.

It can handle the varying load of your application traffic in a single Availability Zone or across multiple Availability Zones

- Application Load Balancer: HTTP & HTTPS
- Network Load Balancer: TCP
- Classic Load Balancer: basic load balancing across multiple Amazon EC2 instances

## 3.4 Simple Storage Service (S3)

An object storage service that offers industry-leading scalability, data availability, security, and performance.

## 3.5 CloudFront

A fast content delivery network (CDN) service that securely delivers data, videos, applications, and APIs to customers.

- integrated with AWS –both **physical location**s that are directly connected to the AWS global infrastructure, as well as **other AWS services**.
- works seamlessly with services including AWS Shield for DDoS mitigation, Amazon S3, Elastic Load Balancing or Amazon EC2.
- has a domain name, will redirect the traffic to this domain name.

## 3.6 Relational Database Service (RDS)

- Amazon Aurora is fully managed by Amazon Relational Database Service (RDS), which automates time-consuming administration tasks like hardware provisioning, database setup, patching, and backups.
- makes it easy to set up, operate, and scale a relational database in the cloud.
- provides you with six familiar database engines to choose from, including Amazon Aurora, PostgreSQL, MySQL, MariaDB, oracle database, and SQL Server. You can use the AWS Database Migration Service to easily migrate or replicate your existing databases to Amazon RDS.

## 3.7 AWS Lambda

- Run code without provisioning or managing servers.
- Only run small amount of time.
- Being able to see the configuration and logs.

# 4. Pricing Model

![Overview%20of%20AWS%20Web%20Services%/Untitled.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled.png)

## 4.1 On-Demand

- no up front payment
- no long term commitment

## 4.2 Reserved Instances(RI)

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%201.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%201.png)

## 4.3 Spot Instances

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%202.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%202.png)

## 4.4 Dedicated Host Instances

**Isolated hardware**

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%203.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%203.png)

## 4.5 CheatSheet

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%204.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%204.png)

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%205.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%205.png)

# 5. Billing and Pricing

## 5.1 Free services

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%206.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%206.png)

## 5.2 AWS Support Plans

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%207.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%207.png)

concierge: 看门人

TAM: Technical Account Manager

## 5.3 AWS Marketplace

Find Buy Deploy

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%208.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%208.png)

## 5.4 AWS Trusted Advisor

- Advises you on security, saving money, performance, service limits and fault tolerance.
- A automated checklist.

[For detailed 5 categories ](https://www.notion.so/For-detailed-5-categories-5be7ddc1aa1548f89a20b92951654562)

## 5.5 Consolidated Billing

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%209.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%209.png)

### Consolidated Billing Volume Discounts

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2010.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2010.png)

## 5.6 AWS Cost Explorer

- Being able to know the forecast cost.
- Breakdown cost

 

## 5.7 AWS Budgets

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2011.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2011.png)

## 5.7 Total Cost of Ownership (TCO) Calculator

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2012.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2012.png)

## 5.8 AWS Landing Zone

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2013.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2013.png)

## 5.9 Resource Groups and Tagging

**Resource groups:** 

Lets you create a logical group of resources associated with a particular workload such as different layers of an application stack, or production versus development environments. 

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2014.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2014.png)

## 5.10 AWS QuickStart

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2015.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2015.png)

# 6. Technology Overview

## 6.1 AWS Organization and Accounts

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2016.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2016.png)

Where the root user is the master account.

## 6.2 AWS Networking

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2017.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2017.png)

VPC: Virtual Private Cloud

## 6.3 Database Services

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2018.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2018.png)

DynamoDB: key-value and document database that delivers single-digit millisecond performance at any scale.

Redshift: handle a huge amount of data.

## 6.4 Provisioning Services

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2019.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2019.png)

**Elastic Beanstalk:** simply upload your code, and AWS Elastic Beanstalk automatically handles the deployment, from capacity provisioning, load balancing, and auto-scaling to application health monitoring.

**Chef and Puppet:** are automation platforms that allow you to use code to automate the configurations of your servers.

## 6.5 Computing Services

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2020.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2020.png)

**Amazon ECS** eliminates the need for you to install and operate your own container orchestration software, manage and scale a cluster of virtual machines, or schedule containers on those virtual machines. Only pay for the run time and CPU used.

**Fargate**: a compute engine for Amazon ECS that allows you to run containers without having to manage servers or clusters.

## 6.6 Storage Services

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2021.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2021.png)

**Storage Gateway:** 
a hybrid storage service that enables your **on-premise**s applications to seamlessly use AWS cloud storage. You can use the service for **backup** and archiving, disaster **recovery**, cloud data processing, storage tiering, and migration.

**EBS:** 
provides **persistent** block storage volumes for use with Amazon EC2 instances in the AWS Cloud. Each Amazon EBS volume is **automatically replicated** within its Availability Zone to protect you from component failure, offering high availability and durability.

**EFS:**
Similar to EBS, while multiple EC2 can access the storage.

**Snowball:**
a petabyte-scale data transport solution that uses secure appliances to transfer large amounts of data into and out of AWS.

## 6.7 Business Centric Services

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2022.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2022.png)

## 6.8 Enterprise Integration

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2023.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2023.png)

## 6.9 Logging Services

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2024.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2024.png)

## 6.10 Know your Initialisms

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2025.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2025.png)

# 7. Security

## 7.1 Shared Responsibility Model

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2026.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2026.png)

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2027.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2027.png)

## 7.2 AWS Compliance programs

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2028.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2028.png)

## 7.3 AWS Artifact

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2029.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2029.png)

## 7.3 Amazon Inspector

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2030.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2030.png)

## 7.4 AWS WAF

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2031.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2031.png)

## 7.5 AWS Shield

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2032.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2032.png)

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2033.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2033.png)

## 7.6 Penetration Testing

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2034.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2034.png)

## 7.7 Guard Duty

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2035.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2035.png)

## 7.8 Key Management Service

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2036.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2036.png)

## 7.9 Amazon Macie

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2037.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2037.png)

## 7.10 Security Groups vs NACLs

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2038.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2038.png)

You can deny a particular IP address using NACLs.

## 7.11 AWS VPN

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2039.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2039.png)

# 8. Variation Study

## 8.1 Cloud* Service

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2040.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2040.png)

## 8.2 Connect Service

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2041.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2041.png)

## 8.3 Elastic Transcoder vs. Media Convert

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2042.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2042.png)

## 8.4 SNS vs SQS

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2043.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2043.png)

SNS: like billing emails

SQS: for delay test

## 8.5 Inspector vs Trusted Advisor

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2044.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2044.png)

Inspector: only EC2 instance

Trusted advisor: multiple aspects

## 8.6 ALB vs NLB vs CLB

Load Banlancer

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2045.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2045.png)

Layer 7 is the application layer.

Layer 4 is transprt layer

## 8.7 SNS vs SES

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2046.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2046.png)

SNS: internal and practical purposes. No HTML emails.

SES: Professional and marketing purposes. Optimized for emails.

## 8.8 Artifact vs Inspector

![Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2047.png](Overview%20of%20AWS%20Web%20Services%20b0d1671c1f454aaeab23e9228fcc9fba/Untitled%2047.png)

# 9. Supplementary Concepts

 

- **Amazon Cognito:**
lets you add user sign-up, sign-in, and access control to your web and mobile apps quickly and easily. Amazon Cognito scales to millions of users and supports sign-in with social identity providers, such as Facebook, Google, and Amazon, and enterprise identity providers via SAML 2.0
- **APN Consulting Partners:**
are professional services firms that help customers of all sizes design, architect, build, migrate, and manage their workloads and applications on AWS. Consulting Partners include System Integrators (SIs), Strategic Consultancies, Agencies, Managed Service Providers (MSPs), and Value-Added Resellers (VARs).
- **Shared Controls:**
Controls which apply to both the infrastructure layer and customer layers, but in completely separate contexts or perspectives
- **Patch Management**– 
AWS is responsible for patching and fixing flaws within the infrastructure, but customers are responsible for patching their guest OS and applications
- **Configuration Management**– 
AWS maintains the configuration of its infrastructure devices, but a customer is responsible for configuring their own guest operating systems, databases, and applications
- **Service and Communications Protection-**
It is an example of a customer-specific control
- **Amazon Elastic Map Reduce (EMR)-**
provides a managed Hadoop framework that makes it easy, fast, and cost-effective to **process vast amounts of data** across dynamically scalable Amazon EC2 instance. (For data analysis)
- **Amazon Athena:**
It is an interactive query service that makes it easy to analyze data in Amazon S3 using standard SQL.
- **AWS Systems Manager**
gives you visibility and control of your infrastructure on AWS. Systems Manager provides a unified user interface so you can view operational data from multiple AWS services and allows you to automate operational tasks across your AWS resources.
- **AWS OpsWorks:**
It is a configuration management service that provides managed instances of Chef and Puppet.
- **AWS Config:**
it is a fully-managed service that provides you with an AWS resource inventory, configuration history, and configuration change notifications to enable security and regulatory compliance.
- **Amazon CloudWatch:**
is a monitoring service for AWS cloud resources and the applications you run on AWS. You use CloudWatch for performance monitoring, not automating operational tasks.
- **5 Pillars of the AWS Well-Architected Framework**
Operational Excellence
Security
Reliability
Performance Efficiency
Cost Optimization 
Detailer may see below:

[The 5 Pillars of the AWS Well-Architected Framework | Amazon Web Services](https://aws.amazon.com/blogs/apn/the-5-pillars-of-the-aws-well-architected-framework/)
