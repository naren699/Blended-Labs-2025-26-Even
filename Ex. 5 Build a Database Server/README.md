# Lab 5 – Build a Database Server (AWS)

## Author

* **Name**: NARENDHIRAN P
* **Register Number**: 212224230177
* **Date of Submission**: 01/09/2026

---

## Objective

The objective of this experiment is to understand how to deploy and configure a database server in AWS. This lab focuses on launching an EC2 instance, installing a database management system (DBMS), configuring basic database settings, creating a sample database, and validating connectivity to the database server.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing VPC and EC2 knowledge (from previous labs)
* Basic knowledge of Linux commands and SQL

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Security Groups
* SSH Client (Terminal / PuTTY)
* MySQL / MariaDB / PostgreSQL (any one)

---

## Tasks Performed

### Task 1: Launch EC2 Instance for Database Server

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type and configure key pair and security group.

---

### Task 2: Configure Security Group for Database Access

Modify the security group to allow:

* SSH (Port 22) for remote access
* Database port (e.g., MySQL – 3306 or PostgreSQL – 5432)

---

### Task 3: Connect to EC2 Instance

Connect to the EC2 instance using SSH from your local machine.

---

### Task 4: Install Database Server

Install a database server software such as MySQL, MariaDB, or PostgreSQL on the EC2 instance using package manager commands.

---

### Task 5: Start and Configure Database Service

Start the database service and configure basic settings such as root password and user privileges.

---

### Task 6: Create a Sample Database

Create a sample database and a table inside it. Insert a few records into the table.

---

### Task 7: Test Database Connectivity

Test the database server by connecting to it locally or remotely and performing basic SQL queries.

---

## Workflow (Student Explanation)


1. Logged in to the AWS Management Console and launched an Amazon EC2 instance using Amazon Linux 2 AMI.
2. Configured the security group to allow SSH access (Port 22) and MySQL database access (Port 3306).
3. Connected to the EC2 instance using SSH and updated the system packages.
4. Installed the MySQL database server, started the service, and configured the database environment.
5. Created a sample database and table, inserted records, and verified the data using SQL queries.

---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Instance for Database Server
<img width="1716" height="718" alt="image" src="https://github.com/user-attachments/assets/67b7f5de-b4f9-482f-96c7-892c230f4e9b" />


---

### Screenshot 2: Database Service Running

<img width="1909" height="962" alt="Screenshot 2026-05-30 111615" src="https://github.com/user-attachments/assets/ec660c4e-4263-48f9-a849-35aad3b9326c" />

---

### Screenshot 3: Sample Database and Table

<img width="1919" height="970" alt="Screenshot 2026-05-30 111724" src="https://github.com/user-attachments/assets/446a71b9-e05c-4816-ab43-ebaacdb64feb" />


---

## Result

The database server was successfully deployed on an AWS EC2 instance. The MySQL service was installed and configured correctly. A sample database and table were created, records were inserted, and database connectivity was verified through SQL queries. This experiment provided practical experience in deploying and managing a cloud-based database server using AWS services.
