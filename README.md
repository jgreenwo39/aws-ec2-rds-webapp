# EC2 Web App + RDS Database

A 3-tier web application deployed on AWS using EC2 for compute and RDS for managed database services.

## Live Demo

http://3.151.20.180/index.php

## Architecture

User → EC2 (Nginx + PHP) → RDS (MySQL)

## AWS Services Used

- **Amazon EC2** — t2.micro Ubuntu server running Nginx and PHP
- **Amazon RDS** — Managed MySQL 8.0 database (db.t3.micro)
- **VPC & Security Groups** — Network isolation and access control
- **IAM** — Permissions and access management

## Features

- Linux web server (Nginx) on EC2
- PHP application connecting to MySQL database
- Managed database on Amazon RDS
- Security groups controlling traffic between EC2 and RDS
- Live data displayed from RDS database

## Project Structure

- index.php — PHP web application with RDS connection
- README.md — Project documentation

## Deployment Steps

1. Launched Ubuntu EC2 instance (t2.micro) with SSH access
2. Installed and configured Nginx web server
3. Installed PHP and php-mysql for database connectivity
4. Created RDS MySQL database (db.t3.micro)
5. Connected EC2 to RDS via VPC security groups
6. Created database schema and inserted sample data
7. Built PHP application that queries and displays live RDS data

## Technical Details

- **OS:** Ubuntu Server 24.04 LTS
- **Web Server:** Nginx
- **Language:** PHP 8.3
- **Database:** MySQL 8.4 on Amazon RDS
- **Region:** us-east-2 (Ohio)

## Author

**Joe Greenwood**
AWS Cloud Practitioner
[GitHub](https://github.com/jgreenwo39)