# Lab 6 – Scale and Load Balance Your Architecture

## Author

* **Name**: NARENDHIRAN P
* **Register Number**: 212224230177
* **Date of Submission**: 05/09/2026

---

## Objective

The objective of this lab is to understand how to design a scalable and highly available architecture on AWS using Auto Scaling and Elastic Load Balancing. This experiment focuses on distributing incoming traffic across multiple EC2 instances, automatically scaling resources based on demand, and validating fault tolerance.

---

## Prerequisites

* Basic knowledge of Amazon EC2 and VPC
* Completion of previous labs (IAM, EC2, EBS, Database Server)
* AWS Academy Lab access
* Stable internet connection

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Elastic Load Balancer (ELB / ALB)
* Auto Scaling Groups (ASG)
* Amazon CloudWatch

---

## Tasks Performed

### Task 1: Review Existing Architecture

Students review the existing EC2-based application architecture created in previous experiments.

### Task 2: Create a Launch Template

Students create a launch template that defines the EC2 instance configuration including AMI, instance type, security group, and user data.

### Task 3: Create an Auto Scaling Group

Students create an Auto Scaling Group using the launch template and configure minimum, maximum, and desired instance capacity.

### Task 4: Configure an Application Load Balancer

Students create an Application Load Balancer and configure target groups for routing traffic to EC2 instances.

### Task 5: Register Auto Scaling Group with Load Balancer

Students attach the Auto Scaling Group to the target group of the load balancer.

### Task 6: Configure Scaling Policies

Students configure scaling policies based on CPU utilization using Amazon CloudWatch alarms.

### Task 7: Test Load Balancing and Scaling

Students test the setup by generating traffic and observing automatic scaling and load distribution.

---

## Workflow (To be filled by Student)

1.The workflow begins by reviewing the existing EC2-based application architecture in the AWS Management Console, allowing students to understand how instances, networking, and prior configurations are structured before implementing scaling and load balancing.

2.Next, a launch template is created to define the EC2 configuration, including the AMI, instance type, security group, and user data scripts, which standardizes instance deployment for automated scaling.

3.An Auto Scaling Group is then set up using the launch template, where minimum, maximum, and desired capacities are defined to ensure that the application can automatically adjust the number of running instances based on demand.

4.Following this, an Application Load Balancer is configured to distribute incoming traffic across multiple EC2 instances, along with target groups that manage routing and health checks of instances.

5.The Auto Scaling Group is then attached to the load balancer’s target group so that newly launched or terminated instances are automatically registered or deregistered, ensuring continuous availability.

6.Scaling policies are configured using Amazon CloudWatch, where CPU utilization thresholds trigger automatic scaling actions such as adding or removing instances.

7.Finally, the system is tested by generating traffic to observe how the load balancer distributes requests and how the Auto Scaling Group dynamically adjusts the number of instances in response to workload changes.

---

## Output Screenshots 

<img width="1919" height="1021" alt="Screenshot 2026-03-12 154410" src="https://github.com/user-attachments/assets/9213b030-16d6-4290-8f80-4aa84f48072f" />

<img width="1919" height="1017" alt="Screenshot 2026-03-12 154600" src="https://github.com/user-attachments/assets/af6ff0a9-94f5-429b-bb1f-7ccb88f4bd4e" />

<img width="1917" height="1019" alt="Screenshot 2026-03-12 154837" src="https://github.com/user-attachments/assets/f94a0fab-aea4-42f4-86a7-3391255c0709" />

<img width="1907" height="1019" alt="Screenshot 2026-03-12 161321" src="https://github.com/user-attachments/assets/fb243a39-6f8d-45b7-ba3e-8d6e7c54255d" />

## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.
