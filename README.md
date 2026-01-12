# Application-load-balancer

Application Load Balancer with EC2 (AWS)

📌 Project Overview

This project demonstrates how to create and configure an AWS Application Load Balancer (ALB) to distribute incoming HTTP traffic across multiple EC2 instances. The setup ensures high availability, scalability, and fault tolerance for a web application.

--------------------------------------------------------------------------

🛠️ Services Used

Amazon EC2 – Virtual servers to host the web application

Application Load Balancer (ALB) – Distributes traffic across EC2 instances

Target Groups – Routes traffic and performs health checks

Amazon VPC – Networking and security

Security Groups – Control inbound and outbound traffic

-------------------------------------------------------------------------

🧱 Architecture

Two EC2 instances deployed in the same VPC

Apache web server installed on each EC2 instance

One Application Load Balancer (Internet-facing)

ALB listener on HTTP port 80

Target group with EC2 instances registered

Health checks enabled to monitor instance health

--------------------------------------------------------------

⚙️ Project Setup Steps

1. Launch EC2 Instances

Amazon Linux 2 AMI

Instance type: t2.micro

Install Apache web server

Host a simple HTML page on each instance

2. Configure Security Groups

Allow HTTP (80) from anywhere

Allow SSH (22) from your IP

3. Create Target Group

Target type: Instance

Protocol: HTTP

Port: 80

Register both EC2 instances

Health check path: /

4. Create Application Load Balancer

Type: Application Load Balancer

Scheme: Internet-facing

Listener: HTTP on port 80

Attach target group to the listener

5. Verify Load Balancing

Access the ALB DNS name in a browser

Refresh the page to see traffic distributed between instances

-------------------------------------------------------------------

✅ Output / Result

Load Balancer status: Active

Target group status: Healthy

Traffic successfully distributed between EC2 instances

High availability achieved using ALB

----------------------------------------------------------------


📈 Benefits of Using ALB

Automatic traffic distribution

Improved availability and reliability

Health monitoring of backend servers

Easy scalability

-------------------------------------------------------------------

🎯 Use Case

This architecture is ideal for:

Web applications

Microservices

High-availability systems

Production-ready cloud deployments

------------------------------------------------


📚 Learning Outcome

Hands-on experience with AWS Load Balancing

Understanding listeners, target groups, and health checks

Real-world cloud architecture implementation

----------------------------------------------------------

👤 Author

Dharani Boominathan
AWS Learner | Cloud Enthusiast


Create architecture diagram description

Just tell me 👍
