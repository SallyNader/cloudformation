![Blank diagram (2)](https://user-images.githubusercontent.com/14328150/190657024-463dd781-5748-43f2-9063-fcf320ffc3db.jpeg)


## Project Description:
This project aims to:<br/>
•	Create VPC with public and private subnets, NAT gateway and internet gateway.<br/>
•	Create auto scaling group to deploy multiple bastion hosts on multiple availability zones.<br/>
•	Create auto scaling group to deploy private EC2 instances on multiple availability zones.<br/>
•	Create ELB to access web application in the private EC2 instances.<br/>
•	Create IAM role to perform actions on s3 and attach it to EC2 instances.
 <br/>

## Prerequisites:
1- You should have AWS account.<br/>  
2- You have to install and configure AWS CLI on your local machine.
<br/>

## Steps:
1- Add your parameters values to vpc-parameters.json and infra-parameters.json files. <br/>
2- If you want to create the infrastructure you have to **cd to bash folder** and run the bash script with parameters, first parameter for **stack name**,
second for **file name** and third for **parameters file name**.
<br/> ex: **./create.sh vpc vpc.yml parameters.json**, if you want to update the stack you have to use update.sh instead of create.sh . <br/>

3- When stack is created successfully you can get ELB url from output and if you go to the url you will find the website is working on apache server.

