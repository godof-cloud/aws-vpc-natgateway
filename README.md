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

- cloudformation.yml: Cloudformation template that builds all the AWS resources. The template expects the following parameters:
  
  - prefix: This value will be appended in the resource's name that we are going to create to be sure that there is any conflict with other resources that you might have, by default is *custom*.
  
  - sgCidr: Custom IP to configure the Security Group to allow access only from the specified IP.
  
  - vpcCidrBlock: IP block for the VPC network , for example, 10.0.0.0
  
  - subnetCidrBlocks: IP blocks for the subnets separated by commas, for example, 10.0.1.0, 10.0.2.0, 10.0.3.0, 10.0.4.0
  
  - vpcCidrRange: IP range for the VPC, by default 16.
  
  - subnetCidrRange: IP range for the Subnets, by default 24.
  
  - createNatGateway: Flag to decide if the template would create a NatGateway.
