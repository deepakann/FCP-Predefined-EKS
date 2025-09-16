# FCP-Predefined-EKS
Repository to store Terraform Configuration Files using Predefined Modules for VPC and EKS

Provisioning Infrastructure via Terraform Configuration using AWS Cloud Providers.

Have used Terraform Predefined Modules to create VPC and EKS:-

VPC:
terraform-aws-modules/vpc/aws | Terraform Registry
Source Code: github.com/terraform-aws-modules/terraform-aws-vpc 

EKS:
terraform-aws-modules/eks/aws | Terraform Registry
Source Code: github.com/terraform-aws-modules/terraform-aws-eks
Below resources will get created using Terraform built-in Module?:
<img width="1727" height="845" alt="image" src="https://github.com/user-attachments/assets/baf47cb4-c032-4fbd-884d-dfc934913c63" />

Errors faced during Terraform plan:
<img width="1664" height="1027" alt="image" src="https://github.com/user-attachments/assets/24541014-8b44-4593-8b99-c04012770be9" />
Update Provider Version:
<img width="1664" height="1027" alt="image" src="https://github.com/user-attachments/assets/ea4b3e4f-9eb2-4571-bcf6-48fd83c86a59" />
<img width="1545" height="294" alt="image" src="https://github.com/user-attachments/assets/1b38a554-b33d-4a69-9357-4c99fc6c8250" />



For now, EKS Nodegroup is defined of instance type -> t3.medium. 
This is defined in variables.tf, and hence can be changed at any point of time in the terraform configuration files in future as per client requirement.

**Remote backend with S3 + DynamoDB locking Enabled:**
Configured Terraform remote backend leveraging Amazon S3 (with versioning enabled for state rollback) and integrated DynamoDB state locking to ensure consistency and prevent concurrent state operations.

GitHub:

**EKS Cluster Setup using Predefined Terraform Modules:**
https://github.com/deepakann/FCP-Predefined-EKS.git

**EKS Cluster Setup with Userdefined Terraform Modules:**
https://github.com/deepakann/FCP-Userdefined-EKS.git

