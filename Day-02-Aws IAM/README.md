\# Day 02 - AWS Identity and Access Management (IAM)



\## 📌 Overview



On Day 2 of the AWS Zero to Hero series, I learned about \*AWS Identity and Access Management (IAM)\*, which is used to securely manage access to AWS resources. This session covered the core components of IAM and demonstrated how permissions affect resource accessibility.



\---



\## 🎯 Objectives



\- Understand the purpose of AWS IAM

\- Learn the key components of IAM

\- Create and manage IAM users

\- Assign permissions using IAM policies

\- Manage permissions through IAM groups

\- Understand the importance of the Principle of Least Privilege



\---



\## 📚 Topics Covered



\- What is AWS IAM?

\- Why IAM is important

\- IAM Users

\- IAM Groups

\- IAM Policies

\- IAM Roles

\- Authentication vs Authorization

\- Principle of Least Privilege



\---



\## 🛠️ Practical Demonstration



\### 1. Created an IAM User

\- Created a new IAM user.

\- Enabled console access.

\- Did not attach any permissions.



\### 2. Tested User Access

\- Logged in using the IAM user credentials.

\- Attempted to access Amazon S3.

\- Observed that the user could not view S3 buckets due to lack of permissions.



\### 3. Attached IAM Policy

\- Logged back into the root account.

\- Attached the \*AmazonS3FullAccess\* managed policy to the IAM user.



\### 4. Verified Access

\- Logged into the IAM user again.

\- Successfully accessed Amazon S3.

\- Verified that the user could now view S3 buckets.



\### 5. Created an IAM Group

\- Created a group named \*Development Group\*.

\- Attached the \*AmazonS3FullAccess\* policy to the group.

\- Added multiple IAM users to the group.

\- Verified that users inherited the group's permissions automatically.



\---



\## 📂 AWS Services Used



\- AWS Identity and Access Management (IAM)

\- Amazon S3



\---



\## 📖 Key Learnings



\- IAM provides secure access management for AWS resources.

\- IAM users should only receive permissions required for their tasks.

\- Policies define what actions are allowed or denied.

\- Groups simplify permission management by assigning permissions to multiple users at once.

\- Roles provide temporary permissions to AWS services or trusted entities.

\- Authentication verifies identity, while authorization determines what actions are permitted.



\---



\## 📸 Screenshots



Add screenshots for:

\- IAM User Creation

\- IAM User Login

\- S3 Access Denied

\- AmazonS3FullAccess Policy Attached

\- Successful S3 Access

\- IAM Group Creation

\- Users Added to Group



\---



\## 📁 Project Structure





Day-02-IAM/

│── README.md

└── screenshots/

&#x20;   ├── create-iam-user.png

&#x20;   ├── s3-access-denied.png

&#x20;   ├── attach-policy.png

&#x20;   ├── s3-access-success.png

&#x20;   ├── create-group.png



\---



\## ✅ Outcome



Successfully learned how AWS IAM manages authentication and authorization by creating IAM users, assigning permissions using policies, and managing multiple users efficiently through IAM groups

