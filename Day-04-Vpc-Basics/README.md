\# Day 04 - Amazon VPC (Virtual Private Cloud)



\## 📌 Overview



Today I learned the fundamentals of Amazon Virtual Private Cloud (VPC), how AWS networking works, and how internet traffic reaches applications running inside a VPC.



\---



\## 🎯 Objectives



\- Understand Amazon VPC

\- Learn VPC components

\- Understand public and private subnets

\- Learn Internet Gateway

\- Understand Route Tables

\- Learn NAT Gateway

\- Understand request flow inside a VPC



\---



\## 📚 Topics Covered



\- What is Amazon VPC?

\- CIDR Block

\- Public Subnet

\- Private Subnet

\- Internet Gateway

\- Route Table

\- Elastic Load Balancer

\- NAT Gateway

\- Security Groups

\- Network Architecture



\---



\## ☁️ What is Amazon VPC?



Amazon Virtual Private Cloud (VPC) is an isolated virtual network inside AWS where cloud resources such as EC2 instances are deployed securely.



A VPC allows users to define:



\- IP address range

\- Subnets

\- Route tables

\- Internet connectivity

\- Security controls



\---



\## 🏗️ Critical Components



\- Internet Gateway

\- Public Subnet

\- Private Subnet

\- Route Table

\- Security Groups

\- NAT Gateway

\- Elastic Load Balancer



\---



\## 🌐 Request Flow



A request from a user reaches the application through the following path:



Internet



↓



Internet Gateway



↓



Public Subnet



↓



Elastic Load Balancer



↓



Route Table



↓



Security Group



↓



Application (EC2)



\---



\## 🔒 NAT Gateway



Private EC2 instances should not be directly exposed to the internet.



A NAT Gateway allows private instances to:



\- Download software updates

\- Access AWS services

\- Access the internet securely



while keeping their private IP addresses hidden.



\---



\## 📌 Public vs Private Subnet



\### Public Subnet



\- Has internet access

\- Uses Internet Gateway

\- Hosts public-facing resources



\### Private Subnet



\- No direct internet access

\- Uses NAT Gateway

\- Hosts databases and backend services



\## ✅ Outcome



Learned how Amazon VPC provides secure networking for AWS resources and understood how internet traffic flows from users to applications.

