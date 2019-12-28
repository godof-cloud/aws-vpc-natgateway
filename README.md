# VPC with NatGatewat



## Description

Example of that creates a VPC with 8 subnets in two different Availability Zones with the option to create a NatGateway



## Architecture

The cloudformation template will build the following resources:

- VPC

- Security Group

- 8 Subnets

- Internet Gateway

- 2 Route Tables (public y private)

- Elastic IP

- NatGateway (optional)



## Content

- cloudformation.yml: Cloudformation template that builds all the AWS resources. The template expects the following parameters:
  
  - prefix: A prefix that will be set in the name of all the resources to be sure that all the names used are unique, by default vpc-gw
  
  - vpcCidrBlock: IP that will be assigned with the VPC
  
  - subnet1CidrBlock: Subnet 1 IP
  
  - subnet2CidrBlock: Subnet 2 IP
  
  - subnet3CidrBlock: Subnet 3 IP
  
  - subnet4CidrBlock: Subnet 4 IP
  
  - subnet5CidrBlock: Subnet 5 IP
  
  - subnet6CidrBlock: Subnet 6 IP
  
  - subnet7CidrBlock: Subnet 7 IP
  
  - subnet8CidrBlock: Subnet 8 IP
  
  - vpcCidrRange: IP Range for the VPC IP, by default 16
  
  - subnetCidrRange: IP Range for the Subnet's IP, by deault 24
  
  - createNatGateway: Flag to enable the creation of the NatGateway


