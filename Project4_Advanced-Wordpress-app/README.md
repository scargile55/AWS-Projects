Main Goal
=========
Create a VPC with three public/private subnets
Create MySQL databases in each private subnets
Setup and configure Wordpress on instances in private subnets and connect them to RDS using security groups
Configure Application Load Balancers in public subnets and connect to EC2 instances using target groups
	- EC2 instances were configure using Systems Session Manger instead of using a Bastion host

Validation:
==========
I was able to validate successfully by confirming that the ALB DNS URL directed me to the appropriate Wordpress page

Tech Stack:
===========
ALB, EC2, RDS, VPC 

