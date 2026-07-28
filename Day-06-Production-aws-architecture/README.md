\# Day 06 - AWS Production Architecture (Theory)



\## 📌 Overview



On Day 06, I learned how a production-ready application is deployed on AWS using networking and high-availability services. The focus was on understanding the complete architecture before implementing it practically.



\---



\## 🛠️ AWS Services Covered



\- Amazon VPC

\- Public Subnets

\- Private Subnets

\- Internet Gateway

\- NAT Gateway

\- Security Groups

\- Application Load Balancer (ALB)

\- Target Group

\- Launch Template

\- Auto Scaling Group

\- Bastion Host (Jump Server)

\- EC2



\---



\## 🏗️ Production Architecture





&#x20;                   Internet

&#x20;                       │

&#x20;               Internet Gateway

&#x20;                       │

&#x20;         Application Load Balancer

&#x20;                /                \\

&#x20;       Public Subnet AZ1     Public Subnet AZ2

&#x20;         (NAT Gateway)        (NAT Gateway)

&#x20;               │                   │

&#x20;       Private Subnet AZ1   Private Subnet AZ2

&#x20;           EC2 Instance         EC2 Instance

&#x20;                   ↑

&#x20;            Bastion Host (SSH)





\---



\## 📚 Concepts Learned



\- Created a VPC spanning two Availability Zones.

\- Used public subnets for NAT Gateways and Load Balancer.

\- Deployed application servers inside private subnets.

\- Understood how the Internet Gateway provides internet connectivity.

\- Learned that private instances access the internet through a NAT Gateway.

\- Understood the role of an Application Load Balancer in distributing incoming traffic.

\- Learned how Auto Scaling automatically launches or terminates EC2 instances based on demand.

\- Understood how a Bastion Host provides secure SSH access to private EC2 instances.



\---



\## 🔄 Request Flow





User

&#x20; │

&#x20; ▼

Application Load Balancer

&#x20; │

&#x20; ▼

Private EC2 Instances

&#x20; │

&#x20; ▼

Internet Access via NAT Gateway





\---



\## 🎯 Key Takeaways



\- Keep application servers in private subnets for better security.

\- Use a Load Balancer to distribute incoming traffic.

\- Use Auto Scaling to improve availability and handle traffic spikes.

\- Use NAT Gateway for outbound internet access from private instances.

\- Use a Bastion Host to securely access private EC2 instances.



\---



\## 📖 Summary



This session focused on understanding how production environments are designed in AWS. Instead of deploying everything on a single EC2 instance, production applications use multiple Availability Zones, private networking, load balancing, and auto scaling to achieve high availability, scalability, and security.



\---



\*Status:\* ✅ Theory Completed | Practical Implementation on Day 07

