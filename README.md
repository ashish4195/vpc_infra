# vpc_infra
Terraform script to create a VPC infrastructure in AWS. It includes components such as a VPC, subnets, an internet gateway, route tables, and security groups.

Explanation:
Provider Block: Defines AWS as the cloud provider and sets the region.
VPC: Creates a Virtual Private Cloud with a 10.0.0.0/16 CIDR block.
Subnets:
Public Subnet (10.0.1.0/24) - Assigns public IPs.
Private Subnet (10.0.2.0/24) - Used for internal resources.
Internet Gateway: Provides internet access for public resources.
Route Table:
Public route table with a default route (0.0.0.0/0) to the internet.
Security Group:
Allows HTTP (port 80) and SSH (port 22) traffic from anywhere.
Allows all outbound traffic.
