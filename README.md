![Blank diagram (2)](https://user-images.githubusercontent.com/14328150/190657024-463dd781-5748-43f2-9063-fcf320ffc3db.jpeg)

## Prerequisites:
1- You should have AWS account.<br/>  
2- You have to install and configure AWS CLI on your local machine.

## Steps:
1- If you want to create the infrastructure you have to **cd to bash folder** and run the bash with parameters first parameter for **stack name**,
second for **file name** and third for **parameters file name**.
<br/> ex: **./create.sh vpc vpc.yml parameters.json**, if you want to update the stack you have to use update.sh instead of create.sh . <br/>

2- When stack is created successfully you can get ELB url from output and if you go to the url you will find the website is working on apache server.

