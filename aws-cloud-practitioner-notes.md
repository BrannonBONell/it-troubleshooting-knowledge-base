# AWS Cloud Practitioner Notes

# What is AWS?

AWS (Amazon Web Services) is a cloud computing platform that provides:
- servers
- storage
- databases
- networking
- security
- AI services
- monitoring
- virtualization

AWS allows companies to rent infrastructure instead of owning physical hardware.

---

# Benefits of Cloud Computing

# On-Demand Resources
Resources can be created and removed quickly.

---

# Scalability
Infrastructure can scale up or down depending on demand.

---

# Pay-As-You-Go Pricing
Customers only pay for resources they use.

---

# Global Infrastructure
AWS has data centers around the world.

---

# High Availability
Cloud systems can be designed for redundancy and fault tolerance.

---

# Shared Responsibility Model

# AWS Responsibilities
AWS manages:
- physical hardware
- networking infrastructure
- data center security
- power/cooling

---

# Customer Responsibilities
Customers manage:
- accounts
- data
- operating systems
- permissions
- applications

---

# Core AWS Services

# EC2 (Elastic Compute Cloud)

Virtual machines hosted in AWS.

Common uses:
- websites
- applications
- game servers
- Linux servers

Key concepts:
- instance types
- AMIs
- security groups
- EBS storage

---

# S3 (Simple Storage Service)

Object storage service.

Common uses:
- backups
- file storage
- static websites
- media hosting

Key concepts:
- buckets
- object storage
- permissions
- lifecycle policies

---

# IAM (Identity and Access Management)

Controls permissions and account access.

Best practices:
- least privilege
- MFA enabled
- avoid root account usage

---

# VPC (Virtual Private Cloud)

Private networking environment in AWS.

Key concepts:
- subnets
- route tables
- internet gateway
- security groups
- NACLs

---

# RDS (Relational Database Service)

Managed database service.

Supported engines:
- MySQL
- PostgreSQL
- MariaDB
- SQL Server

Benefits:
- automated backups
- scaling
- patching

---

# Lambda

Serverless compute service.

Runs code without managing servers.

Common uses:
- automation
- event-driven tasks
- API backends

---

# CloudWatch

Monitoring and logging platform.

Used for:
- metrics
- alarms
- logging
- monitoring resource health

---

# AWS Regions and Availability Zones

# Region
A physical geographic location.

Example:
- us-east-1
- us-west-2

---

# Availability Zone
Separate isolated data centers within a region.

Used for:
- redundancy
- fault tolerance
- high availability

---

# Security Concepts

# Security Groups
Virtual firewalls attached to instances.

Control:
- inbound traffic
- outbound traffic

---

# Multi-Factor Authentication (MFA)
Adds additional account security.

Strongly recommended for all AWS accounts.

---

# Principle of Least Privilege
Users should only have the permissions necessary to perform their tasks.

---

# Basic Networking Concepts

# Public Subnet
Resources accessible from the internet.

---

# Private Subnet
Resources isolated from direct internet access.

---

# Elastic IP
Static public IP address in AWS.

---

# Load Balancer
Distributes traffic across multiple servers.

Improves:
- availability
- scalability

---

# Cloud Pricing Concepts

# OpEx vs CapEx

# CapEx
Traditional hardware purchases.

# OpEx
Cloud subscription/pay-as-you-go model.

---

# Reserved Instances
Lower pricing for long-term commitments.

---

# On-Demand Pricing
Pay only for active usage.

---

# AWS Support Plans

Examples:
- Basic
- Developer
- Business
- Enterprise

Higher tiers provide:
- faster response times
- technical support
- architecture guidance

---

# Common AWS Troubleshooting Scenarios

# Scenario 1
Cannot connect to EC2 instance.

Possible causes:
- security group issue
- wrong IP
- SSH/RDP disabled
- instance stopped

Check:
- instance status
- inbound rules
- public IP assignment

---

# Scenario 2
Website hosted in S3 unavailable.

Possible causes:
- bucket permissions
- static hosting disabled
- DNS issue

---

# Scenario 3
Unexpected AWS charges.

Possible causes:
- forgotten resources
- running EC2 instances
- snapshots
- data transfer costs

Best practice:
- review billing dashboard regularly

---

# Important AWS Concepts for Beginners

- cloud scalability
- high availability
- virtualization
- object storage
- identity management
- serverless computing
- monitoring
- shared responsibility model

---

# Beginner AWS Skills Valuable for IT Careers

- launching EC2 instances
- configuring security groups
- basic Linux administration
- troubleshooting connectivity
- managing S3 buckets
- monitoring CloudWatch alerts

These skills are relevant for:
- cloud support
- help desk
- junior cloud engineer
- DevOps
- AI infrastructure
- technical support roles

---

# AWS Learning Goals

# Beginner Goals
- understand cloud fundamentals
- launch EC2 instance
- create S3 bucket
- configure IAM user
- understand VPC basics

# Intermediate Goals
- Docker
- automation
- CI/CD
- Infrastructure as Code
- monitoring and logging
- serverless applications
