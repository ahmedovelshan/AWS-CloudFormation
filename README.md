# AWS ECS CloudFormation Templates

This repository contains a set of AWS CloudFormation templates designed to create a complete infrastructure for hosting containerized applications on Amazon Elastic Container Service (ECS). The primary goal is to demonstrate practical experience in setting up AWS infrastructure using CloudFormation.

## Purpose

These templates are part of my portfolio to showcase my experience with AWS CloudFormation and ECS. They create an ECS environment with necessary networking, security, and load balancing components.

## Prerequisites

- An AWS account with appropriate permissions to create VPCs, Security Groups, Load Balancers, and ECS clusters.
- AWS CLI or AWS Management Console to deploy CloudFormation stacks.

## Deployment Instructions

Follow these steps to deploy the infrastructure:

1. **VPC Configuration**
    - Deploy `vpc.yaml` to create a Virtual Private Cloud (VPC) with subnets, route tables, and internet gateways.

2. **Security Groups**
    - Deploy `sg.yml` to create security groups for the application and load balancer.

3. **Application Load Balancer**
    - Deploy `alb.yml` to create an Application Load Balancer (ALB) that distributes traffic to your ECS services.

4. **ECS Cluster**
    - Deploy `ecs.yml` to create an ECS cluster, task definitions, and services.

## Architecture Overview

- **VPC:** Provides isolated networking for your ECS environment.
- **Security Groups:** Manage inbound and outbound traffic for your ECS services and ALB.
- **ALB:** Distributes incoming traffic to ECS services based on routing rules.
- **ECS Cluster:** Hosts your containerized applications with auto-scaling and high availability.

## Usage

These templates are intended to be used as a foundation for deploying containerized applications on AWS. They can be extended or modified based on specific application needs.
