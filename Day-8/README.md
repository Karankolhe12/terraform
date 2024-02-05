# MIGRATION TO TERRAFORM & DRIFT DETECTION

https://youtu.be/-4IMy5ihiiU


provider "aws" {
 region = "ap-south-1"
}
import {
id ="instance_id"
to = aws_instance.example
}

after init and plan this the create the genrated.tf file

provider "aws" {
 region = "ap-south-1"
}
all configuration file except ipv6

then this file configuration copy and paste in main.tf which means above and remove import block and this configuration ipv6 show an error after plan so remove both ipv6 line

then run command 
terraform import aws_instance.example instance_id

then create a terraform.tfstate file for our infrastrucature which is allready on aws
