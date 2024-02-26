# AWS Lambda Terraform Template

An opinionated guide on setting up AWS Lambda with Terraform.

## The Problem

AWS Lambda enables developers to swiftly provision computational resources and execute their code through its serverless architecture via the AWS console. However, the complexity arises when setting up initial configurations and managing them, especially in scenarios where multiple Lambda functions require the same configuration settings or adjustments over time. This situation complicates the task of teams in managing and reverting changes when necessary.

## The Solution

Infrastructure as Code (IoC) with Terraform!

IoC tools such as Terraform allows us to provision AWS resouces in a declarative mannner in code, making the process of provising cloud resources:

- **Trackable** - The use of git's commit history allows for the tracking of changes and configurations over time, ensuring that modifications to the infrastructure are well-documented and traceable.
- **Verifiable** - Allows for the verification of configurations against the actual state in the cloud. This ensures that the configuration described in the code matches the current state of resources in on the AWS account.
- **Reapeatable** - Terraform ensures that each configuration is consistent and repeatable, allowing for consistent provisioning of resources across different development environments.

In this template, we will answer the following questions:

1. How to provision AWS Lambda using Terraform?
2. How to setup a Terraform remote backend?
3. How to create a Terraform module?
4. How to setup CI/CD pipeline with GitHub Actions?

## Features

- Terraform S3 Remote Backend
- Lambda deployment package stored in S3
- Terraform Lambda and S3 Modules
- GitHub Actions for CI/CD
