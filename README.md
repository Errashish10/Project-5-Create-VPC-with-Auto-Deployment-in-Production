# Project-5-Create-VPC-in-Production
Design and build a production-ready AWS Virtual Private Cloud (VPC) architecture with public and private subnets, routing, and essential networking components
| Resource                | Purpose                                           |
| ----------------------- | ------------------------------------------------- |
| VPC                     | Isolated network environment                      |
| Subnets                 | Public for web/app, private for databases/backend |
| Route Tables            | To manage routing for subnets                     |
| Internet Gateway        | For public internet access                        |
| NAT Gateway             | Allow private subnet outbound access              |
| Security Groups         | Fine-grained traffic control                      |
| NACLs (optional)        | Subnet-level traffic filtering                    |

| Element          | Detail                    |
| ---------------- | ------------------------- |
| VPC CIDR         | `10.0.0.0/16`             |
| Public Subnet 1  | `10.0.1.0/24` (AZ1)       |
| Public Subnet 2  | `10.0.2.0/24` (AZ2)       |
| Private Subnet 1 | `10.0.3.0/24` (AZ1)       |
| Private Subnet 2 | `10.0.4.0/24` (AZ2)       |
| IGW              | Attached to VPC           |
| NAT Gateways     | One in each AZ (with EIP) |

 

