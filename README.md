***AWS Cloud Project: Automated Web Service Remediation and High Availability Architecture***
- This project involved designing and deploying a secure, scalable, and highly available web application environment using AWS.
- Key components include network infrastructure, monitoring, and automated recovery actions to ensure resilience and minimize downtime.

**Project Overview:**

**Infrastructure Setup:**

- Built a Virtual Private Cloud (VPC) with two Availability Zones (AZs), each containing one public and one private subnet, ensuring high availability.
- Configured an Internet Gateway and NAT Gateway for secure and reliable access to the internet for public and private subnets.

**Hosting and Storage:**

- Deployed a web application on EC2 instances (t2.micro) using a well-architected, scalable design.
- Stored static content in Amazon S3, utilizing S3's durability and cost-effectiveness, decoupling storage from the EC2 instances.

**Monitoring and Alarms:**

- Integrated Amazon CloudWatch for real-time monitoring of EC2 health, performance metrics (e.g., CPU utilization), and web service availability.
- Configured CloudWatch alarms to trigger notifications when thresholds, such as CPU utilization or instance health checks, exceeded specified limits.

**Automatic Remediation:**

Implemented automatic remediation mechanisms for web service failures:

- EC2 Auto Recovery to restart failed instances when health checks failed.
- AWS Lambda function for custom actions, like restarting web services.
- AWS Systems Manager Automation to perform complex recovery actions, including service restarts and instance rebooting.
- Elastic Load Balancer (ELB) to monitor and route traffic to healthy instances, ensuring high availability.

**Security and Resilience:**

- Used security best practices such as security groups, IAM roles, and encryption for S3 data.
- Ensured the environment was disaster recovery-ready by leveraging multi-AZ deployment, automated backups, and scaling mechanisms.

**Scalability and Load Balancing:**

- Designed the architecture to automatically scale based on demand, using Auto Scaling groups to maintain application performance.
- Integrated Elastic Load Balancing (ELB) for distributing traffic across multiple instances and ensuring zero-downtime deployments.

**Technologies Used:**

- AWS Services: EC2, VPC, S3, CloudWatch, Lambda, Systems Manager, Auto Scaling, Elastic Load Balancer.
- Infrastructure as Code: AWS CloudFormation to automate the creation of network and compute resources.
- Monitoring & Notifications: CloudWatch for metrics, SNS for alerts.
- Remediation: Lambda, EC2 Auto Recovery, Systems Manager Automation.

**Outcome:** 

The project demonstrates an automated, resilient cloud infrastructure capable of detecting failures and self-healing without manual intervention.
It showcases strong knowledge of AWS services, cloud architecture, and DevOps practices, ensuring scalability, security, and disaster recovery readiness.

![AWS_Project drawio (2)](https://github.com/user-attachments/assets/f02eef88-1ae2-4dec-957c-cdf21d377330)

