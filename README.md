# TF_FN-SecurityGroups_Public
## **Overview**
This repository combines two examples to demonstrate Terraform's powerful capabilities in managing AWS resources efficiently. Explore how to create and manage security groups with ease, along with setting up EC2 instances tailored to your needs.

# Examples
## **TF_FN-ForEachExample1**
## Description:
This example dives into the usage of the for_each meta-argument in Terraform, alongside the toset and tomap functions. Learn how to efficiently create and manage security groups in AWS, from configuring SSH traffic to defining web access rules. Optimize your infrastructure configurations with ease and scalability.

## Usage:
Explore the c3-securitygroups.tf file to see how security group rules are defined using for_each. The output_v3_1, output_v3_2, output_v3_3, and output_v3_4 outputs provide insights into the availability zones and supported instance types.

## **TF_EC2-Example2**
## Description:
In this example, discover Terraform scripts designed to effortlessly create EC2 instances in AWS. The scripts include configurations for security groups, allowing SSH traffic (port 22) and web traffic (ports 80 and 443). Customize your infrastructure by adjusting input variables such as region, instance type, and EC2 key pair.

## Usage:
Navigate through the c4-ami-datasource.tf, c5-ec2instance.tf, c6-outputs.tf, and c7-get-instancetype-supported-per-az-in-a-region.tf files to understand the EC2 instance creation process. Use terraform apply to deploy your EC2 instances and observe the outputs for availability zones and supported instance types.

# Instructions:
- Clone this repository:
```
git clone https://github.com/gerardodavidlopezcastillo/TF_FN-SecurityGroups_Public.git
```
- Navigate to the desired example folder:
- For Example 1:
```
cd TF_FN-SecurityGroups_Public/TF_FN-ForEachExample1
```
- For Example 2:
```
cd TF_FN-SecurityGroups_Public/TF_EC2-Example2
```
- Initialize Terraform:
```
terraform init
terraform plan
terraform apply -auto-approve
```
- Explore the created resources in your AWS console.
- Clean up resources when done:
```
terraform destroy -auto-approve
```
