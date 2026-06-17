# AWS EC2 IAM Role S3 Access Project

##  Project Overview

Implemented secure access from an Amazon EC2 instance to Amazon S3 using an IAM Role. This project demonstrates AWS best practices by eliminating the need for access keys and using temporary credentials provided by AWS.

##  AWS Services Used

- Amazon EC2
- AWS IAM
- IAM Roles
- Amazon S3
- AWS CLI
- AWS STS

##  Steps Followed

1. Created an IAM Role for EC2
2. Attached the AmazonS3ReadOnlyAccess policy
3. Attached the IAM Role to a running EC2 instance
4. Verified the role using the EC2 Metadata Service
5. Verified identity using AWS STS
6. Accessed S3 buckets from EC2 using the AWS CLI

##  Security Benefit

Instead of storing AWS Access Keys on the server, the EC2 instance receives temporary credentials automatically through the IAM Role.

EC2 → IAM Role → AWS Services

This approach follows AWS security best practices and reduces the risk of credential exposure.

##  Outcome

Successfully configured an EC2 instance to access Amazon S3 securely using an IAM Role and verified access through AWS CLI commands.

##  Key Learnings

- IAM Roles and temporary credentials
- EC2 Metadata Service (IMDS)
- AWS STS identity verification
- Secure service-to-service authentication
- S3 access management using IAM
