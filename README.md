# TF-AWS-IGW

## Terraform AWS Internet Gateway Module

This Terraform module creates an Internet Gateway in AWS and associates it with an existing VPC.

## Usage

To use this module, include it in your Terraform configuration, specifying the required variables.

### Example

```hcl
module "internet_gateway" {
  source = "github.com/Swanson-IT/TF-AWS-IGW" # Change to a release tag or version if needed

  vpc_id = "vpc-1234567890abcdef0"   # Replace with your VPC ID
  name   = "my-internet-gateway"     # Desired name for the Internet Gateway
}