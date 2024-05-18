# EC2: Launching a Instance

## Overview
This project demonstrates how to launch and manage an EC2 instance using AWS free tier. In this prjoect I launched, connected to, use a Linux instance, and then terminate the instance.

## Steps

1. **Sign in to the AWS Management Console**
   - In this case, I do not have any users with administrative access so I have created one to be able to complete this project without using my root user account.
   - To create the IAM user, I navigated to the IAM service and selected *Users* on the right-hand side under the *Access management* dropdown of the Dashboard.
   - From here I pressed the orange *Create user* button on the top-right, then gave set a user name for my new IAM user. 
   - I decided to allow this user to have AWS Management Consol Access, then proceeded to creat the IAM user and set a custom password. 
   - In the permissions step, the only policies I attached were the permissions related to giving administrator access. 
   - After creating my new IAM user, I signed out of my root account and signed into the new IAM user account with admin access. 

2. **Launching an Instance**
   - After signing in, I navigated to the EC2 service Dashboard and clicked *Launch instance*
   
   ![Launch Instance Button](EC2/Launch-Instance-Button.png)

   - I input a name for the instance under *Name and tags* '(Linux Instance)'.
   - After naming, I chose the operating system I wnated to use '(in this case, the HVM version of the Amazon Linux 2 AMI)'
   - **Note:** AMI = Amazon Machine Image

   ![Choosing Instance](EC2/Choosing-Instance.png)

   - When selecting th instance type, I kept the default t2.micro instance type.
   - Then created a key pair '(since I did not have one set up already)'

   ![Instance Type and Key Pair](EC2/Instance-Type-Key-Pair.png)

   - I kept all other settings default and pressed *Launch instance*. 
   - In the next screen, I chose *View all instances* to close the confirmation page and return to the console to wait for the instance to pass it's status check.

3. **Connect to the Instance**
   - While on the *Instances* page, I connected to the instance by checking the box next to the instance I just created, clicking the *Actions* dropdown, and then pressing the *Connect* button.
   - I used *EC2 Instance Connect* and then connected.

   ![Connect](EC2/Connect.png)

   ![Connected](EC2/Connected.png)

4.**Terminate the Instance**
   - To terminate the instance, I first navigated back to the *Instances* page.
   - I selected the instance using the check box.
   - Using the *Instance state* dropdown, I selected *Terminate instance*.

   ![Terminate](EC2/Terminate.png)

   ![Terminate Confirmation](EC2/Terminate Confirmation.png)

## Resources
- [Launch Your First Amazon EC2 Instance](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html)
