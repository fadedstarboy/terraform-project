# Terraform Project(IAC)

![Screenshot from 2023-06-27 17-09-31](https://github.com/fadedstarboy/terraform-project/assets/51039641/670191bd-b9f9-44e8-97ac-e0b9b569903f)


This is the blueprint of the infrastructure I created. This contains the following:
1. Build a Reusable module for AWS
2. VPC Creation (1 VPC in this case)
3. Multiple Subnets Creation (2 public, 2 private)
4. Internet Gateway Creation 
5. Route Table creation 
6. Route table association 
7. EKS cluster + IAM roles+ Policies 
8. NodeGroup Creation + IAM roles +Policies

To run these terraform files, install terraform and use the following lines of code:

```
terraform init
```
```
terraform plan --var-file="./config/terraform.tfvars"
```
```
terraform apply --var-file="./config/terraform.tfvars"
```

In an ideal case scenario, Jenkins will be used to automate this process once the terraform files are ready.
