# AWS 3-Tier VPC Application with RDS

## 📌 Project Overview

This project demonstrates the deployment of a 3-tier application environment on AWS using Amazon VPC, EC2, Amazon RDS MariaDB, Nginx, Apache Tomcat, Internet Gateway and NAT Gateway.

A custom VPC was created with public and private subnets to separate the application and database components.

## 🏗️ Architecture

Internet
   ↓
Internet Gateway
   ↓
Public Subnet
   ↓
Application Server
   ↓
Private Subnet
   ↓
Amazon RDS MariaDB

Private Resources
   ↓
NAT Gateway
   ↓
Internet Gateway
   ↓
Internet

## 🛠️ AWS Services & Technologies Used

- Amazon VPC
- Amazon EC2
- Amazon RDS MariaDB
- Internet Gateway
- NAT Gateway
- Route Tables
- Security Groups
- Nginx
- Apache Tomcat
- Linux
- MySQL/MariaDB

## 🌐 VPC Configuration

- VPC Name: `my-vpc`
- CIDR: `10.0.0.0/16`
- Public and private subnets
- Public route table
- Private/NAT route table
- Internet Gateway: `my-igw`
- NAT Gateway: `my-nat`

## 🖥️ EC2 Infrastructure

The project uses EC2 instances for application deployment and administration.

### Servers

- Application Server
- Database Server
- Jump Server

The Jump Server was used for administration of private resources.

## 🌐 Web Application

A Student Registration application was deployed using Apache Tomcat and Nginx.

The application provides:

- Student Registration Form
- Students List
- Edit student records
- Delete student records

## 🗄️ Database

Amazon RDS MariaDB was configured as the database layer.

Database connectivity was configured through private networking and security groups using port `3306`.

## 🔐 Security

Security Groups were configured to control access between the different components.

The project used:

- SSH — Port 22
- HTTP — Port 80
- Tomcat — Port 8080
- MySQL/MariaDB — Port 3306

## 🔄 Application Flow

1. User accesses the web application.
2. Traffic reaches the application/web layer.
3. Nginx and Apache Tomcat handle the application.
4. Application communicates with the database layer.
5. Student information is stored in MariaDB.
6. Private resources use the NAT Gateway for outbound internet connectivity.

## 📷 Project Screenshots

Screenshots demonstrating the VPC, subnets, route tables, Internet Gateway, NAT Gateway, EC2 instances, security groups, Tomcat, Nginx and RDS configuration are included in this repository.

## 📚 Documentation

Detailed implementation steps and configuration screenshots are available in the project documentation.

---

## 👨‍💻 Author

**Saurabh Chavan**

AWS & DevOps Enthusiast
