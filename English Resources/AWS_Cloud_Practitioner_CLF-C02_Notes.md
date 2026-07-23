# AWS Certified Cloud Practitioner (CLF-C02) - Course Notes

> **Course:** AWS Certified Cloud Practitioner Certification Course (CLF-C02) - Pass the Exam!
> **Instructor:** Andrew Brown (ExamPro)
> **Channel:** freeCodeCamp.org
> **Link:** https://www.youtube.com/watch?v=NhDYbskXRgc

---

## Table of Contents

1. [[#1. Introduction & Exam Guide|Introduction & Exam Guide]] 
2. [[#2. Cloud Concepts|Cloud Concepts]] 
3. [[#3. Getting Started|Getting Started]] 
4. [[#4. Digital Transformation|Digital Transformation]] 
5. [[#5. The Benefits Of Cloud|The Benefits Of Cloud]] 
6. [[#6. Global Infrastructure|Global Infrastructure]] 
7. [[#7. Cloud Architecture|Cloud Architecture]] 
8. [[#8. Management And Developer Tools|Management And Developer Tools]] 
9. [[#9. Shared Responsibility Model|Shared Responsibility Model]] 
10. [[#10. Compute|Compute]] 
11. [[#11. Storage Services|Storage Services]] 
12. [[#12. Databases|Databases]] 
13. [[#13. Networking|Networking]] 
14. [[#14. EC2|EC2]] 
15. [[#15. EC2 Pricing Models|EC2 Pricing Models]] 
16. [[#16. Identity|Identity]] 
17. [[#17. Application Integration|Application Integration]] 
18. [[#18. Containers|Containers]] 
19. [[#19. Governance|Governance]] 
20. [[#20. Provisioning|Provisioning]] 
21. [[#21. Serverless|Serverless]] 
22. [[#22. Windows On AWS|Windows On AWS]] 
23. [[#23. Logging|Logging]] 
24. [[#24. ML, AI & Big Data|ML, AI & Big Data]] 
25. [[#25. AWS Well-Architected Framework|AWS Well-Architected Framework]] 
26. [[#26. TCO And Migration|TCO And Migration]] 
27. [[#27. Billing And Pricing|Billing And Pricing]]

---

## 1. Introduction & Exam Guide

### About the CLF-C02 Exam
- **Name:** AWS Certified Cloud Practitioner (CLF-C02)
- **Duration:** 90 minutes
- **Format:** 65 questions (multiple choice and multiple response)
- **Passing score:** 700/1000
- **Cost:** ~$100 USD
- **Available languages:** English, Japanese, Korean, Chinese, and others
- **Validity:** 3 years

### Who is this exam for?
- People with no prior technical experience on AWS
- Ideal as a **first certification** on the AWS path
- Great for non-technical roles (sales, managers, finance) who need to understand the cloud
- Foundation for more advanced certifications (Solutions Architect, Developer, SysOps)

### AWS Certification Roadmap
- **Foundational:** Cloud Practitioner (CLF-C02)
- **Associate:** Solutions Architect, Developer, SysOps Administrator
- **Professional:** Solutions Architect Professional, DevOps Engineer Professional
- **Specialty:** Security, Machine Learning, Advanced Networking, Database, Data Analytics, SAP

### Exam Content Outline (Domains)
| Domain | Weight |
|--------|--------|
| 1. Cloud Concepts | 24% |
| 2. Security and Compliance | 30% |
| 3. Cloud Technology and Services | 34% |
| 4. Billing, Pricing and Support | 12% |

---

## 2. Cloud Concepts

### What is Cloud Computing?
- The **on-demand** delivery of IT resources over the internet with a **pay-as-you-go** pricing model
- Instead of buying and maintaining physical servers, you access technology services (compute, storage, databases) as you need them

### Evolution of Cloud Hosting
1. **Dedicated Server:** A single physical server for one business. Very expensive, high maintenance
2. **Virtual Private Server (VPS):** A single physical server split into multiple virtual machines. Better resource usage
3. **Shared Hosting:** A single server shared among many users. Cheap but limited
4. **Cloud Hosting:** Multiple servers acting as one system. Flexible, scalable, pay-as-you-go

### What is Amazon?
- Company founded in 1994 by Jeff Bezos as an online bookstore
- Grew to become the world's largest retailer
- Amazon Web Services (AWS) was born from Amazon's internal infrastructure

### What is AWS?
- **Amazon Web Services** is the world's largest cloud service provider (CSP)
- Officially launched in **2006** with S3 and EC2
- Offers **200+** services
- Generates billions of dollars in annual revenue
- Used by companies like Netflix, Twitch, LinkedIn, Facebook

### What is a CSP (Cloud Service Provider)?
- A company that offers multiple cloud services
- Services accessible via a Single Unified API (e.g., AWS API)
- Metered billing based on usage
- Built-in monitoring
- Infrastructure as a Service (IaaS) with automation
- Top CSPs: **AWS, Azure, GCP**

### Landscape of CSPs
- **Tier 1 (Top):** AWS, Azure, GCP — Wide range of services, market leaders
- **Tier 2:** Alibaba Cloud, IBM Cloud, Oracle Cloud, Huawei Cloud
- **Tier 3:** Rackspace, DigitalOcean, Linode, Vultr

### Gartner Magic Quadrant for Cloud
- AWS has been a consistent leader in Gartner's Magic Quadrant for IaaS
- AWS and Azure are the leaders, with GCP as a "visionary" catching up

### Common Cloud Services
The 4 most common services from any CSP:
1. **Compute** — Virtual servers (EC2)
2. **Storage** — File storage (S3)
3. **Networking** — Virtual networks (VPC)
4. **Databases** — Managed databases (RDS)

### AWS Technology Overview
- AWS has **200+** services grouped into categories:
  - Compute, Storage, Database, Networking, Machine Learning, Analytics, Security, IoT, etc.

### Evolution of Computing
1. **Dedicated:** Full physical server for you
2. **VMs (Virtual Machines):** Multiple VMs on a physical server via hypervisor
3. **Containers:** Multiple isolated apps on a VM, sharing the OS
4. **Functions (Serverless):** Run code without managing servers (AWS Lambda)

### Types of Cloud Computing
| Type | Description | AWS Example |
|------|-------------|-------------|
| **IaaS** (Infrastructure as a Service) | You get the basic infrastructure, you manage the rest | EC2, VPC |
| **PaaS** (Platform as a Service) | You get the platform, you just upload your code | Elastic Beanstalk, Heroku |
| **SaaS** (Software as a Service) | Ready-to-use software | Gmail, Salesforce, Office 365 |

### Cloud Deployment Models
| Model | Description |
|-------|-------------|
| **Public Cloud** | Everything on the CSP's cloud. E.g., AWS, Azure |
| **Private Cloud** | Your own cloud in your datacenter (on-premise). E.g., OpenStack, VMware |
| **Hybrid Cloud** | Combination of Public + Private Cloud |
| **Cross-Cloud / Multi-Cloud** | Using multiple CSPs (AWS + Azure + GCP) |

---

## 3. Getting Started

### Creating an AWS Account
- You need: email, credit/debit card, phone number
- AWS offers a **Free Tier** for new users for 12 months
- A root account is created with full access — **NEVER use the root account for daily tasks**

### Overbilling Story
- It's common for new users to leave resources running and receive unexpected bills
- **Always** set up billing alerts and budgets when creating your account

### AWS Budgets
- Service to create **budgets** and receive alerts when you approach or exceed the limit
- You can create budgets by cost, usage, or reservations
- Set alerts via email when you reach 50%, 80%, 100% of your budget
- **This is the first thing you should configure when creating your account**

### AWS Free Tier
Three types of free offers:
1. **Always Free:** Services that are always free (e.g., Lambda 1M requests/month, DynamoDB 25GB)
2. **12 Months Free:** Free for 12 months from account creation (e.g., EC2 t2.micro 750hrs/month, S3 5GB)
3. **Trials:** Short-duration free trials for specific services

### Turning on MFA (Multi-Factor Authentication)
- **Critical** for your account security
- Enable MFA on the root account immediately
- Options: Authenticator app (Google Authenticator, Authy), Security key (YubiKey), Hardware MFA
- Go to IAM > Security credentials > MFA > Assign MFA device

---

## 4. Digital Transformation

### Innovation Waves
- Kondratiev waves show cycles of technological innovation every ~50 years
- We are in the wave of **Digital Transformation** driven by cloud, AI, IoT, Big Data

### Burning Platform
- Concept: when a company **must** change because the status quo is more dangerous than the change
- Example: Nokia didn't adopt smartphones and disappeared from the market
- The cloud is the answer to many corporate "burning platforms"

### Digital Transformation Checklist
- Migrate from on-premise to the cloud
- Modernize legacy applications
- Adopt DevOps and CI/CD
- Use data to drive decisions (Data-Driven)
- Implement Machine Learning and AI

### Evolution of Computing Power
- From mainframes to PCs, to servers, to VMs, to containers, to serverless
- **AWS Graviton** — ARM processors designed by AWS, more efficient and cost-effective
- **AWS Inferentia** — Chips optimized for Machine Learning inference

### Amazon Braket
- AWS **quantum computing** service
- Allows you to experiment with quantum simulators and real quantum hardware
- Supports multiple technologies: D-Wave, IonQ, Rigetti

---

## 5. The Benefits of Cloud

### The 6 Advantages of Cloud Computing (according to AWS)
1. **Trade capital expense for variable expense** — Switch from CAPEX to OPEX. No datacenter investment, pay only for what you use
2. **Benefit from massive economies of scale** — AWS buys at massive scale and passes savings to customers
3. **Stop guessing capacity** — No need to guess how much capacity you need; scale up or down based on demand
4. **Increase speed and agility** — Deploy resources in minutes instead of weeks
5. **Stop spending money running and maintaining data centers** — Focus on your business, not on maintaining servers
6. **Go global in minutes** — Deploy your application across multiple regions worldwide in minutes

### The 7th Advantage (added in CLF-C02)
7. **Security** — AWS offers enterprise-grade security. The shared responsibility model ensures AWS protects the infrastructure and you protect your data and configurations

---

## 6. Global Infrastructure

### Overview
- AWS has the largest cloud infrastructure in the world
- Distributed globally for high availability, low latency, and resilience

### Regions
- A **Region** is a geographic area with 2 or more Availability Zones
- Example: `us-east-1` (N. Virginia), `eu-west-1` (Ireland), `sa-east-1` (Sao Paulo)
- **Factors for choosing a Region:**
  1. **Compliance / Regulation:** Data residency laws
  2. **Latency:** Proximity to your users
  3. **Available services:** Not all services are available in every region
  4. **Cost:** Prices vary by region

### Regions vs Global Services
- **Regional Services:** EC2, RDS, Lambda (deployed in a specific region)
- **Global Services:** IAM, Route 53, CloudFront, WAF, S3 (global namespace)

### Availability Zones (AZs)
- Each Region has a **minimum of 3 AZs** (typically 3-6)
- Each AZ is one or more **physical datacenters** with redundant power, networking, and connectivity
- AZs are physically separated (tens of km apart) but connected with high-speed, low-latency fiber
- Named as: `us-east-1a`, `us-east-1b`, `us-east-1c`
- **Designing with multi-AZ is key for high availability**

### Fault Tolerance
- **Fault Domain:** Section of infrastructure that can fail without affecting other sections
- **Fault Level:** Defines how large the failure is (server, rack, datacenter, AZ, Region)
- Distributing resources across multiple AZs protects against datacenter-level failures

### AWS Global Network
- AWS's private fiber optic network connecting all regions and AZs
- Provides high speed and low latency between AWS services

### Points of Presence (PoP)
- Intermediate locations between users and AWS regions
- Used by **CloudFront (CDN)** and **Route 53 (DNS)**
- **400+ PoPs** globally (Edge Locations + Regional Edge Caches)
- **Tier 1 ISPs:** AWS has peering agreements with major internet providers

### AWS Direct Connect
- A **dedicated, private** network connection between your datacenter and AWS
- Does not traverse the public internet
- Provides higher bandwidth, lower latency, and greater consistency
- Ideal for workloads requiring a stable, fast connection

### Direct Connect Locations
- Physical facilities where you can establish a Direct Connect connection
- Operated by AWS partners worldwide

### AWS Local Zones
- Extension of an AWS Region closer to end users
- For workloads requiring **single-digit millisecond** latency
- E.g., gaming, real-time streaming, AR/VR
- Example: `us-east-1-bos-1a` (Boston)

### Wavelength Zones
- AWS infrastructure deployed within 5G telecom operator datacenters
- Ultra-low latency for mobile and edge applications
- Ideal for IoT, mobile gaming, streaming

### Data Residency
- Some countries' laws require data to remain within their borders
- AWS allows you to choose the region where data is stored
- **AWS Outposts:** Extension of AWS in your own datacenter to meet residency requirements

### AWS for Government
- AWS meets government compliance requirements (FedRAMP, ITAR, etc.)
- **AWS GovCloud:** Isolated regions designed for U.S. government workloads
  - Only accessible by authorized U.S. citizens
  - Complies with regulations like ITAR, FedRAMP High, DoD SRG

### AWS in China
- AWS operates in China through local partners (Sinnet, NWCD)
- China regions are **completely isolated** from the rest of AWS
- A separate account and a Chinese business license (ICP License) are required

### Sustainability
- AWS is committed to being **100% renewable energy** by 2025
- It is the largest corporate buyer of renewable energy in the world
- Customers can reduce their carbon footprint by migrating to AWS

### AWS Ground Station
- Fully managed service for controlling **satellite communications**
- Download satellite data directly into AWS
- Use cases: weather, mapping, communications

### AWS Outposts
- AWS hardware installed in **your own datacenter**
- Runs AWS services locally (EC2, EBS, S3, EKS, RDS)
- For workloads that need to remain on-premise due to latency or regulation
- AWS installs, manages, and updates it

---

## 7. Cloud Architecture

### Key Terminologies

| Term | Definition |
|------|-----------|
| **High Availability (HA)** | Your system stays accessible most of the time. Minimal downtime. Uses multi-AZ |
| **High Scalability** | Ability to grow to handle more demand. Vertical (more power) or Horizontal (more instances) |
| **High Elasticity** | **Automatically scales** based on demand. Auto Scaling Groups in AWS |
| **Fault Tolerance** | Ability to keep operating even when a component fails. No downtime for the user |
| **High Durability** | Stored data is not lost. E.g., S3 offers 99.999999999% (11 nines) durability |

### Business Continuity Plan (BCP)
- Plan to ensure the business continues operating during disasters
- Defines **RPO** and **RTO**

### Disaster Recovery Options (from lowest to highest cost and speed)
| Option | Description | RTO |
|--------|-------------|-----|
| **Backup & Restore** | Back up data and restore when disaster strikes | Hours |
| **Pilot Light** | Minimal version of your environment always running | Tens of minutes |
| **Warm Standby** | Scaled-down but fully functional version | Minutes |
| **Multi-site / Hot Standby** | Full copy actively running | Real-time / Seconds |

### RTO (Recovery Time Objective)
- **Maximum acceptable time** to restore service after a disaster
- Example: "Our RTO is 4 hours" = we must be operational within 4 hours

### RPO (Recovery Point Objective)
- **Maximum amount of data you can lose** measured in time
- Example: "Our RPO is 1 hour" = we lose at most 1 hour of data
- More frequent backups = lower RPO = more expensive

---

## 8. Management and Developer Tools

### AWS API
- All AWS services are controlled through an **HTTP API**
- You can interact with AWS via: Web Console, CLI, SDK, IaC

### AWS Management Console
- Web-based graphical interface (GUI) for managing AWS services
- Accessible from the browser at https://console.aws.amazon.com
- Ideal for learning and exploring services
- **Not recommended for production** (better to use IaC)

### AWS Account ID
- Each AWS account has a **unique 12-digit ID**
- Used to uniquely identify your account
- Useful for cross-account access and ARNs

### Amazon Resource Names (ARNs)
- **Globally unique** identifier for any resource in AWS
- Format: `arn:aws:service:region:account-id:resource`
- Example: `arn:aws:s3:::my-bucket`
- Example: `arn:aws:ec2:us-east-1:123456789012:instance/i-1234567890abcdef0`

### AWS CLI (Command Line Interface)
- Command-line tool to interact with AWS
- Installable on Windows, Mac, Linux
- Requires **Access Keys** (Access Key ID + Secret Access Key)
- Example: `aws s3 ls` (list S3 buckets)
- **Widely used in automation and scripting**

### AWS SDK (Software Development Kit)
- Code libraries to interact with AWS from your application
- Available for: Python (boto3), JavaScript, Java, .NET, Go, Ruby, PHP, C++
- Allows integrating AWS services directly into your code

### AWS CloudShell
- Browser-based terminal **within the AWS console**
- Pre-installed with AWS CLI, Python, Node.js, and common tools
- 1 GB of persistent storage per region
- Free (no additional cost)

### AWS Tools for PowerShell
- PowerShell module for managing AWS resources
- Ideal for Windows administrators

### Infrastructure as Code (IaC)
- Practice of defining and managing infrastructure using **configuration files** instead of manual processes
- Benefits: reproducibility, versioning, automation, consistency

### AWS CloudFormation
- **AWS-native** IaC service
- Define infrastructure in **JSON or YAML** files (templates)
- CloudFormation creates, updates, and deletes resources automatically
- Concept of **Stacks**: group of resources managed as a single unit
- Free — you only pay for the resources created

### AWS CDK (Cloud Development Kit)
- Framework to define infrastructure using **programming languages** (TypeScript, Python, Java, C#, Go)
- "Compiles" into CloudFormation templates
- More developer-friendly than writing YAML/JSON directly
- Allows using programming logic (loops, conditionals, functions)

### AWS Toolkit for VS Code
- Visual Studio Code extension for working with AWS
- Allows deploying Lambda functions, viewing logs, exploring resources

### Access Keys
- Credentials for accessing AWS from CLI or SDK
- Composed of: **Access Key ID** (public) + **Secret Access Key** (private)
- **Never share your Access Keys**
- **Never put them in your source code**
- Best practice: use IAM Roles instead of Access Keys whenever possible

---

## 9. Shared Responsibility Model

### Core Concept
- Cloud security is a **shared responsibility** between AWS and the customer
- **AWS is responsible for security "OF" the cloud** (infrastructure)
- **The customer is responsible for security "IN" the cloud** (data, configuration)

### AWS Responsibilities (Security OF the Cloud)
- Physical hardware and datacenters
- Global network infrastructure
- Hypervisors
- Managed service software
- Physical security (guards, access controls, CCTV)

### Customer Responsibilities (Security IN the Cloud)
- Customer data (encryption)
- Platform and application configuration
- Identity and Access Management (IAM)
- OS configuration (patches, updates) on EC2
- Network configuration (Security Groups, NACLs)
- Firewall configuration

### Types of Responsibility by Service

| Model | Customer Responsibility |
|-------|------------------------|
| **IaaS (EC2)** | Maximum — OS, patches, networking, firewall, data |
| **PaaS (Beanstalk, RDS)** | Medium — Data, code, app configuration |
| **SaaS (e.g., S3)** | Minimum — Data and access permissions |

### Shared Responsibility for Compute
- **EC2 (IaaS):** Customer manages OS, patches, security, data
- **Lambda (Serverless):** AWS manages almost everything, customer only their code and data
- **ECS/EKS (Containers):** Depends on whether you use EC2 (more responsibility) or Fargate (less)

---

## 10. Compute

### VMs, Containers & Serverless
| Type | Description | AWS Service |
|------|-------------|-------------|
| **Virtual Machines** | Full virtual server with OS | EC2 |
| **Containers** | Lightweight packaging of application + dependencies | ECS, EKS, Fargate |
| **Serverless** | Run code without managing servers | Lambda |

### AWS Compute Services
- **EC2** (Elastic Compute Cloud): Virtual machines in the cloud, wide variety of instance types
- **ECS** (Elastic Container Service): Docker container orchestration, AWS-native
- **EKS** (Elastic Kubernetes Service): Managed Kubernetes on AWS
- **Fargate**: Serverless engine for containers (no EC2 instances to manage)
- **Lambda**: Serverless functions, pay only per execution (max 15 minutes)
- **Elastic Beanstalk**: PaaS — upload your code and AWS manages the rest
- **AWS Batch**: Process batch workloads at large scale
- **Lightsail**: Simplified VPS for small projects (simple alternative to EC2)

### High Performance Computing (HPC)
- **AWS ParallelCluster**: Create and manage HPC clusters
- **AWS Batch**: For massive batch jobs
- **P and G instances**: NVIDIA GPUs for ML, rendering, simulation
- **Elastic Fabric Adapter (EFA)**: Network interface for HPC with ultra-low latency

### Edge & Hybrid Computing
- **AWS Outposts**: AWS infrastructure in your datacenter
- **AWS Wavelength**: Compute at the edge of 5G networks
- **AWS Local Zones**: Region extension for low latency
- **AWS IoT Greengrass**: Local compute on IoT devices
- **AWS Snow Family**: Physical devices for edge computing and data transfer

### Cost & Capacity Management
- **AWS Savings Plans**: Discounts for usage commitment (1 or 3 years)
- **Spot Instances**: Up to 90% discount for unused capacity
- **Reserved Instances**: Discount for usage commitment
- **AWS Compute Optimizer**: Recommends optimal instance type based on actual usage

---

## 11. Storage Services

### Amazon S3 (Simple Storage Service)
- **Object storage** (files) — virtually unlimited
- Objects are stored in **Buckets**
- Each object can be up to **5 TB**
- Durability: **99.999999999% (11 nines)**
- Use cases: backups, static hosting, data lakes, media files

### S3 Storage Classes
| Class | Use Case | Cost |
|-------|----------|------|
| **S3 Standard** | Frequently accessed data | Higher storage cost |
| **S3 Intelligent-Tiering** | Automatically moves data between tiers based on access patterns | Monitoring cost |
| **S3 Standard-IA** | Infrequently accessed data | Lower storage, higher access cost |
| **S3 One Zone-IA** | Infrequent, non-critical data (single AZ) | Even cheaper |
| **S3 Glacier Instant Retrieval** | Archives with immediate access | Very cheap to store |
| **S3 Glacier Flexible Retrieval** | Archives with retrieval in minutes to hours | Cheaper |
| **S3 Glacier Deep Archive** | Long-term archives (7-10 years), 12-hour retrieval | Cheapest |

### AWS Snow Family
- Physical devices for **transferring large volumes of data** or computing at the edge

| Device | Capacity | Use |
|--------|----------|-----|
| **Snowcone** | 8-14 TB | Small transfers, edge computing |
| **Snowball Edge** | 80 TB (Storage) / 42 TB (Compute) | Medium transfers, edge |
| **Snowmobile** | 100 PB | Massive migrations (a literal truck) |

### Other Storage Services
- **EBS (Elastic Block Store)**: Virtual hard drive for EC2. Persistent. Single AZ. Types: gp3, io2, st1, sc1
- **EFS (Elastic File System)**: Shared file system (NFS) for Linux. Multi-AZ. Auto-scales
- **FSx**: Managed file systems (Windows File Server, Lustre, NetApp ONTAP, OpenZFS)
- **AWS Storage Gateway**: Connects your on-premise storage to the cloud (File Gateway, Volume Gateway, Tape Gateway)
- **AWS Backup**: Centralized service to automatically back up AWS resources

---

## 12. Databases

### Types of Databases

#### Data Warehouse
- Database optimized for **analytics** (OLAP — Online Analytical Processing)
- Stores large volumes of historical data
- **Amazon Redshift** is AWS's data warehouse
- Columnar storage for fast queries over large datasets

#### Key-Value Store
- Simple NoSQL database: key -> value
- Extremely fast and scalable
- **Amazon DynamoDB** is the AWS service (horizontal scale)

#### Document Database
- Stores data in document format (JSON, BSON)
- Flexible, no fixed schema
- **Amazon DocumentDB** (MongoDB-compatible)

### NoSQL Database Services
- **DynamoDB**: Serverless key-value and document DB. Millisecond latency. Auto-scales horizontaly
- **DocumentDB**: MongoDB-compatible
- **Amazon Keyspaces**: Apache Cassandra-compatible
- **Neptune**: Graph database (complex relationships, social networks)
- **Amazon QLDB**: Immutable and verifiable ledger database (blockchain-like)
- **ElastiCache**: In-memory cache (Redis / Memcached). Microsecond latency
- **Amazon MemoryDB for Redis**: Durable in-memory database compatible with Redis

### Relational Database Services (RDBMS)
- **Amazon RDS** (Relational Database Service):
  - Supports: MySQL, PostgreSQL, MariaDB, Oracle, SQL Server
  - Managed by AWS (backups, patches, replicas)
  - Multi-AZ for high availability
- **Amazon Aurora**:
  - MySQL and PostgreSQL compatible
  - **5x faster than MySQL, 3x faster than PostgreSQL**
  - Auto-scales up to 128 TB
  - Aurora Serverless: automatically scales compute capacity
- **Amazon Aurora Global Database**: Replicates across multiple regions for DR

### Other Database Services
- **Redshift**: Petabyte-scale columnar data warehouse
- **Redshift Serverless**: Redshift without managing clusters
- **Amazon Timestream**: Time-series database
- **DMS (Database Migration Service)**: Migrate databases to AWS with minimal downtime

---

## 13. Networking

### Cloud-Native Networking Services
- **VPC** (Virtual Private Cloud): Your private virtual network in AWS
- **Subnets**: Segments within your VPC (public and private)
- **Internet Gateway**: Allows your VPC to connect to the internet
- **NAT Gateway**: Allows private subnets to access the internet (outbound only)
- **Route Tables**: Define traffic routes within your VPC

### Enterprise/Hybrid Networking Services
- **AWS Direct Connect**: Dedicated private connection to AWS
- **AWS VPN (Site-to-Site)**: Encrypted VPN between your network and AWS over the internet
- **AWS Transit Gateway**: Central hub to connect multiple VPCs and on-premise networks
- **AWS PrivateLink**: Access AWS services privately without going to the internet

### VPC & Subnets
- **VPC** spans an entire Region
- **Subnets** exist within a specific AZ
- **Public Subnet**: Has a route to the Internet Gateway (resources accessible from the internet)
- **Private Subnet**: No direct route to the internet (databases, app servers)

### Security Groups vs NACLs
| Feature | Security Groups | NACLs |
|---------|----------------|-------|
| Level | Instance (ENI) | Subnet |
| State | **Stateful** (return traffic is automatic) | **Stateless** (you must define both inbound AND outbound rules) |
| Rules | ALLOW only | ALLOW and DENY |
| Evaluation | All rules are evaluated | Rules evaluated in **numerical order** |
| Default | Denies all inbound, allows all outbound | Allows all inbound and outbound |

### AWS CloudFront
- AWS's global **CDN (Content Delivery Network)**
- Distributes content from **Edge Locations** close to the user
- Reduces latency and improves performance
- Built-in DDoS protection (AWS Shield)
- Works with S3, EC2, ALB, and custom origins
- Supports HTTPS, geo-restriction, and configurable caching

---

## 14. EC2

### EC2 Instance Families
| Family | Optimized For | Example |
|--------|--------------|---------|
| **General Purpose (T, M)** | Balance of compute, memory, networking | t3.micro, m6i.large |
| **Compute Optimized (C)** | Compute-intensive, batch, gaming | c6i.xlarge |
| **Memory Optimized (R, X, z)** | In-memory databases, caches | r6i.large, x2idn |
| **Storage Optimized (I, D, H)** | High sequential I/O, data warehouses | i3.large |
| **Accelerated Computing (P, G, Inf, Trn)** | ML, GPU, HPC, video | p4d.24xlarge |

### EC2 Instance Types — Naming Convention
- Format: `m5.xlarge`
  - `m` = family (general purpose)
  - `5` = generation
  - `xlarge` = size (nano, micro, small, medium, large, xlarge, 2xlarge, etc.)

### Dedicated Hosts vs Dedicated Instances
| | Dedicated Host | Dedicated Instance |
|--|---------------|-------------------|
| **Hardware** | Full physical server for you | Instance on dedicated hardware |
| **Visibility** | You see sockets, cores, host ID | You don't see hardware details |
| **Licensing** | You can bring your own licenses (BYOL) | No |
| **Cost** | More expensive | Less expensive |

### EC2 Tenancy
- **Shared (Default):** Your instance shares hardware with other customers
- **Dedicated Instance:** Dedicated hardware, but AWS manages it
- **Dedicated Host:** Full physical server for you, hardware visibility

### Launching an EC2 — Key Concepts
- **AMI** (Amazon Machine Image): Template for the OS and software
- **Key Pair**: For SSH access (Linux) or RDP access (Windows)
- **Security Group**: Instance firewall
- **User Data**: Script that runs when the instance launches
- **Instance Profile / IAM Role**: AWS permissions for the instance

### Auto Scaling Group (ASG)
- Automatically scales the number of EC2 instances based on demand
- Defines: **min, desired, max** number of instances
- Scaling policies: Target Tracking, Step Scaling, Scheduled
- Automatically replaces failing instances (health checks)

### Application Load Balancer (ALB)
- Distributes traffic across multiple EC2 instances
- Operates at **Layer 7** (HTTP/HTTPS)
- Supports path-based, host-based, and header-based routing
- Integrated with Auto Scaling Groups
- Other LBs: NLB (Layer 4, TCP/UDP), CLB (Legacy), GLB (Layer 3, appliances)

---

## 15. EC2 Pricing Models

### On-Demand
- Pay per **hour or second** with no commitment
- No upfront payment
- Ideal for: unpredictable workloads, development, testing
- **Most expensive** option in the long run

### Reserved Instances (RI)
- Discount of **up to 72%** vs On-Demand for a 1 or 3 year commitment
- **Payment:** All Upfront (highest discount) | Partial Upfront | No Upfront
- Ideal for **predictable, steady-state** workloads

### Reserved Instance Attributes
- Instance type, platform (Linux/Windows), tenancy, region/AZ

### Regional vs Zonal RI
- **Regional RI:** Discount applies to any AZ in the region. Capacity reservation NOT included
- **Zonal RI:** Discount only in the specified AZ. Capacity reservation IS included

### RI Limits
- Maximum 20 RIs per region by default (you can request an increase)

### Capacity Reservations
- Reserve EC2 capacity in a specific AZ without a time commitment
- You pay the On-Demand price whether or not the instance is running
- Useful when you need to guarantee availability

### Standard vs Convertible RI
| | Standard RI | Convertible RI |
|--|------------|----------------|
| **Discount** | Up to 72% | Up to 66% |
| **Change attributes** | No | Yes (family, OS, tenancy) |
| **Sell on Marketplace** | Yes | No |

### RI Marketplace
- You can **sell your unused RIs** to other AWS customers
- Only Standard RIs can be sold

### Spot Instances
- Up to **90% discount** vs On-Demand
- You use AWS's **unused capacity**
- **AWS can reclaim your instance with 2 minutes notice**
- Ideal for: batch processing, big data, CI/CD, fault-tolerant workloads
- **DO NOT use for:** databases, critical workloads

### Dedicated
- **Dedicated Instances:** Dedicated hardware, per-instance cost + per-region charge
- **Dedicated Hosts:** Full physical server, useful for BYOL (Bring Your Own License)

### Savings Plans
- Discount of up to **72%** vs On-Demand for a usage commitment ($/hour) for 1 or 3 years
- **Compute Savings Plan:** Applies to EC2, Lambda, Fargate. Most flexible
- **EC2 Instance Savings Plan:** EC2 only, you specify family and instance. Higher discount
- More flexible than Reserved Instances

---

## 16. Identity

### Zero-Trust Model
- Security model: **"Never trust, always verify"**
- Every request is authenticated and authorized regardless of where it comes from
- Principles: continuous verification, least privilege, assume breach

### Zero-Trust on AWS
- Implemented using a combination of services: IAM, VPC, Security Groups, AWS SSO
- AWS doesn't have a single "Zero Trust" service but rather a combination of services

### Directory Services
- **AWS Directory Service**: Managed Active Directory on AWS
- Options: AWS Managed Microsoft AD, AD Connector, Simple AD

### Active Directory
- Microsoft directory service for managing users and permissions in an enterprise network
- Foundation of corporate authentication on Windows

### Identity Providers (IdP)
- Systems that handle authentication and pass it to your application
- Protocols: **SAML 2.0**, **OpenID Connect (OIDC)**, **OAuth 2.0**
- Examples: Okta, Auth0, AWS SSO, Google, Facebook

### Single Sign-On (SSO)
- Log in once and access multiple applications without re-authenticating
- **AWS IAM Identity Center** (formerly AWS SSO): SSO for multiple AWS accounts and applications

### LDAP
- Protocol for querying and modifying user directories
- Foundation of Active Directory

### Multi-Factor Authentication (MFA)
- Requires **two or more factors** to authenticate: something you know (password) + something you have (token/phone)
- **Always enable MFA**, especially on the root account

### Security Keys
- Physical devices for MFA (YubiKey, FIDO2)
- More secure than authenticator apps
- Phishing-resistant

### AWS IAM (Identity and Access Management)
- **Free** and **global** service to control access to AWS resources
- Main components:
  - **Users**: People or applications
  - **Groups**: Collection of users (e.g., Developers, Admins)
  - **Roles**: Temporary permissions assignable to services or users
  - **Policies**: JSON documents that define permissions (Allow/Deny)

### Anatomy of an IAM Policy
```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::my-bucket/*"
    }
  ]
}
```
- **Effect:** Allow or Deny
- **Action:** What operations are allowed/denied
- **Resource:** Which resources it applies to (ARN)
- **Condition (optional):** Additional conditions

### Principle of Least Privilege
- Grant only the **minimum permissions necessary** to perform a task
- Fundamental security concept in AWS
- Start with no permissions and add only what's needed

### AWS Account Root User
- User with **complete, unrestricted access** to all resources
- Created when the AWS account is created
- **Root-only tasks:** change support plan, close account, change account settings
- **Never use root for daily tasks** — create IAM users
- **Always enable MFA on root**

### AWS SSO (IAM Identity Center)
- Service for managing SSO access to multiple AWS accounts and business applications
- Integrates with Active Directory and SAML 2.0 identity providers
- Centralized portal for users to access all their accounts

---

## 17. Application Integration

### Queuing & Amazon SQS
- **Amazon SQS** (Simple Queue Service): Fully managed message queuing service
- Decouples application components
- **Standard Queue:** Best-effort ordering, unlimited throughput
- **FIFO Queue:** Strict ordering (First-In-First-Out), 300 msg/sec
- Messages persist until processed or expired

### Streaming & Amazon Kinesis
- **Amazon Kinesis**: **Real-time** streaming data processing
- **Kinesis Data Streams**: Real-time streaming ingestion
- **Kinesis Data Firehose**: Load streaming data to S3, Redshift, etc.
- **Kinesis Data Analytics**: SQL/Apache Flink analytics on streaming data
- Use cases: real-time logs, IoT, clickstream analytics

### Pub/Sub & Amazon SNS
- **Amazon SNS** (Simple Notification Service): Pub/Sub (publish/subscribe) service
- A publisher sends a message to a **Topic**
- All subscribers of the Topic receive the message
- Subscribers: email, SMS, Lambda, SQS, HTTP endpoints, mobile push
- Useful for alerts, notifications, fan-out

### API Gateway & Amazon API Gateway
- **Amazon API Gateway**: Create, publish, and manage APIs (REST, HTTP, WebSocket)
- Handles authentication, rate limiting, caching, transformation
- Integrates with Lambda to create serverless APIs

### State Machines & AWS Step Functions
- **AWS Step Functions**: Orchestrates multiple AWS services into workflows
- Define flows using **Amazon States Language** (JSON) or visual Workflow Studio
- Ideal for coordinating microservices and complex processes

### Event Bus & Amazon EventBridge
- **Amazon EventBridge** (formerly CloudWatch Events): Serverless event bus
- Connects applications using events from AWS, SaaS, or your own apps
- Rule-based routing
- Ideal for event-driven architectures

### Other Application Integration Services
- **Amazon MQ**: Managed message broker (ActiveMQ, RabbitMQ) for on-premise migrations
- **AWS AppSync**: Managed GraphQL API, real-time sync
- **Amazon AppFlow**: Data integration between SaaS (Salesforce, SAP) and AWS

---

## 18. Containers

### VMs vs Containers
| Feature | VMs | Containers |
|---------|-----|-----------|
| **Isolation** | Complete (own OS) | Share the host kernel |
| **Size** | GBs | MBs |
| **Startup** | Minutes | Seconds |
| **Overhead** | High | Low |
| **Density** | Fewer VMs per host | Many containers per host |

### Microservices
- Architecture where each application function is an independent service
- Each microservice can be deployed, scaled, and updated independently
- Containers are ideal for microservices

### Kubernetes
- Open-source platform for orchestrating containers
- Handles deployment, scaling, networking of containers
- **AWS EKS** (Elastic Kubernetes Service): Managed Kubernetes on AWS

### Docker
- Open-source platform for building, packaging, and running applications in containers
- **Dockerfile**: Defines how to build the image
- **Docker Image**: Immutable template
- **Docker Container**: Running instance of an image
- **Amazon ECR** (Elastic Container Registry): Private Docker image repository

### Podman
- Alternative to Docker, daemonless, rootless by default
- Compatible with Docker images and commands

### Container Services on AWS
- **ECS** (Elastic Container Service): AWS-native container orchestration
- **EKS** (Elastic Kubernetes Service): Managed Kubernetes
- **Fargate**: Serverless engine for containers (no EC2 management needed)
- **ECR** (Elastic Container Registry): Docker image registry
- **AWS App Runner**: Simplified container/source code deployment (PaaS-like)
- **AWS Copilot**: CLI for easily deploying containers on ECS/Fargate

---

## 19. Governance

### Organizations & Accounts
- **AWS Organizations**: Centrally manage multiple AWS accounts
- **Root Account User**: Complete access to all AWS services
- **Organizational Units (OUs)**: Logical grouping of accounts
- **Service Control Policies (SCPs)**: Policies that restrict what accounts can do
- **Consolidated Billing**: Single bill for all accounts + volume discounts
- Typical structure: Root Account > OUs > Member Accounts

### AWS Control Tower
- Set up and govern a **secure, compliant** multi-account environment
- Automates account creation with best practices
- **Guardrails**: Governance rules (preventive and detective)
- Uses: AWS Organizations, AWS SSO, AWS Config, CloudTrail
- **Landing Zone**: Well-configured multi-account environment set up automatically

### AWS Config
- Service that **audits and evaluates the configuration** of your AWS resources per region basis
- Is a Compliance-as-Code (CaC)
- Use to configure a resources in a specific way
- Keep track of of configuration changes
- List of all resources of a region
- Does not prevent changes, only **detects and reports** them

### AWS Quick Starts
- CloudFormation templates and deployment guides created by AWS and partners
- Deploy popular architectures in minutes
- Available in the **AWS Solutions Library**

### Tagging
- **Tags** are key-value pairs you assign to AWS resources
- E.g., `Environment: Production`, `Team: DevOps`, `Project: WebApp`
- Uses: organization, cost control, automation, access control
- **Best practice:** Define a consistent tagging strategy

### Resource Groups
- Collection of AWS resources grouped by tags
- Allows viewing and managing related resources as a unit
- **Tag Editor**: Tool for searching and tagging resources in bulk

### Business Centric Services
- **Amazon Connect**: Cloud-based contact center
- **Amazon WorkSpaces**: Virtual desktops (VDI)
- **Amazon WorkDocs**: Enterprise document storage and sharing
- **Amazon Chime**: Video conferencing and chat
- **Amazon WorkMail**: Managed enterprise email
- **Amazon Pinpoint**: Marketing service to send targeted email via SMS
- **Amazon Email Service (SES)**: Transactional email service
- **Amazon QuickSight**: Business Intelligence (BI) service

---

## 20. Provisioning

### Provisioning Services
The allocation or creation of resources and services to a customer.

| Service                             | Description                                   |
| ----------------------------------- | --------------------------------------------- |
| **CloudFormation**                  | IaC with YAML/JSON templates                  |
| **Elastic Beanstalk**               | PaaS — upload your code                       |
| **AWS OpsWorks**                    | Configuration management with Chef and Puppet |
| **AWS QuickStarts**                 | Premade packages to launch and configure      |
| **AWS Marketplace**                 | Digital catalogue of software listings        |
| **AWS Amplify**                     | A mobile and web-application framework        |
| **AWS App Runner**                  | Makes easy to deploy containers               |
| **AWS Copilot**                     | CLI to quickly launch and manage applications |
| **AWS CodeStar**                    | User interface to manage software development |
| **AWS Cloud Development Kit (CDK)** | IaC tool to use any programming language      |

### AWS Elastic Beanstalk
- AWS **PaaS** (Platform as a Service)
- Not recommended for Production (only for big companies)
- Upload your code and Beanstalk automatically:
  - Provisions EC2, Load Balancers, Auto Scaling...
  - Configures monitoring, logging
  - Manages deployments and rollbacks
- Supports: Java, .NET, PHP, Node.js, Python, Ruby, Go, Docker
- You retain full control over the underlying resources if needed
- **Free** — you only pay for the resources created (EC2, RDS, etc.)

---

## 21. Serverless

### Serverless Services on AWS
The underlying servers, infrastructure and OS is taken care of by the CSP.

| Service               | Function                                                                            |
| --------------------- | ----------------------------------------------------------------------------------- |
| **AWS Lambda**        | Run code without servers. Max 15 min per execution. Pay per invocation and duration |
| **ECS Fargate**       | Serverless orchestration container service                                          |
| **Amazon S3**         | Serverless object storage                                                           |
| **DynamoDB**          | Serverless NoSQL database                                                           |
| **Aurora Serverless** | Serverless on-demand version of Aurora (relational database)                        |
| **Amazon SQS**        | Serverless message queue                                                            |
| **Amazon SNS**        | Serverless notifications                                                            |
| **API Gateway**       | Serverless APIs                                                                     |
| **Step Functions**    | State machine service                                                               |
| **EventBridge**       | Serverless event bus                                                                |
| **Amazon Cognito**    | Serverless user authentication                                                      |

**Serverless = No server management, auto-scales, pay per use**

---

## 22. Windows on AWS

### EC2 Windows
- You can launch EC2 instances with Windows Server
- Windows license included in the instance price (License Included)
- Access via **RDP** (Remote Desktop Protocol) port 3389
- Supports: IIS, SQL Server, Active Directory, .NET Framework

### AWS License Manager
- Manage software licenses from Microsoft, Oracle, SAP, etc.
- For Microsoft Windows Server and Microsoft SQL Server license you need to use a **Dedicated Host**
- Options:
  - **License Included (LI):** AWS provides the license
  - **Bring Your Own License (BYOL):** Bring your existing licenses

---

## 23. Logging

### AWS CloudTrail
- Records **all API calls** made in your AWS account
- Answers: Where, When Who and What 
- Essential for auditing, compliance, and security
- Trails saved in S3, to analyze use **Amazon Athena**
- **CloudTrail is for AUDITING (who did what)**

### Amazon CloudWatch
- AWS **monitoring and observability** service
- Main components: Logs, Metrics, Events, Alarms, Dashboards

#### CloudWatch Alarms
- Alerts when a metric crosses a defined threshold
- Actions: SNS notification, Auto Scaling, EC2 action (stop, terminate, reboot)
- **Anatomy of an Alarm:**
  - Metric (e.g., CPU Utilization)
  - Threshold (e.g., > 80%)
  - Evaluation period (e.g., 5 minutes)
  - Action (e.g., send email via SNS)

#### CloudWatch Logs
- **Log Events**: Individual activity records
- **Log Groups**: Collection of Log Streams from the same source
- **Log Streams**: Sequence of Log Events from a specific source
- You can configure retention (1 day to 10 years or never expire)

#### CloudWatch Logs Insights
- Query and analyze logs using an interactive query language
- Search patterns, filter, aggregate log data

#### CloudWatch Metrics
- Performance metrics for AWS services
- Default metrics: CPU, NetworkIn/Out, DiskRead/Write
- **Custom Metrics**: Your own metrics via PutMetricData API

**Summary:**
- **CloudTrail** = AUDITING (who did what)
- **CloudWatch** = MONITORING (how are resources performing)

---

## 24. ML, AI & Big Data

### Intro to ML & AI
- **AI (Artificial Intelligence):** Machines that mimic human intelligence
- **ML (Machine Learning):** Subset of AI; machines learn from data without being explicitly programmed
- **Deep Learning:** Subset of ML using deep neural networks

### AI & ML Services on AWS
| Service                       | Function                                                          |
| ----------------------------- | ----------------------------------------------------------------- |
| **Amazon SageMaker**          | Complete platform for building, training, and deploying ML models |
| **Amazon Rekognition**        | Image and video analysis (face detection, objects, text)          |
| **Amazon Transcribe**         | Speech-to-Text (audio to text)                                    |
| **Amazon Polly**              | Text-to-Speech (text to voice)                                    |
| **Amazon Translate**          | Automatic language translation                                    |
| **Amazon Comprehend**         | Natural Language Processor (NLP). Looks data.                     |
| **Amazon Lex**                | Conversational chatbots (the technology behind Alexa)             |
| **Amazon Textract**           | Extracts text and data from documents/PDFs                        |
| **Amazon Forecast**           | Time-series predictions using ML                                  |
| **Amazon Personalize**        | Personalized recommendations (like Amazon.com)                    |
| **Amazon Kendra**             | Intelligent enterprise search powered by ML                       |
| **Amazon CodeWhisperer**      | AI programming assistant (code suggestions)                       |
| **Amazon Bedrock**            | Access to generative AI foundation models from multiple providers |
| **Amazon Deep Learning AMIs** | Pre-installed with popular deep learning frameworkd               |

### Big Data & Analytics Services
Big Data: Term to describe massive volumes of structured/unstructured data

| Service                | Function                                                              |
| ---------------------- | --------------------------------------------------------------------- |
| **Amazon Redshift**    | Petabyte-scale data warehouse for analytics                           |
| **Amazon Athena**      | SQL queries on S3 data (serverless, pay per query)                    |
| **Amazon EMR**         | Managed Hadoop/Spark for big data processing                          |
| **Amazon Kinesis**     | Real-time streaming processing                                        |
| **AWS Glue**           | Serverless ETL (Extract, Transform, Load) + Data Catalog              |
| **Amazon OpenSearch**  | Log search and analytics (formerly ElasticSearch)                     |
| **Amazon QuickSight**  | BI (Business Intelligence) — serverless dashboards and visualizations |
| **AWS Data Pipeline**  | Orchestration of data movement and transformation                     |
| **AWS Lake Formation** | Create and manage Data Lakes securely                                 |
| **Amazon MSK**         | Managed Apache Kafka                                                  |
| **Amazon CloudSearch** | Full-text search service                                              |
| **Amazon Bedrock**     | LLM to generate text and image responses                              |

### Amazon QuickSight
- **Serverless Business Intelligence** (BI) service
- Creates interactive dashboards and visualizations
- Connects to: S3, RDS, Redshift, Athena, and more
- **SPICE** technology (Super-fast, Parallel, In-memory Calculation Engine)
- Pay per session (per use)

### Generative AI
- **Amazon Bedrock**: Access to Foundation Models (FM) from AI21 Labs, Anthropic, Cohere, Meta, Stability AI, and Amazon Titan
- Allows building generative AI applications without training models from scratch
- **Amazon CodeWhisperer**: AI pair programmer for code suggestions

### ML & DL Frameworks
- AWS supports: TensorFlow, PyTorch, Apache MXNet
- **AWS Deep Learning AMIs**: Pre-configured AMIs with ML frameworks
- **AWS Deep Learning Containers**: Docker containers with ML frameworks

### GPUs on AWS
- Instances with NVIDIA GPUs for ML training/inference
- **CUDA**: NVIDIA's parallel computing platform for GPUs
- Families: P (training), G (graphics/inference), Inf (Inferentia), Trn (Trainium)
- **AWS Trainium**: AWS-designed chip for ML training
- **AWS Inferentia**: AWS-designed chip for ML inference

---

## 25. AWS Well-Architected Framework

### Overview
- **Best practices** guide for designing systems in the cloud
- Created by AWS Solutions Architects with real-world experience
- Helps evaluate and improve your architectures

### General Design Principles
1. Stop guessing your capacity needs
2. Test systems at production scale
3. Automate to make architectural experimentation easier
4. Allow for evolutionary architectures
5. Drive architectures using data
6. Improve through Game Days (simulations)

### The 6 Pillars of the Well-Architected Framework

#### 1. Operational Excellence
- Run and monitor systems to deliver business value
- Continuous improvement of processes and procedures
- Key principles: Operations as code, frequent small reversible changes, anticipate failure
- Services: CloudFormation, Config, CloudTrail, CloudWatch, X-Ray

#### 2. Security
- Protect information, systems, and assets
- Key principles: Implement a strong identity foundation, traceability, security at all layers, automate best practices, protect data in transit and at rest, prepare for security events
- Services: IAM, CloudTrail, KMS, WAF, Shield, GuardDuty, Inspector, Macie

#### 3. Reliability
- Ability to recover from failures and scale to meet demand
- Key principles: Test recovery procedures, scale horizontally, stop guessing capacity, automate changes, automatic recovery
- Services: CloudWatch, CloudFormation, S3, Glacier, Route 53

#### 4. Performance Efficiency
- Use compute resources efficiently and maintain efficiency over time
- Key principles: Democratize advanced technologies, go global in minutes, use serverless architectures, experiment frequently
- Services: Auto Scaling, Lambda, EBS, S3, RDS, CloudFront

#### 5. Cost Optimization
- Avoid unnecessary spending
- Key principles: Implement Cloud Financial Management, adopt a consumption model, measure efficiency, stop spending on undifferentiated heavy lifting
- Services: Cost Explorer, Budgets, Reserved Instances, Spot Instances, Trusted Advisor

#### 6. Sustainability (New in WAF)
- Minimize the environmental impact of cloud workloads
- Principles: Understand your impact, establish sustainability goals, maximize utilization, use managed services, reduce downstream impact

### AWS Well-Architected Tool
- **Free** tool in the AWS console
- Evaluates your architecture against the 6 pillars by answering questions
- Generates a **report with improvement recommendations**
- Available at AWS Console > Well-Architected Tool

### AWS Architecture Center
- Online resource with **reference diagrams, whitepapers, and guides**
- Reference architectures for common use cases
- https://aws.amazon.com/architecture/

---

## 26. TCO and Migration

### Total Cost of Ownership (TCO)
- Financial comparison of the **total cost** of on-premise vs cloud
- On-premise includes: hardware, licenses, electricity, cooling, personnel, physical space, maintenance
- In the cloud you only pay for what you use, no hidden infrastructure costs

### CAPEX vs OPEX
|                     | CAPEX (Capital Expenditure)                                                       | OPEX (Operational Expenditure)              |
| ------------------- | --------------------------------------------------------------------------------- | ------------------------------------------- |
| **What**            | Upfront capital expense (buying servers, datacenter, physical security, hardware) | Ongoing operational expense (pay-as-you-go) |
| **Cloud**           | N/A                                                                               | Cloud is OPEX — monthly payments            |
| **On-Premise**      | High upfront CAPEX                                                                | Lower OPEX but fixed costs                  |
| **Cloud advantage** | No upfront investment                                                             | Flexible, scales with the business          |

### Shifting IT Personnel
- When migrating to the cloud, IT staff move from maintaining hardware to higher-value tasks
- A company can change employees activities from **Managing Infrastructure to Revenue Generating**
- Focus on architecture, automation, optimization, and security

### AWS Pricing Calculator
- Tool to **estimate costs** of AWS services before using them
- Allows building scenarios and comparing options
- https://calculator.aws/
- Replacement for the former Simple Monthly Calculator and TCO Calculator

### Migration Evaluator
- Tool to create a **business case** for AWS migration
- Analyzes your current on-premise environment
- Provides a cost projection on AWS
- Formerly known as TSO Logic

### VM Import/Export
- Allows **importing** VM images from your environment to EC2
- Allows **exporting** EC2 instances back to your environment
- Supports: VMware, Hyper-V, Citrix Xen

### Database Migration Service (DMS)
- Migrate databases to AWS with **minimal downtime**
- Supports homogeneous migrations (e.g., MySQL to MySQL) and heterogeneous (e.g., Oracle to Aurora)
- **AWS Schema Conversion Tool (SCT)**: Converts database schemas for heterogeneous migrations
- The source database remains operational during migration

### Cloud Adoption Framework (AWS CAF)
- AWS guide for planning cloud migration
- **6 Perspectives:**
  1. **Business**: Aligning IT with business objectives
  2. **People**: Culture, organization, training
  3. **Governance**: IT governance, risk management
  4. **Platform**: Architecture, patterns, services
  5. **Security**: Security, compliance, controls
  6. **Operations**: Cloud operations, monitoring

---

## 27. Billing and Pricing

### AWS Free Services
AWS services that have **no cost** (but the resources they create do):
- IAM, VPC, Organizations, Consolidated Billing
- Elastic Beanstalk (you only pay for resources), CloudFormation, Auto Scaling Groups
- AWS Free Tier services

### AWS Support Plans
| Plan | Cost | Features |
|------|------|----------|
| **Basic** | Free | Access to documentation, whitepapers, forums. 24/7 customer service for billing. Trusted Advisor (7 basic checks). Personal Health Dashboard |
| **Developer** | From $29/month | Everything in Basic + technical support via email (business hours). 1 primary contact. Response: < 24h general, < 12h system impaired |
| **Business** | From $100/month | Everything in Developer + 24/7 phone support. Unlimited contacts. **All Trusted Advisor checks**. Response: < 1h for production system down. AWS Support API |
| **Enterprise On-Ramp** | From $5,500/month | Everything in Business + pool of Technical Account Managers. Response: < 30min for business-critical. Concierge Support Team |
| **Enterprise** | From $15,000/month | Everything above + **dedicated TAM**. Response: < 15min for business-critical. Infrastructure Event Management. Well-Architected Reviews |

### TAM (Technical Account Manager)
- Available only on **Enterprise On-Ramp** and **Enterprise** plans
- Your dedicated technical point of contact at AWS
- Helps with best practices, optimization, architecture planning
- Coordinates access to AWS programs and experts

### AWS Marketplace
- Digital catalog with **thousands of software listings** from independent vendors (ISVs)
- Categories: security, networking, storage, ML, DevOps, BI
- Models: AMI, SaaS, Containers, Professional Services
- Billing integrates with your AWS bill

### Consolidated Billing
- Feature of **AWS Organizations**
- Single bill for all accounts in the organization
- **Volume discounts**: Combined usage across all accounts may generate volume discounts
- Simplifies cost tracking per account

### AWS Trusted Advisor
- Service that **inspects your environment** and makes recommendations in 5 categories:
  1. **Cost Optimization**: Underutilized resources, unused RIs
  2. **Performance**: Bottlenecks, service limits
  3. **Security**: Open permissions, MFA not enabled
  4. **Fault Tolerance**: Backups, multi-AZ, redundancy
  5. **Service Limits**: Usage nearing service limits
- **Basic/Developer:** 7 basic checks (Core checks) including S3 bucket permissions, Security Groups, IAM use, MFA on root, EBS snapshots, RDS snapshots, Service Limits
- **Business/Enterprise:** **All checks** + API access + CloudWatch integration

### SLAs (Service Level Agreements)
- Service level agreements that AWS guarantees
- If AWS doesn't meet them, you receive service credits
- Example: EC2 SLA = 99.99% monthly uptime
- If uptime is < 99.99%, you receive credits between 10-100% of your bill for the affected service}

### SLI (Service Level Indicator)
- Metric/measurement that indicates what measure of performance a costumer is receiving
- Could be uptime, performance, availability, latency...

### SLO (Service Level Objective)
- The objective that the provider has agreed to meet
- Represented as a specific target percentage over a period of time

### SLA Examples12

| Service | SLA |
|---------|-----|
| EC2 | 99.99% |
| S3 | 99.9% (availability) |
| RDS Multi-AZ | 99.95% |
| Lambda | 99.95% |
| CloudFront | 99.9% |

### Service Health Dashboard
- Shows the status of **all AWS services** globally
- Overview of current and past incidents
- https://health.aws.amazon.com/health/status

### AWS Personal Health Dashboard
- Shows events that affect **your specific resources**
- Proactive, personalized alerts
- Accessible from the console as **AWS Health Dashboard**
- Shows scheduled maintenance, performance issues, etc.

### AWS Abuse
- Channel to report **abusive use** of AWS resources
- Report: spam, port scanning, DDoS, malware, illegal content
- Contact: email-abuse@amazon.com / trustandsafety@support.aws.com or web form in console

### AWS Free Tier
- Reminder: 3 types (Always Free, 6 Months Free, Trials)
- $200 in credits
- Check https://aws.amazon.com/free/ for updated details
- Set up **AWS Budgets** to avoid exceeding the Free Tier

### AWS Credits
- Coupons applied to your AWS bill
- Obtained via: events, AWS programs, AWS Activate (startups), promotions
- Applied automatically to your bill

### AWS Partner Network (APN)
- Global network of AWS partners
- **Technology Partners**: Software/SaaS providers that integrate with AWS
- **Consulting Partners**: Consulting firms that help migrate to and use AWS
- **Training Partners**: Organizations authorized to deliver AWS training

### AWS Budgets
- Create **cost, usage, or reservation** budgets
- Alerts when you exceed or approach the budget
- **Budget Reports**: Scheduled budget reports sent via email

### AWS Cost & Usage Reports (CUR)
- The **most detailed** cost and usage report available
- Data by hour, day, or month; broken down by service, resource, tags
- Exported to S3 in CSV format
- Can be analyzed with Athena, Redshift, QuickSight

### Cost Allocation Tags
- Specific tags for cost tracking
- **AWS-generated tags**: Automatically created by AWS (e.g., aws:createdBy)
- **User-defined tags**: Created by you (e.g., Department, Project)
- Must be **activated** in the Billing console to appear in reports

### Billing Alarms
- CloudWatch alarms based on estimated charges
- Configured in the **us-east-1** region
- Difference vs Budgets: Billing Alarms are basic, Budgets are more advanced

### AWS Cost Explorer
- Visual tool to **analyze and understand** your AWS spending over time
- Filter by service, account, region, tag, etc.
- Cost forecasting (12 months)
- Savings Plans and Reserved Instances recommendations
- Free

### Programmatic Pricing APIs
- **Price List API**: Gets current AWS service prices
- **Savings Plans Purchase Recommendation API**: Savings Plans recommendations
- Useful for integrating pricing data into your internal tools
- JSON or HTML

### AWS Savings Plans
- Discounts for spending commitment ($/hour) for 1 or 3 years
- **Compute Savings Plans**: Most flexible, applies to EC2, Lambda, Fargate
- **EC2 Instance Savings Plans**: Specific to EC2 family in a region
- **SageMaker Savings Plans**: For SageMaker usage
- Managed from **AWS Cost Explorer > Savings Plans**

### AWS Service Quotas
- View and manage your service quotas at scale as your AWS workloads grow.
- Manage your AWS service quotas from one central location

## 28. Defence in Depth

### Stages
1. **Data**: Encryption and protection of sensitive information. 
2. **Application**: Ensuring software is secure and vulnerability-free. 
3. **Compute**: Securing virtual machines and managing access ports. 
4. **Network**: Resource segmentation and communication control. 
5. **Perimeter**: Defense against external threats like DDoS attacks. 
6. **Identity**: Access management and infrastructure change control. 
7. **Physical**: Restricting physical access to hardware and data centers.

### Confidentiality, Integrity, Availability (CIA) Triad
The **CIA triad** is a foundational model in security principles that describes the relationship and trade-offs between three core concepts. 
#### Confidentiality 
* **Definition:** Protecting data from unauthorized viewers.
* **In Practice:** Using cryptographic keys for encryption and implementing "envelope encryption" (encrypting keys with other keys). 
#### Integrity 
* **Definition:** Ensuring the accuracy and completeness of data throughout its entire lifecycle. 
* **In Practice:** Using ACID-compliant databases for transactions and employing Hardware Security Modules (HSM) that are tamper-evident or tamper-proof. 
#### Availability 
* **Definition:** Ensuring information is accessible whenever it is needed. 
* **In Practice:** Implementing High Availability (HA) systems, mitigating DDoS attacks, and ensuring proper decryption access.  
#### History and Evolution 
* **Origin:** First mentioned in a **NIST publication in 1977**. 
* **Modernization Efforts:** 
  * **1998:** Expanded to the "Six Atomic Elements of Information" (Confidentiality, Possession, Integrity, Authenticity, Availability, and Utility). 
  * **2004:** NIST Engineering Principles for IT Security introduced 33 security principles.

## Vulnerabilities
A hole or a weakness in the application, which can be a design flaw or an implementation bug, that allows an attacker to cause harm.

#### Examples
- Buffer Overflow
- Improper Data Validation
- Least Privilege Violation
- Memory leak
- Using a broken or risky cryptographic algorithm

### Encryption
#### What is Cryptography? 
Cryptography is the practice and study of techniques used to ensure **secure communication** even in the presence of third-party adversaries. 
#### What is Encryption? 
Encryption is the specific process of encoding (scrambling) information to store sensitive data in an unintelligible format for protection. 
* **Mechanism**: It uses a **key** and a **cypher** (algorithm). 
* **Input**: Plaintext (readable data). 
* **Output**: Ciphertext (unreadable/protected data).

## Cryptographic Keys
- **Cryptographic Key**: A variable used with an algorithm to encrypt or decrypt data. 
- **Symmetric Encryption**: Uses the **same key** for both encryption and decryption. *Example:* AES 
- **Asymmetric Encryption**: Uses **two different keys** (one to encode, one to decode). - *Example:* RSA

## Hashing and Salting
- **Hashing**: A **one-way**, **deterministic** function that turns any input into a fixed-size string. 
  - *Purpose*: Securely store passwords (only the hash is stored, not the plaintext). 
  - *Common Functions*: MD5, SHA256, Bcrypt. 
- **Salting**: Adding a **random string** (salt) to the password before hashing. 
  - *Purpose*: Breaks the deterministic nature of hashing to prevent dictionary and rainbow table attacks.

## In-Transit vs. At-Rest Encryption 
- **Encryption In-Transit**: Protects data while it is **moving** between locations. 
  - *Protocols*: **TLS** (v1.2/1.3 are current best practices) and **SSL** (deprecated). 
- **Encryption At-Rest**: Protects data while it is **stored** on a disk or in a database. 
  - *Algorithms*: **AES**, **RSA**.

## AWS Artifact
- Is a self-serve portal for on-demand access to AWS compliance reports
- Get ISO certifications, SOC reports, PCI reports and GDPR data processing agreements

## AWS Inspector
- Runs a security benchmark against specific EC2 intances.
- Can be perform both Network and Host
- Run by CIS, has 699 checks

## AWS Shield
- Is a manages DDoS protection service
- **Shield Standard (Free)**: protection against mos  common DDoS attacks
- **Shield Advance (3000 USD / Year)**: additional protection against larger and more sophisticated attacks

## Amazon Guard Duty
- Is a threat detection service that continuously monitors for malicious, suspicious activity.
- Analyze: CloudTrail, VPC Flow, DNS logs

## AWS Web Application Firewall (WAF)
- Protect your web apps from common web exploits
- Write own rutes to ALLOW or DENY.
- Cover the OWASP Top 10

## Know Your Initialisms
| Sigla    | Significado                    |
| :------- | :----------------------------- |
| **IAM**  | Identity and Access Management |
| **S3**   | Simple Storage Service         |
| **SWF**  | Simple Workflow Service        |
| **SNS**  | Simple Notification Service    |
| **SQS**  | Simple Queue Service           |
| **SES**  | Simple Email Service           |
| **SSM**  | Simple Systems Manager         |
| **RDS**  | Relational Database Service    |
| **VPC**  | Virtual Private Cloud          |
| **VPN**  | Virtual Private Network        |
| **CFN**  | CloudFormation                 |
| **WAF**  | Web Application Firewall       |
| **MQ**   | Amazon ActiveMQ                |
| **ASG**  | Auto Scaling Groups            |
| **TAM**  | Technical Account Manager      |
| **ELB**  | Elastic Load Balancer          |
| **ALB**  | Application Load Balancer      |
| **NLB**  | Network Load Balancer          |
| **GWLB** | Gateway Load Balancer          |
| **CLB**  | Classic Load Balancer          |
| **EC2**  | Elastic Cloud Compute          |
| **ECS**  | Elastic Container Service      |
| **ECR**  | Elastic Container Repository   |
| **EBS**  | Elastic Block Storage          |
| **EFS**  | Elastic File Storage           |
| **EMR**  | Elastic MapReduce              |
| **EB**   | Elastic Beanstalk              |
| **ES**   | Elasticsearch                  |
| **EKS**  | Elastic Kubernetes Service     |
| **MSK**  | Managed Kafka Service          |
| **RAM**  | AWS Resource Manager           |
| **ACM**  | Amazon Certificate Manager     |
| **PoLP** | Principle of Least Privilege   |
| **IoT**  | Internet of Things             |
| **RI**   | Reserved Instances             |

---

## Exam Summary

### Tips to Pass the CLF-C02
1. Focus on the **4 exam domains** (Cloud Concepts 24%, Security 30%, Technology 34%, Billing 12%)
2. Understand the **Shared Responsibility Model** well — it appears in MANY questions
3. Know the differences between **Security Groups and NACLs**
4. Know the **EC2 pricing models** (On-Demand, Reserved, Spot, Savings Plans)
5. Understand the **6 pillars of the Well-Architected Framework**
6. Know the **6+1 advantages of Cloud Computing**
7. Differentiate between similar services (e.g., CloudTrail vs CloudWatch, SQS vs SNS)
8. Understand Region vs AZ vs Edge Location
9. Know the **Support Plans** and what each one includes
10. Practice with mock exams before the real exam

### Key Services You Should Know
| Category | Services |
|----------|----------|
| Compute | EC2, Lambda, ECS, Fargate, Lightsail, Elastic Beanstalk |
| Storage | S3, EBS, EFS, Glacier, Snow Family |
| Database | RDS, Aurora, DynamoDB, Redshift, ElastiCache |
| Networking | VPC, CloudFront, Route 53, Direct Connect, API Gateway |
| Security | IAM, KMS, WAF, Shield, GuardDuty, Inspector, Macie |
| Management | CloudWatch, CloudTrail, Config, Trusted Advisor, Organizations |
| Cost | Cost Explorer, Budgets, Pricing Calculator, Savings Plans |

---

> **Note:** These notes cover the main topics from Andrew Brown's course for the CLF-C02 exam. It is recommended to supplement with official AWS documentation and practice exams.
