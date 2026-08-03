\# AWS Day 9 – Amazon S3 (Simple Storage Service)



\## Overview



On Day 9, I learned about Amazon S3 (Simple Storage Service), AWS's object storage service used to store and retrieve data from anywhere over the internet. I explored its features, created an S3 bucket, uploaded files, configured IAM permissions, enabled static website hosting, applied bucket policies, enabled versioning, and learned resource tagging.



\---



\## Topics Covered



\- Introduction to Amazon S3

\- Buckets and Objects

\- Advantages of Amazon S3

\- Creating an S3 Bucket

\- Uploading Files and Folders

\- IAM User Permissions

\- AmazonS3FullAccess Policy

\- Bucket Policies

\- Restricting Bucket Access

\- Static Website Hosting

\- Block Public Access

\- Bucket Versioning

\- Bucket Tags



\---



\## What I Learned



\### What is Amazon S3?



Amazon S3 (Simple Storage Service) is an object storage service that allows users to store and retrieve any amount of data from anywhere using HTTPS.



Data is stored inside \*Buckets, and every file stored inside a bucket is called an \*\*Object\*.



Examples of objects include:



\- Images

\- Videos

\- Documents

\- CSV Files

\- HTML Files

\- Application Files



\---



\## Features of Amazon S3



\- Highly Scalable

\- Highly Available

\- Highly Durable

\- Secure

\- Cost Effective

\- Reliable Performance



A single bucket can store almost unlimited data, while an individual object can be up to \*5 TB\* in size.



\---



\## Practical Implementation



\### Creating an S3 Bucket



\- Open AWS Console

\- Search for Amazon S3

\- Create a new bucket

\- Select the AWS Region

\- Provide a unique bucket name

\- Upload files such as index.html



\---



\### IAM User Permissions



Created an IAM user and initially verified that the user had no permissions to access S3.



Granted permissions by attaching the \*AmazonS3FullAccess\* policy so the user could view and download objects from the bucket.



\---



\### Restricting Bucket Access



Configured a Bucket Policy to deny access even if an IAM user has permissions.



Used:



\- Effect: Deny

\- Principal

\- Action: S3 Actions

\- Resource: Bucket ARN

\- Condition using aws:PrincipalArn



This allows only specific principals to access the bucket.



\---



\### Static Website Hosting



Configured the bucket to host a static website by:



\- Enabling Static Website Hosting

\- Setting index.html as the Index Document

\- Disabling Block Public Access

\- Adding the required Bucket Policy

\- Accessing the website through the Static Website Endpoint



\---



\### Bucket Versioning



Enabled Bucket Versioning to maintain multiple versions of uploaded files.



Benefits include:



\- Protecting against accidental deletion

\- Recovering previous versions

\- Maintaining object history



\---



\### Bucket Tagging



Added tags to organize AWS resources.



Example:



\- Key: Project

\- Value: App1



Tags help identify resources belonging to different projects.



\---



\## Key Takeaways



\- Learned how Amazon S3 stores objects inside buckets.

\- Created and configured an S3 bucket.

\- Managed access using IAM policies and Bucket Policies.

\- Hosted a static website on S3.

\- Enabled Bucket Versioning for data protection.

\- Used Tags to organize AWS resources.

\- Understood how public access and bucket permissions work.



\---



\## Skills Learned



\- Amazon S3

\- IAM

\- Bucket Policies

\- Static Website Hosting

\- Versioning

\- Object Storage

\- Access Management

\- Resource Tagging

\- AWS Management Console

