Main Goal
=========
Create VPC with 3 public/private subnets

Install nginx on web servers located in private subnet

Configure ALB in public subnets and connect to EC2 intances using target groups

Create a AutoScaling group that can scale ALB and instances
 
Set up CloudWatch scaling alarm in AutoScaling group that would increase by two instances
if CPU utilization is above 70% and decrease by two instances if CPU utilization is below 40%

Validation
==========
I was able to validate successfuly by spiking an instance over 70% and confirming the AutoScaling
group policies took into effect. Configuring SNS allowed me to promptly be notified that the configurations were working as expected. Two instances were spun up if CPU was over 70% and were shutdown if under 40%
as defined in the policies configured.  

Tech Stack
=========
VPC,ALB,SNS,EC2,AutoScaling group
