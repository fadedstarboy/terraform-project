# Terraform Project(IAC)

![image](https://github.com/fadedstarboy/terraform-project/assets/51039641/e87a3065-04d5-4866-ab1e-bc46dcf7a03e)

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
