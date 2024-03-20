# Cloud Migration Project (Code to be Uploaded)

This project has the scenario of migrating companies’ pre-existing on-premises datacentre to the Cloud.

The purpose of the module is to write a 2500-3000 word Service Management System (SMS) document for the newly developed system.

The infrastructure is the technical, practical aspect of the module in order to experiment and build a more modern and true-to-life deployment as well as test our adaptability to challenges as each one of us received completely different set requirements and pre-existing systems that we had to migrate or replace in order to meet business requirements as well as bring improvements.

## Infrastructure

1. Website - .NET Core MVC web application with M SQL Server database deployed in Kubernetes in AWS EKS
2. Lightweight Active Directory Service using Samba
3. Mass storage using AWS S3 buckets mounted as network-attached storage to Windows and Linux instances.
4. High-speed storage using NFS v4 (AWS EFS)
5. CI/CD (Continuous Integration & Deployment) pipeline for automating testing and deployment using GitHub Actions and AWS CodeBuild (Testing & Building)
6. AWS Secret Manager for storing and auto-rotating database credentials in the code (improving security and resilience).
7. AWS CloudWatch, CloudTrail, Macie and Inspector are used for continuous tracking, logging, and alerting on various services and resources in the infrastructure.
8. AWS RDS is used to host the Microsoft SQL Server instance.


## Software Part - Web Application (Source Code, Docker Image and YAML deployment scripts to be uploaded)

The application is developed using the MVC .NET framework in order to create a simple, performant web application that can perform CRUD operations to the database.

  The application is containerised in Kubernetes Clusters using AWS EKS (Elastic Kubernetes Services).
  It is also Auto-Scaled and Load Balanced.
  The database code is generated by the C# code using EF Core (Entity Framework) mapping, by using the models defined, EF Core generates the SQL syntax directly by using the connection it has with the instance. 
