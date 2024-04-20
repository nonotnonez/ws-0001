---
title : "EC2"
date : "`r Sys.Date()`"
weight : 1
chapter : false
pre : " <b> 5.1 </b> "
---
## AWS Infratructure as code with EC2
#### 1- Create Key Pairs
-   AWS key-pair name: **tf-keypair**

#### 2- Terraform configure
- Same configure files:  **visions.tf** , **provider.tf**  

- **terraform.tfvars**
![51](/ws-0001/images/5-iac/5.1-ec2/2-1-tfvars.png)

- **main.tf**
    - Review : Variables - VPC & Subnet
    ![51](/ws-0001/images/5-iac/5.1-ec2/main-1.png)

    - Review : Route table - Internet gateway - Assciate subnet with Route table
    ![51](/ws-0001/images/5-iac/5.1-ec2/main-2.png)

    - Review : Security Group
    ![51](/ws-0001/images/5-iac/5.1-ec2/main-3.png)

    - Review : EC2 Instance provision
    ![51](/ws-0001/images/5-iac/5.1-ec2/main-4.png)

#### 3 - Run Terraform
-   **docker-compose run --rm terraform init**
-   **docker-compose run --rm terraform plan**
-   **docker-compose run --rm terraform apply**

#### 4 - AWS Console Check:

- Review : Instances
![51](/ws-0001/images/5-iac/5.1-ec2/aws/1-ec2.png?featherlight=false&width=90pc)

- Review : VPC
![51](/ws-0001/images/5-iac/5.1-ec2/aws/2-vpc.png?featherlight=false&width=90pc)

- Review : Subnet
![51](/ws-0001/images/5-iac/5.1-ec2/aws/3-subnet.png?featherlight=false&width=90pc)

- Review : Route table
![51](/ws-0001/images/5-iac/5.1-ec2/aws/4-rtb.png?featherlight=false&width=90pc)

![51](/ws-0001/images/5-iac/5.1-ec2/aws/4-rtb-2.png?featherlight=false&width=90pc)

- Review : Internet Gateway
![51](/ws-0001/images/5-iac/5.1-ec2/aws/5-igw.png?featherlight=false&width=90pc)

- Review : Security Group
![51](/ws-0001/images/5-iac/5.1-ec2/aws/6-sg.png?featherlight=false&width=90pc)

![51](/ws-0001/images/5-iac/5.1-ec2/aws/6-sg-2.png?featherlight=false&width=90pc)

#### 5 - Clean up:
- **docker-compose run –rm terraform destroy**