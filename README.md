#  Terraform AWS S3 Static Website Hosting

## Project Description:
Developed a streamlined infrastructure for hosting a static website using Terraform and Amazon Web Services (AWS) S3. The primary goal of this project is to demonstrate the automated provisioning and deployment of a web hosting solution for static websites. 
This project serves as an excellent foundation for hosting various types of static websites, including personal blogs, portfolio sites, or small business websites.

## Overview:



## Steps :

### Step 1: Set Up Your Development Environment

Install Terraform and the AWS Command Line Interface (CLI) on your local machine.
Configure your AWS credentials by running ```aws configure``` and providing your AWS access key and secret key.

### Step 2: Define Your Website Content

To prepare static website files (HTML), place them in the directory where your Terraform configuration files are located. Name the main HTML file "index.html," and optionally, you can also include an "error.html" file. Created a static website that lists best books for cloud and devops.

### Step 3: Terraform Configuration File Syntax

If we want to Create a terraform configuration file we have to use .tf (e.g., main.tf) to define the infrastructure as code using terraform.

### Step 4: Define your Configuration Files in your IDE
### Define the AWS provider and required resources like S3 buckets, IAM roles, and policies
1. Define ```provider.tf``` file.
2. In your Integrated Development Environment (IDE), open the terminal and navigate to the directory where you have created these configuration files.
3. After navigating to the directory where your configuration files are located in your IDE's terminal, you can run the following command to initialize Terraform and prepare it for use with AWS:

```shell
terraform init
```

Running `terraform init` will install the necessary plugins and modules required for connecting to AWS and managing your infrastructure.<br>
4. And then define __resource.tf__ file.

5. Then below command for creating the bucket :
```
terraform apply -auto-approve
```

6. The code above will apply the necessary configurations for features such as static website hosting, bucket policies, and blocking public access to your bucket.


### Step 5: Define the Output file

1. We use an output file to obtain your website link in your IDE, eliminating the need to access the link through the AWS Console.
2. Define __output.tf__ terraform file.
3. And then run the following command :
```
terraform apply -auto-approve
```
4. It will give your website link as output 

### Step 6: Verify the Output 

Copy the link and paste it in your browser.