# 📘 Lecture 2: Cloud Computing - Amazon Services

***

#### 📌 Topics of Lecture

1. **Elastic Compute Cloud (EC2)**
2. **Instance Types**
3. **Security Groups**
4. **Elastic Block Storage (EBS)**
5. **Elastic Load Balancers (ELB)**
6. **Auto Scaling Group (ASG)**
7. **Relational Database Service (RDS)**
8. **Simple Storage Service (S3)**

***

#### 🌐 Elastic Compute Cloud (EC2)

* **Amazon EC2** provides virtual machines and is an **Infrastructure as a Service (IaaS)**.
* Key capabilities:
  * Renting virtual machines (EC2)
  * Storing data on virtual drives (EBS)
  * Distributing load (ELB)
  * Scaling services (ASG)

**EC2 Configuration Options:**

* OS: Linux, Windows, Mac OS
* CPU, RAM, storage options
* Network settings, firewall rules (security group), and bootstrapping with **EC2 User Data**

***

#### 🖥️ EC2 User Data

* **User Data** allows commands to run at the machine’s first start:
  * Installing updates/software
  * Initial configuration

**Sample User Data Script:**

```bash
bashCopy code#!/bin/bash
apt update -y
apt install -y apache2
systemctl enable apache2
echo "<h1>machine2</h1>" > /var/www/html/index.html
```

**💡 Exam Questions:**

1. What is Amazon EC2, and how does it differ from traditional data centers?
2. Explain the purpose of EC2 User Data and provide a sample script.

***

#### ⚙️ EC2 Instance Types

Amazon offers EC2 instances optimized for specific workloads:

1. **General Purpose** 📊 – Balanced compute, memory, storage (e.g., T2, M5)
2. **Compute Optimized** 💻 – For compute-intensive tasks like HPC, gaming (e.g., C5)
3. **Memory Optimized** 🧠 – For large in-memory workloads (e.g., R5, X1)
4. **Storage Optimized** 💾 – For storage-intensive tasks (e.g., I3, D2)

**💡 Exam Questions:**

1. Differentiate between general-purpose and compute-optimized EC2 instances.
2. List use cases for memory-optimized EC2 instances.

***

#### 🔐 Security Groups

* **Security Groups** act as firewalls for EC2 instances, controlling inbound and outbound traffic.
* Rules:
  * Defined by IP or security group
  * Default allows all outbound traffic; SSH only for inbound by default

**Shared Responsibility Model for EC2:**

* AWS manages global network security and physical hardware.
* User manages OS patches, software updates, and IAM roles.

**💡 Exam Questions:**

1. Explain the purpose of security groups in AWS.
2. What is the Shared Responsibility Model for EC2?

***

#### 💾 Elastic Block Storage (EBS)

* **EBS** is a network drive attached to EC2 for persistent storage.
  * Can be detached/reattached between instances.
  * Limited to a specific availability zone.

**Features:**

* Types: SSD, provisioned IOPS, etc.
* Scalable: Increase capacity as needed.

**💡 Exam Questions:**

1. Describe EBS and its main use cases.
2. How does EBS support data persistence in cloud environments?

***

#### ⚖️ Load Balancing

* **Elastic Load Balancer (ELB)** distributes incoming traffic to multiple EC2 instances.
  * AWS manages maintenance, scaling, and availability.

**💡 Exam Questions:**

1. What is an ELB, and why is it critical for cloud applications?
2. Describe how ELB ensures high availability.

***

#### 📈 Auto Scaling Group (ASG)

* **ASG** dynamically scales EC2 instances based on load:
  * **Scale out** for high traffic, **scale in** when load decreases.
  * Ensures a minimum and maximum number of instances.

**Benefits:**

* Elasticity across multiple AZs, integration with ELB for load management.

**💡 Exam Questions:**

1. How does an Auto Scaling Group (ASG) work?
2. Describe a scenario where an ASG would be beneficial.

***

#### 🗄️ Relational Database Service (RDS)

* **RDS** provides managed relational databases:
  * Supports SQL-based DBs (Postgres, MySQL, Aurora)
  * Offers automatic backups, scaling, and multi-AZ setup for disaster recovery.

**Advantages over EC2 DBs:**

* Managed service, backup, scaling, maintenance.

**💡 Exam Questions:**

1. What are the benefits of using RDS over deploying a database on EC2?
2. Explain multi-AZ deployment in RDS.

***

#### 📂 Simple Storage Service (S3)

* **Amazon S3** is a storage service for objects (files) within **buckets**:
  * Unique bucket names required globally.
  * Buckets are region-specific.

**Use Cases:**

* Backup, data archiving, static website hosting, big data analytics.

**💡 Exam Questions:**

1. What is Amazon S3, and how is data organized within it?
2. List three typical use cases for Amazon S3.
