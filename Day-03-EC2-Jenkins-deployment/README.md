\# Day 03 - Amazon EC2 \& Jenkins Deployment



\## 📌 Overview



On Day 3 of the AWS Zero to Hero series, I learned about \*Amazon Elastic Compute Cloud (EC2)\* and deployed \*Jenkins\* on an Ubuntu EC2 instance. I also learned how to securely connect to an EC2 instance using SSH and expose Jenkins to the internet using Security Groups.



\---



\## 🎯 Objectives



\- Understand Amazon EC2

\- Learn EC2 instance types

\- Understand AWS Regions and Availability Zones

\- Launch an EC2 instance

\- Connect to an EC2 instance using SSH

\- Install Java

\- Install Jenkins

\- Configure Security Groups

\- Access Jenkins through a web browser



\---



\## 📚 Topics Covered



\- What is Amazon EC2?

\- Benefits of EC2

\- Multi-tenancy in AWS

\- EC2 Instance Types

\- AWS Regions

\- Availability Zones

\- Key Pairs

\- Public IPv4 Address

\- Security Groups

\- SSH Connection

\- Jenkins Deployment



\---



\## ☁️ What is Amazon EC2?



Amazon Elastic Compute Cloud (EC2) provides scalable virtual servers in the AWS Cloud.



It allows users to:



\- Launch virtual machines on demand

\- Scale resources as required

\- Avoid purchasing physical hardware

\- Pay only for the resources used



AWS uses virtualization, allowing multiple customers to share the same physical infrastructure while keeping each virtual machine isolated and secure.



\---



\## 🖥️ EC2 Instance Types



The following EC2 instance categories were discussed:



\- General Purpose

\- Compute Optimized

\- Memory Optimized

\- Storage Optimized

\- Accelerated Computing



Each type is designed for different workloads depending on CPU, memory, storage, or GPU requirements.



\---



\## 🌍 AWS Regions \& Availability Zones



\- A Region is a geographical location where AWS has data centers.

\- Each Region contains multiple Availability Zones (AZs).

\- Availability Zones are physically separated data centers that provide high availability and fault tolerance.



\---



\## 🛠️ Practical Demonstration



\### 1. Launch EC2 Instance



\- Opened EC2 Dashboard

\- Clicked \*Launch Instance\*

\- Selected Ubuntu AMI

\- Chose \*t3.micro\* instance type

\- Created a new Key Pair

\- Launched the instance successfully



\---



\### 2. Connect to EC2



Connected to the instance using SSH.



Verified the logged-in user and switched to the root user.



Updated package information before installing software.



\---



\### 3. Install Java



Installed OpenJDK, which is required to run Jenkins.



Verified the installation using:



bash

java --version





\---



\### 4. Install Jenkins



Installed Jenkins on the EC2 instance.



Verified the Jenkins service status after installation.



\---



\### 5. Configure Security Group



Edited the EC2 Security Group.



Added an inbound rule:



\- Port: \*8080\*

\- Source: \*Anywhere (0.0.0.0/0)\*



Saved the rule to allow external access to Jenkins.



\---



\### 6. Access Jenkins



Copied the Public IPv4 address of the EC2 instance.



Opened the following URL in a web browser:





http://<Public-IP>:8080





Successfully accessed the Jenkins setup page.



\---



\## ☁️ AWS Services Used



\- Amazon EC2

\- Security Groups

\- Key Pairs



\---



\## 💻 Software Installed



\- Ubuntu

\- OpenJDK

\- Jenkins



\---



\## ✅ Outcome



Successfully launched an Ubuntu EC2 instance, connected to it using SSH, installed Java and Jenkins, configured the required Security Group rules, and accessed Jenkins from a web browser using the instance's public IP address.

