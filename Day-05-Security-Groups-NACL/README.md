\# Day 05 - Security Groups \& Network ACL (NACL)



\## 📌 Overview



Today I learned how AWS controls network traffic using Security Groups and Network Access Control Lists (NACLs). I also performed a practical demonstration by allowing and blocking traffic to understand how requests are handled.



\---



\## 🎯 Objectives



\- Understand Security Groups

\- Understand Network ACL

\- Learn inbound and outbound traffic

\- Compare Security Groups and NACL

\- Test traffic using Python HTTP Server



\---



\## 📚 Topics Covered



\- Security Groups

\- Network ACL

\- Inbound Rules

\- Outbound Rules

\- Stateful vs Stateless

\- Traffic Filtering

\- VPC Networking



\---



\## 🔐 Security Groups



Security Groups work at the EC2 instance level.



They control which traffic is allowed to enter or leave an EC2 instance.



Security Groups:



\- Allow traffic only

\- Are Stateful

\- Apply to individual EC2 instances



\---



\## 🌐 Network ACL (NACL)



Network ACL operates at the subnet level.



It controls traffic entering or leaving an entire subnet.



NACL:



\- Allow or Deny traffic

\- Stateless

\- Applies to all instances inside the subnet



\---



\## 🔄 Inbound vs Outbound



\### Inbound Traffic



Traffic coming from users into the application.



Example:



User → EC2



\---



\### Outbound Traffic



Traffic leaving the EC2 instance.



Example:



EC2 → Internet



\---



\## ⚖️ Security Group vs NACL



| Security Group | Network ACL |

|---------------|-------------|

| Instance Level | Subnet Level |

| Stateful | Stateless |

| Allow Only | Allow and Deny |

| Applied to EC2 | Applied to Subnet |



\---



\## 🛠️ Practical Demonstration



\### Step 1



Created a custom VPC.



\---



\### Step 2



Launched an EC2 instance inside the VPC.



\---



\### Step 3



Connected using SSH.



\---



\### Step 4



Started a Python HTTP Server on Port 8000.



\---



\### Step 5



Allowed Port 8000 in the Security Group.



Verified the application was accessible.



\---



\### Step 6



Modified the Network ACL.



Created a rule to deny traffic on Port 8000.



\---



\### Step 7



Verified the application became inaccessible because the request was blocked at the subnet level.



\---



\## 📌 Key Learning



Even if the Security Group allows traffic, the request can still be blocked if the Network ACL denies it.





\## ✅ Outcome



Successfully understood the difference between Security Groups and Network ACLs by allowing and denying traffic and observing how requests behaved in real time.

