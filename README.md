AWS Project: Deploying Applications in Private Subnets

Project Overview

This project demonstrates a secure and highly available AWS architecture where web applications are deployed on EC2 instances running inside private subnets and exposed to users through an Application Load Balancer (ALB).

The objective of this project was to gain hands-on experience with AWS networking, security, load balancing, and auto scaling concepts while following cloud architecture best practices.

Architecture Components

Amazon VPC

Public Subnets (2)

Private Subnets (2)

Internet Gateway

NAT Gateway

Application Load Balancer (ALB)

Auto Scaling Group

Amazon EC2 Instances

Security Groups

S3 Gateway Endpoint

Architecture Flow

User Request → Application Load Balancer → Target Group → EC2 Instances (Private Subnets) → Web Application (index.html)

The Application Load Balancer receives incoming requests and distributes traffic across EC2 instances running inside private subnets. The instances remain protected from direct internet access, improving security.

Implementation Steps

Created a custom VPC.

Created public and private subnets across multiple Availability Zones.

Attached an Internet Gateway to the VPC.

Configured NAT Gateway for outbound internet access from private subnets.

Configured route tables for public and private subnets.

Created security groups for controlled access.

Launched EC2 instances in private subnets.

Deployed a sample HTML web application.

Created a Target Group.

Configured an Application Load Balancer.

Attached EC2 instances to the Target Group.

Configured Auto Scaling Group.

Verified application accessibility through the Load Balancer DNS endpoint.

AWS Services Used

Amazon VPC

Amazon EC2

Application Load Balancer (ALB)

Auto Scaling Group

NAT Gateway

Internet Gateway

Security Groups

Amazon S3 Gateway Endpoint

Key Learnings

Understanding VPC networking concepts.

Difference between public and private subnets.

Implementing secure architectures using private EC2 instances.

Configuring Application Load Balancers.

Using Auto Scaling for high availability.

Managing network access with Security Groups and Route Tables.

Project URL

https://aws-prod-example-1919309594.us-east-1.elb.amazonaws.com/

Outcome

Successfully deployed a web application hosted on EC2 instances within private subnets while providing secure public access through an Application Load Balancer. The solution demonstrates scalability, security, and high availability using core AWS services.

Author

Hithesh Gowda B.E. Information Science & Engineering Malnad College of Engineering
