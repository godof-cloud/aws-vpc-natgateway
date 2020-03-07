# VPC with NatGateway

## Description

Example that creates a VPC with 4 subnets in two different Availability Zones with the option to create a NatGateway.

You can find the full explanation of this template in: [https://godof.cloud/vpc-with-nat-gateway/](https://godof.cloud/vpc-with-nat-gateway/)

## Architecture

The cloudformation template will build the following resources:

- VPC

- Security Group

- 4 Subnets

- Internet Gateway

- 2 Route Tables (public y private)

- Elastic IP

- NatGateway (optional)

## Content

- cloudformation.yml: Cloudformation template that builds all the AWS resources. The template expects the following parameters.
