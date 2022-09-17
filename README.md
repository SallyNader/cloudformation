![Blank diagram (2)](https://user-images.githubusercontent.com/14328150/190657024-463dd781-5748-43f2-9063-fcf320ffc3db.jpeg)

## ELB URL: http://webelb-1400881990.us-east-1.elb.amazonaws.com/ <br/>

## Project Description:
This project aims to create multiple ec2 instances on multiple zones to achive high availability, it deploys apache servers on private subnets and you can access your website through ELB url, you can also ssh to the private servers using basion hosts that is created on public subnets, also these instances have IAM role to perform actions on s3. <br/>

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

