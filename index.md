#### AWS Compute Services 
- **AWS Elastic Computing Cloud** 
  - It is virtual server.
  - OS selection from AMI (Amazon Machine Image).
  - Elasticity - we can scale the no of instance as per our need.
  - Types of EC2 instances  
	- General Purpose
	- Compute optimized - High performing web server, video encoding 
	- Memory Optimized - High performance databases and Dist. Memory Cache
	- Storage Optimized  - Data warehousing, data processing apps
	- Accelarated computing - ML, 3D visualizations
  - Unmanaged service


- **AWS Serverless computing**
  - **AWS Lambda**
	- Fully managed compute service
	- Runs stateless code
	- Runs you code on schedule or in response to event such as HTTP request or response

 - Other use cases are also served through varies serverless compute services in AWS.

- **AWS Elastic Container Service**
  -  Provides contianer orchestration on EC2


#### Storage Service

- **Amazon S3**
  - Object storage
  - Objects are stored in the buckets
  - Immediately accesible
  - Static web hosting also can be done
  - Can store an unlimited number of objects in a bucket
- **Amazon S3 Glacier**
  - Archive Storage
  - Long term storage
  - Cheaper than S3
  - Cold data is stored here
  - Low cost storage
  - Data retrievel frequency is low
- **Amazon EFS**
  - Network storage for EC2 storage
- **Amazon Storage Gateway**
  - Cloud storage 
- **Amazon EBS**
  - Network attached volumes that provides block-level storage for Amazon EC2 instances.
  - Persistent block storage
  - Different drive types
  - Encryption available
  - Snapshot functionality


#### Databases 

- SQL 
  - Transactional databases
    - Amazon RDS 
	- Supports
		- Amazon Aurora - MYSQL and PostGresSQL compatible relational built for cloud, it is serverless as well as an option
		- MS SQL Server
		- Maria DB
		- ORACLE
		- PostgreSQL
		- MySQL
  Data Analytics or Relationships
    - Amazon Redshift
- NoSQL
  - Transaction Databases
    - Amazon DynamoDB
	- Fast and flexible
  - Data Analytics or Relationships (Graph)
    - Amzon Neptune
  - In memory 
    - Amazon ElastiCache or Redis


#### Network

- **AWS Virtual Private Cloud**
  - Private network for our workload
  -  Can divide VPC into subnets 
  - It is a regionally scoped service, where as subnets is AZ zone scoped. Cannot have a single VPC expanding our multiple regions.
  - VPC can be connected together.
  - Network Security Groups is used to allow traffic to/from at network interface level. 
  - Network Access Control Lists - Allow/deny traffic in and out of subnets.
  - Layers of Network Security - VPC - Internet Gateway - Route Tables - Network Access Control Lists  - Subnet - You Own Firewall Software - EC2 instance.

- **AWS Elastic Load Balancer**
  - Application load balancer works upon the HTTP and HTTPS protocol and determines which instance would serve the incoming request.

- **Amazon Route 53**
  - Route 53 is DNS service and translates domain names into IP Addresses.
  - Can use same domain name thorughout multiple regions
  - Browser -> Route 53 -> VPCs -> EC2 instances

#### Security
 - Shared responsibility on cloud from customer and AWS.
 - AWS IAM 
	- Authentication and Authorization management 
	- Users - application or person
	- Groups
	- Roles - policy or permission based roles
- AWS CloudTrail
  - Track user activity & API usage
  - Stores log in s3

- AWS Trusted Advisor
  - Provides guidance to help you reduce cost, increase performance, and improve security


#### Iot & ML
- AWS greengrass
	- Provides runtime to locally run AWS lambda, messaging 
	- Device with IoT Sdk can interact with Greengrass on local network

- AWS Sagemaker
	- Prepare, Build, Train and Tune, Deploy and Manage the Ml model using this single service

- AWS Rekognition 
	- Object & Scene recognition
	- Facial recognition

#### Blockchain
- AWS Blockchain services
  - Fully managed service
  - Lets you create scalable blockchain networks using frameworks OS
	- Hyperledger Fabric 
	- Ethereum

#### Other Services
- AWS Ground Station
  - Fully managed service
  - Lets you control satelite communication  
 - Use cases
  - Weather forecasting & Agriculture
  - Global shipping 
  - Earth observation and fire safety
  - Retail forecasting

- AWS Wavelength
  - Combines high bandwidth and ultra low latency of 5G networks with AWS compute and storage services to enable devs to innovate.
  - AWS compute and storage infrastructue embedded inside CSP mobile network.


