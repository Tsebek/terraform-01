# Terraform-101

## Summary
This is an overview of chapters 1-3 of the book "Terraform: Up and Running".

## Getting Started with Terraform

Terraform can provision infrastructure across public cloud providers such as AWS, Azure, and Google Cloud. We are going to use AWS as an example. 
We will do the following steps:
- Setting up your AWS account
- Installing Terraform
- Deploying a single server
- Deploying a single web server
- Deploying a configurable web server
- Deploying a cluster of web servers
- Deploying a load balancer
- Cleaning up

### Setting Up Your AWS Account

- If you don’t already have an AWS account, head over to https://aws.amazon.com and sign up. Initially you sign in as the root user.
- Create a more-limited user account. Navigate to IAM (Identity and Access Management) service.
- Click Users.
- Click the Create User button.
- Enter a name for the user.
- Click the Next button.
- Step 2 allows you to set permissions for this new user. You can create different users with various permissions to get access to Glue, S3, etc. You can choose "Add user to group" option to create a user with no permission, and add permission later. To run the examples in this book, the easiest way to get started is to add the `AdministratorAccess` Managed Policy, so we choose "Attach policies directly" option.
- Click the Next button.
- Review everything and click Create user button.
- Click on the user that you've just created in the list of all users.
- In the Summary table click Create access key.
- You can choose "Other" option on the step 1, skip Step 2 and Create access key.
- You will see an Access Key and a Secret Access Key. You must save these immediately because they will never be shown again, and you’ll need them later on in this tutorial.
- After you’ve saved your credentials, click the Close button. You’re now ready to move on to using Terraform.

