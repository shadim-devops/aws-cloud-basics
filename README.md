# AWS Cloud Basics

A hands-on AWS infrastructure project demonstrating identity and access management, account security, cost monitoring, Amazon S3 operations, and resource inspection with the AWS CLI.

## Overview

This project documents practical AWS administration tasks, including IAM groups and users, permissions, root account MFA, CLI profiles, a monthly budget, and basic S3 operations.

## AWS Services and Tools

- AWS Identity and Access Management (IAM)
- AWS Command Line Interface (AWS CLI)
- Amazon Simple Storage Service (S3)
- AWS Budgets
- Amazon EC2 (AMI and security group inspection)
- AWS Security Token Service (STS)

## Project Structure

```text
aws-cloud-basics/
├── README.md
├── docs/
│   ├── identity-and-security.md
│   └── cli-and-storage.md
└── .gitignore
```

## Implemented Work

### Identity, Security, and Cost Management

- Created IAM groups for administrators, developers, and read-only access.
- Assigned access policies to the groups.
- Created IAM users and assigned group memberships.
- Enabled multi-factor authentication (MFA) for the root account.
- Configured AWS CLI access for different users and verified identities.
- Created a monthly AWS budget with alerts.

See [Identity and Security](docs/identity-and-security.md).

### AWS CLI and Storage

- Created an S3 bucket and uploaded and downloaded a file.
- Listed available Amazon Machine Images (AMIs).
- Inspected EC2 security groups.
- Listed IAM users and inspected user details.
- Listed S3 buckets using the AWS CLI.

See [CLI and Storage](docs/cli-and-storage.md).

## Requirements

- An AWS account with permissions appropriate for the operations
- AWS CLI v2 installed and configured
- An AWS Region selected for regional operations

## Security Notes

Never commit access keys, secret keys, session tokens, or AWS CLI credential files. Prefer short-lived credentials and least-privilege IAM permissions. The commands in the documentation are examples and may require adaptation to your account and Region.

## Project Status

Completed as a practical AWS administration exercise. This repository describes the completed tasks and provides representative commands; it does not contain automated infrastructure deployment code.
# aws-cloud-basics
# aws-cloud-basics
