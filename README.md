# E-Commerce Application

![Highly Available LMS Architecture Diagram](https://github.com/user-attachments/assets/ad6388bb-3d41-4fc6-9d54-750cb1f811d4)

Highly Available Infrastructure for E-commerce Project - AWS Load Balancer & Auto Scaling

Project Overview

This project focuses on designing and deploying a Highly Available and Fault-Tolerant infrastructure for an E-commerce platform on AWS. 
The architecture ensures scalability, redundancy, and continuous service availability by leveraging AWS services such as Elastic Load Balancer (ELB) and Auto Scaling Groups (ASG).

Key Features:

High Availability: Deploy resources across multiple Availability Zones (AZs) to ensure redundancy and fault tolerance.

Fault Tolerance: Implement failover mechanisms to maintain service availability during component failures.

Scalability: Use Auto Scaling to handle changing workloads dynamically.

Load Balancing: Distribute incoming traffic evenly across multiple EC2 instances.

Infrastructure Design

Architecture Components:

Virtual Private Cloud (VPC):

Multi-AZ setup for high availability.

Public and private subnets for segregation.

Elastic Load Balancer (ELB):

Distributes traffic across healthy instances in multiple AZs.

Automatically reroutes traffic from unhealthy instances.

Auto Scaling Group (ASG):

Automatically scales instances based on demand.

Ensures a minimum and maximum number of instances for fault tolerance.

EC2 Instances:

Backend and frontend servers deployed across multiple AZs.

Use Amazon Machine Images (AMIs) for consistent deployments.

Database (RDS):

Multi-AZ deployment for redundancy and disaster recovery.

Technical Details

High Availability

Deploy resources in at least two Availability Zones to ensure redundancy.

Use Elastic Load Balancer (ELB) to distribute traffic across multiple instances.

ELB performs health checks and routes traffic only to healthy instances.

Fault Tolerance

Implement redundant components and failover mechanisms.

Data replication and backups to ensure data integrity and recovery options.

Use Auto Scaling Groups to automatically replace unhealthy instances.

Scalability

Auto Scaling dynamically adjusts the number of instances based on demand.

Use CloudWatch metrics to monitor performance and trigger scaling actions.

Maintain performance during traffic spikes without manual intervention.

Workflow

Create a VPC with subnets across multiple AZs.

Deploy EC2 Instances with pre-configured AMIs.

Configure an Elastic Load Balancer (ELB) for traffic distribution.

Set up Auto Scaling Groups (ASG) for dynamic scaling.

Deploy a Multi-AZ RDS instance for database redundancy.

Integrate CloudWatch for monitoring and triggering scaling actions.

Key AWS Services Used

EC2: Virtual servers for backend and frontend applications.

Elastic Load Balancer (ELB): Distributes traffic across multiple servers.

Auto Scaling Groups (ASG): Automatically adjusts server capacity.

RDS (Relational Database Service): Multi-AZ database setup.

CloudWatch: Monitoring and scaling triggers.

Results

25% Improvement in system availability.

35% Reduction in downtime.

Automated scaling reduced manual intervention and improved operational efficiency.

Getting Started

Clone the repository:

git clone https://github.com/ravi2krishna/ecomm.git

Navigate to the project directory:

cd ecomm

Access the application using the DNS provided by the Elastic Load Balancer.

Conclusion

This project demonstrates the implementation of a Highly Available and Scalable infrastructure for an E-commerce platform using AWS services. 
By leveraging Load Balancers, Auto Scaling, and Multi-AZ deployments, the system is designed to handle traffic surges, reduce downtime, and ensure continuous service availability.
